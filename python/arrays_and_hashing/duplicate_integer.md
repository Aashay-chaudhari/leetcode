class Solution:
    def hasDuplicate(self, nums: List[int]) -> bool:
         return len(nums) != len(set(nums))


In the above function, we are converting the given nums list to a set first. 
This introduces O(n) time complexity in our function, as the list is converted
into a set using hashing (unique items). So, it takes n iterations to complete 
the conversion. The space complexity is also O(n) as we are storing the n item
list temporarily. 

Space complexity : O(n)
Time complexity : O(n)
