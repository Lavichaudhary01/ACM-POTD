# Min Cost Climbing Stairs
class Solution:
    def minCostClimbingStairs(self, cost: list[int]) -> int:
        prev2 = 0
        prev1 = 0
        for i in range(2, len(cost) + 1):
            current = min(prev1 + cost[i-1], prev2 + cost[i-2])
            prev2 = prev1
            prev1 = current            
        return prev1

  <img width="1919" height="969" alt="image" src="https://github.com/user-attachments/assets/a1e26196-7346-4126-b60f-ca1515a56f5f" />
