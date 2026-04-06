# Implement Stack using Queues

class MyStack:
    def __init__(self):
        self.q = deque()
    def push(self, x: int) -> None:
        self.q.append(x)
        for _ in range(len(self.q) - 1):
            self.q.append(self.q.popleft())
    def pop(self) -> int:
        return self.q.popleft()
    def top(self) -> int:
        return self.q[0]
    def empty(self) -> bool:
        return not self.q

 <img width="1917" height="972" alt="Screenshot 2026-04-07 003530" src="https://github.com/user-attachments/assets/8e6251fa-10ed-490f-9f74-9c32b18844ab" />

