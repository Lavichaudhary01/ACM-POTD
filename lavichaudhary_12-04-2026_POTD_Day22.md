# Flood Fill
class Solution:
    def floodFill(self, image: list[list[int]], sr: int, sc: int, color: int) -> list[list[int]]:
        original = image[sr][sc]
        if original == color:
            return image
        def fill(r, c):
            if r < 0 or r >= len(image) or c < 0 or c >= len(image[0]):
                return
            if image[r][c] != original:
                return
            image[r][c] = color
            fill(r + 1, c)
            fill(r - 1, c)
            fill(r, c + 1)
            fill(r, c - 1) 
        fill(sr, sc)
        return image

  <img width="1899" height="911" alt="image" src="https://github.com/user-attachments/assets/0162a6a6-cd99-4678-b050-a0a6a0ce64cc" />
