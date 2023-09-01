class Solution(object):
    def nextPermutation(self, nums):
        """
        :type nums: List[int]
        :rtype: None Do not return anything, modify nums in-place instead.
        """
        n = len(nums)
        if n == 1:
            return
        for i in range(n-1, -1, -1):
            if nums[i] > nums[i-1]:
                break
        if i != 0:
            for j in range(n-1, -1, -1):
                if nums[j] > nums[i-1]:
                    break
            nums[i-1], nums[j] = nums[j], nums[i-1] 
        nums[i:]=reversed(nums[i:]) 
