# Intersection of Two Linked Lists
class Solution:
    def getIntersectionNode(self, headA: ListNode, headB: ListNode) -> Optional[ListNode]:
        a, b = headA, headB
        while a != b:
            a = a.next if a else headB
            b = b.next if b else headA
        return a
        
<img width="1919" height="966" alt="Screenshot 2026-04-03 035545" src="https://github.com/user-attachments/assets/ec9f37ef-be2e-4fdb-8eab-1ab802e17522" />

