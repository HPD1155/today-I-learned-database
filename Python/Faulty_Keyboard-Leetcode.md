Date: 12-4-23
# Leetcode Problem #1: [2810.  Faulty Keyboard](https://leetcode.com/problems/faulty-keyboard/)
## Code:
```python
class  Solution:
	def  finalString(self, s: str) -> str:
		str1=""
		for i in s:
			if i=="i":
				str1=str1[::-1]
			else:
				str1+=i
		return str1
```

We will first make a variable called `str1` which will hold the modified string. We will iterate through the `s` string which is unmodified. We will check if `i` or the position in the string is "i". If it is then we will flip the modified string `str1`. We will use `[::-1]`. If the character is not "i", then we will add the new character to the modified `str1` variable. After it is done iterating, we will return `str1`.
