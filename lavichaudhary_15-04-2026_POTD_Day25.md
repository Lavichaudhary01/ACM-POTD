# Maximum Depth of Binary Tree
class Solution:
    def maxDepth(self, root: Optional[TreeNode]) -> int:
        if not root:
            return 0
        left_side = self.maxDepth(root.left)
        right_side = self.maxDepth(root.right)
        return max(left_side, right_side) + 1

  <img width="1919" height="969" alt="image" src="https://github.com/user-attachments/assets/1e1f529c-ba9c-40b3-8a8b-b6e546acfd6c" />
