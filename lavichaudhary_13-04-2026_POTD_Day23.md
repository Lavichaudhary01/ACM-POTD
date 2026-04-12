# Find the Town Judge
class Solution:
    def findJudge(self, n: int, trust: list[list[int]]) -> int:
        scores = [0] * (n + 1)
        for a, b in trust:
            scores[a] -= 1
            scores[b] += 1
        for i in range(1, n + 1):
            if scores[i] == n - 1:
                return i         
        return -1

   <img width="1919" height="970" alt="Screenshot 2026-04-13 004641" src="https://github.com/user-attachments/assets/6342f580-1d1f-46c3-a87d-11ecf21c1f0d" />
