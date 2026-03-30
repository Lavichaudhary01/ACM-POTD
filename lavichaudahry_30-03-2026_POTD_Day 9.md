#Linked list cycle
class Solution:
    def hasCycle(self, head: Optional[ListNode]) -> bool:
        visited = set()
        curr = head
        while curr:
            if curr in visited:
                return True
            visited.add(curr)
            curr = curr.next
        return False

<img width="1919" height="964" alt="Screenshot 2026-03-30 232024" src="https://github.com/user-attachments/assets/b45da90d-84a1-46af-a238-8bc9d4e9aed7" />
