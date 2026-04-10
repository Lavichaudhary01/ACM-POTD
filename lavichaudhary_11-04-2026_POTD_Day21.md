# Make The String Great
class Solution:
    def makeGood(self, s: str) -> str:
        stack = []      
        for char in s:
            if stack and abs(ord(stack[-1]) - ord(char)) == 32:
                stack.pop()
            else:
                stack.append(char)      
        return "".join(stack)


  <img width="1901" height="906" alt="image" src="https://github.com/user-attachments/assets/d815ceb7-a156-4df9-8871-5187cf8822af" />
