# Backspace String Compare
class Solution:
    def backspaceCompare(self, s: str, t: str) -> bool:
        def build(string):
            stack = []
            for char in string:
                if char != '#':
                    stack.append(char)
                elif stack:
                    stack.pop()
            return "".join(stack)
        return build(s) == build(t)



<img width="1897" height="911" alt="image" src="https://github.com/user-attachments/assets/78ae608c-ca85-4002-85cb-2cf3eefa3ec0" />
