# Climbing Stairs
class Solution:
    def climbStairs(self, n: int) -> int:
        if n <= 2:
            return n
        first = 1  
        second = 2         
        for _ in range(3, n + 1):
            current = first + second
            first = second
            second = current            
        return second

<img width="1919" height="975" alt="image" src="https://github.com/user-attachments/assets/9ca21edc-4a5d-4979-be68-02181a625205" />
        
