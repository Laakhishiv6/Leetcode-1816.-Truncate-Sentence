# Leetcode-1816.-Truncate-Sentence

# Description
A sentence is a list of words that are separated by a single space with no leading or trailing spaces. Each of the words consists of only uppercase and lowercase English letters (no punctuation).

For example, "Hello World", "HELLO", and "hello world hello world" are all sentences.
You are given a sentence s​​​​​​ and an integer k​​​​​​. You want to truncate s​​​​​​ such that it contains only the first k​​​​​​ words. Return s​​​​​​ after truncating it.

# Solution
In the given problem we need to truncate a given sentence , in such a way that it should contain only the first k numbers if words.

For Example :

s= "Hello how are you Contestant", k = 4

Use s.split() to convert the string to array 

["Hello", "how" "are", "you", "Contestant"]

Now slice the array till k elements : ["Hello", "how" "are", "you"]

Lets join the array back to a sentence by using ' '.join() : "Hello how are you"

Hence , the final sentence is "Hello how are you"

# Algorithm

1. Use split() function to to divide a string into a list of substrings.
2. The Slice the array tillk number of elements.
3. Now , for the final result we need to join back the elements.
4. join()  method is a string method used to concatenate elements.
5. Return the truncated sentence.
# Code

class Solution:

    def truncateSentence(self, s: str, k: int) -> str:
        words=s.split()
        first_k_words=words[:k]
        truncated='4 '.join(first_k_words)
        return truncated

# Complexity analysis

Time complexity : O(n)
