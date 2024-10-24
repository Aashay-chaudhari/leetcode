

class Solution:
    def isAnagram(self, s: str, t: str) -> bool:
        if len(s) != len(t):
            return false

        s_dict = {}
        t_dict = {}

        for char in s:
            if char in s_dict.keys():
                s_dict[char] += 1
            else:
                s_dict[char] = 1


        for char in t:
            if char in t_dict.keys():
                t_dict[char] += 1
            else:
                t_dict[char] = 1

        print("s_dict: ", s_dict)
        print("t_dict: ", t_dict)

        return s_dict == t_dict


Space complexity : Creating 2 dictionaries = O(2n) == O(n)

Time complexity : Creating 2 dictionaries + comparing dicts = O(2n + 1) = O(n)

