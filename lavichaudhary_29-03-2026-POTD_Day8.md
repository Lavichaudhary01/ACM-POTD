#Reverse Linked List
class Solution:
    def reverseList(self, head):
        prev = None
        curr = head
        while curr:
            nxt = curr.next  
            curr.next = prev 
            prev = curr      
            curr = nxt         
        return prev 

  <img width="1919" height="973" alt="Screenshot 2026-03-29 232315" src="https://github.com/user-attachments/assets/4be77f78-77aa-4b75-9700-f30f57bb0bbc" />
