# Pascal's Triangle
class Solution:
    def lengthOfLIS(self, nums: list[int]) -> int:
        if not nums:
            return 0
        dp = [1] * len(nums)
        for i in range(len(nums)):
            for j in range(i):
                if nums[i] > nums[j]:
                    dp[i] = max(dp[i], dp[j] + 1)          
        return max(dp)  

  <img width="1919" height="969" alt="image" src="https://github.com/user-attachments/assets/a4e4202e-bdee-45c9-a9fd-e8a69900213b" />
