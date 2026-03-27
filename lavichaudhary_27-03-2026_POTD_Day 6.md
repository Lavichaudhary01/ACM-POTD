#Check If N and Its Double Exist
class Solution:
    def checkIfExist(self, arr: list[int]) -> bool:
        arr.sort()
        n = len(arr)
        for i in range(n):
            target = 2 * arr[i]
            low, high = 0, n - 1
            while low <= high:
                mid = (low + high) // 2
                if arr[mid] == target and mid != i:
                    return True
                if arr[mid] < target:
                    low = mid + 1
                else:
                    high = mid - 1
        return False
        
<img width="1916" height="968" alt="Screenshot 2026-03-27 DAY 6" src="https://github.com/user-attachments/assets/75051c25-6613-4802-bc87-d2817fd8169b" />
