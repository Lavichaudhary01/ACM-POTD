# Remove Outermost Parentheses
class Solution:
    def removeOuterParentheses(self, s: str) -> str:
        res = []
        opened = 0
        for char in s:
            if char == '(':
                if opened > 0:
                    res.append(char)
                opened += 1
            else:
                opened -= 1
                if opened > 0:
                    res.append(char)          
        return "".join(res)


  <img width="1905" height="910" alt="image" src="https://github.com/user-attachments/assets/3f1493ac-a165-4c1d-81f5-cff323b162ce" />
