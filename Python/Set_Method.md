Date: 11-30-23
# What does the `set()` method do?
`set()` is used to make a "set" of unique sorted data. Unique means that it removes duplicates, so there is only one of each element. It could be placed on `lists`, `tuples`, and `dictionaries`. This function works with all data types. If the data is a `int` or `float`, it would sort it in ascending order.

# How to use
**Code:**
```python
intlist = [1, 5, 2, 2, 5, 7, 8, 100]
floatlist = [5.5, 1.2, 1.1, 5, 89, 100.1]
stringlist = ["hi", "hello", "hi", "How"]

# you can use other formats like dictionary or tuple.

print('Int set: ', set(intlist))
print("float set: ", set(floatlist))
print("string set: ", set(stringlist))
```
**Output:**
```
('Int set: ', set([1, 2, 5, 7, 8, 100]))
('float set: ', set([1.2, 1.1, 5.5, 5, 89, 100.1]))
('string set: ', set(['hi', 'hello', 'How']))
```
