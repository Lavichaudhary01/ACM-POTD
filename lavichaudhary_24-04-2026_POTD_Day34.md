# House Robber
class Solution:
    def rob(self, nums: list[int]) -> int:
        rob1, rob2 = 0, 0
        for n in nums:
            temp = max(n + rob1, rob2)
            rob1 = rob2
            rob2 = temp            
        return rob2

<img width="1919" height="963" alt="image" src="https://github.com/user-attachments/assets/77f89bdd-e959-4cfe-becc-390812a204b2" />
