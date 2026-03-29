#Rotate Array
class Solution:
    def rotate(self, nums: list[int], k: int) -> None:
        n = len(nums)
        k %= n
        def reverse(start: int, end: int):
            while start < end:
                nums[start], nums[end] = nums[end], nums[start]
                start += 1
                end -= 1
        reverse(0, n - 1)
        reverse(0, k - 1)
        reverse(k, n - 1)
        
<img width="1919" height="969" alt="Screenshot 2026-03-28 010100" src="https://github.com/user-attachments/assets/1a90bf68-9ca3-4625-8c4a-5d8891c318f0" />
