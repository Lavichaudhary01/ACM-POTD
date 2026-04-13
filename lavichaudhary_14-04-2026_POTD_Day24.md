# Find Center of Star Graph
class Solution:
    def findCenter(self, edges: list[list[int]]) -> int:
        a, b = edges[0]
        c, d = edges[1]
        if a == c or a == d:
            return a
        return b

  <img width="1919" height="964" alt="image" src="https://github.com/user-attachments/assets/793ebe05-4bf2-4055-9290-3f4b1d6ef24b" />
     
