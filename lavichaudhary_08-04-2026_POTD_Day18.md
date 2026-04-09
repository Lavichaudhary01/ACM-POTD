# Remove All Adjacent Duplicates In String
class Solution:
    def removeDuplicates(self, s: str) -> str:
        stack = []
        for char in s:
            if stack and stack[-1] == char:
                stack.pop()
            else:
                stack.append(char)
        return "".join(stack)
        


<img width="1902" height="908" alt="Screenshot 2026-04-09 135858" src="https://github.com/user-attachments/assets/251b8965-4f03-45f4-90ae-654ad2cfc590" />
