#Here is the python code for removing duplicates from sorted array
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
arr = [1,1,2]
k = sol.removeDuplicates(arr)
print(f"The unique array is: {arr[:k]}")


###Execution Result
###Screenshot of output <img width="1913" height="1035" alt="Screenshot 2026-03-22 031555" src="https://github.com/user-attachments/assets/908fc3b6-66f4-4467-aa7b-802ee60ffb78" />
