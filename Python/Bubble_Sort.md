Date: 11-28-2023
Topic: Bubble Sort

# What is Bubble Sort?
Bubble Sort is a sorting algorithm typically used in arrays to sort data. It does it by comparing two numbers in sets, and it checks if they are in order or first number is less than the second. It iterates this a certain amount of times till the array is sorted. The reason it is called **Bubble Sort** is because essentially, the largest number "bubbles" to the top or end of the array.
# How it works
The algorithm goes in order in an increment of 1 number at a time and checks if the current number and the number after it are in order (In this case, the first number should be less than the second number). If they aren't, then the algorithm *swaps* the two. It then moves up by one and compares the current number to the number in front of it. It repeats this until the end of the array. Then depending on how many possible sort combinations there are, it will repeat itself that many times. You can calculate that by `N` being the length of the array and `N-1` being the possible combinations.

# Example
Say for example you have a array of `[5, 4, 8, 6, 2]`. We can mark possible combinations as this variable: `comb = len(arr) - 1`.
Now we are going to iterate the array that many times using `for i in range(comb):`.  Next we are going to move forward by the array elements by `comb` amount. We can use `for j in range(comb):`.
Using `if  arr[j]  >  arr[j  +  1]:` we can check if the current value is greater than the value after. If it is, we can swap it using `arr[j], arr[j+1] = arr[j+1], arr[j]`.
After it has iterated `comb` many times through the list, we can return the sorted array like `return arr`.

Full code:
```python
def  BubbleSort(arr):
	comb  =  len(arr)  -  1
	for  i  in  range(comb):
		for  j  in  range(comb)
			if  arr[j]  >  arr[j  +  1]:
				arr[j],  arr[j  +  1]  =  arr[j  +  1],  arr[j]
	return  arr

  

if  __name__  ==  '__main__':
	arr  =  [5, 4, 8, 6, 2]
	print(BubbleSort(arr))
```
