class Solution:
    def removeDuplicates(self, nums: list[int]) -> int:
        if not nums:
            return 0
        insert_index = 1
        for i in range(1, len(nums)):
            if nums[i] != nums[i - 1]:
                nums[insert_index] = nums[i]
                insert_index += 1
        return insert_index
sol = Solution()
arr= [ 1, 1, 2]
k = sol.removeDuplicates(arr)
print(f"The unique array is: {arr[:k]}")
