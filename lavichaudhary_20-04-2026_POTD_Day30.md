# Power of Two
class Solution:
    def isPowerOfTwo(self, n: int) -> bool:
        if n <= 0: 
            return False
        while n % 2 == 0:
            n //= 2
        return n == 1

  <img width="1911" height="970" alt="image" src="https://github.com/user-attachments/assets/5f9d788f-65c6-48d6-b4fb-4488c67fc233" />
