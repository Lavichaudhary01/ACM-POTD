#Swap Nodes in Pairs
class Solution:
    def swapPairs(self, head: Optional[ListNode]) -> Optional[ListNode]:
      if not head or not head.next:
            return head
        first = head
        second = head.next
        first.next = self.swapPairs(second.next)
        second.next = first
        return second
        

<img width="1919" height="972" alt="Screenshot 2026-04-04 214616" src="https://github.com/user-attachments/assets/66722693-7544-4855-a955-13c7ddd0292f" />
