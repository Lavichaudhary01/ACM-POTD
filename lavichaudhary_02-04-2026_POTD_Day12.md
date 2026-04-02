# Remove Duplicates from Sorted List
class Solution:
    def deleteDuplicates(self, head: Optional[ListNode]) -> Optional[ListNode]:
        curr = head
        while curr and curr.next:
            if curr.val == curr.next.val:
                curr.next = curr.next.next
            else:
                curr = curr.next            
        return head
<img width="1919" height="967" alt="Screenshot 2026-04-02 153400" src="https://github.com/user-attachments/assets/713d868e-9c0e-491b-86d3-145654f02f91" />
