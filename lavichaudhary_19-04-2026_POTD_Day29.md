# Fibonacci Number
class Solution:
    def fib(self, n: int) -> int:
        if n <= 1:
            return n
        prev2 = 0
        prev1 = 1 
        for _ in range(2, n + 1):
            current = prev1 + prev2
            prev2 = prev1
            prev1 = current            
        return prev1

  <img width="1919" height="966" alt="image" src="https://github.com/user-attachments/assets/5a422979-a019-478d-a36a-b016e4720856" />
