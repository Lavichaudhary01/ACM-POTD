#two sum
class Solution:
    def twoSum(self, numbers: list[int], target: int) -> list[int]:
        left = 0
        right = len(numbers) - 1
        while left < right:
            current_sum = numbers[left] + numbers[right]
            if current_sum == target:
                return [left + 1, right + 1]
           elif current_sum < target:
                left += 1
            else:
                right -= 1
        return []

<img width="1908" height="963" alt="Screenshot 2026-03-25 DAY 4" src="https://github.com/user-attachments/assets/18811544-d793-4cad-8355-8cdb2504c4f8" />
