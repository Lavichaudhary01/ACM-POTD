# Invert Binary Tree
class Solution:
    def invertTree(self, root: Optional[TreeNode]) -> Optional[TreeNode]:
        if not root:
            return None
        root.left, root.right = root.right, root.left
        self.invertTree(root.left)
        self.invertTree(root.right)
        return root


  <img width="1918" height="971" alt="image" src="https://github.com/user-attachments/assets/7988b949-bbe1-47ba-9e0e-f8e859a24e7d" />
