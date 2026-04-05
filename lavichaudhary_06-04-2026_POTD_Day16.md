# Implement Queue using Stacks
class MyQueue:
    def __init__(self):
        self.s1 = [] 
        self.s2 = [] 
    def push(self, x: int) -> None:
        self.s1.append(x)
    def pop(self) -> int:
        self.peek()
        return self.s2.pop()
    def peek(self) -> int:
        if not self.s2:
            while self.s1:
                self.s2.append(self.s1.pop())
        return self.s2[-1]
    def empty(self) -> bool:
        return not self.s1 and not self.s2

<img width="1919" height="970" alt="Screenshot 2026-04-06 022320" src="https://github.com/user-attachments/assets/5cd58396-6a69-4c55-a0a5-4e492806ae74" />
