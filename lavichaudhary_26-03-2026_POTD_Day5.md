#PRODUCT OF ARRAY EXCEPT SELF 
class Solution:
    def productExceptSelf(self, nums: list[int]) -> list[int]:
        length = len(nums)
        answer = [1] * length
         prefix_product = 1
        for i in range(length):
            answer[i] = prefix_product
            prefix_product *= nums[i]
             suffix_product = 1
        for i in range(length - 1, -1, -1):
            answer[i] *= suffix_product
            suffix_product *= nums[i]
                return answer

<img width="1919" height="968" alt="Screenshot 2026-03-26 DAY 5" src="https://github.com/user-attachments/assets/f0476e05-275f-4fb2-95bc-7446f56701ca" />
