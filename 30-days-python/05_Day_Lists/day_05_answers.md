### Exercises: Level 1

1. Declare an empty list
```
empty_list = list()
```
2. Declare a list with more than 5 items

```
vegetables = ['Tomato', 'Potato', 'Cabbage','Onion', 'Carrot', 'grape'] 
```
3. Find the length of your list

```
len(vegetables)
```
4. Get the first item, the middle item and the last item of the list

```
>>> print(vegetables[0]) 
Tomato
>>> print(vegetables[(len(vegetables)-1)]) 
grape
```
5. Declare a list called mixed_data_types, put your(name, age, height, marital status, address)

```
mixed_data_types = ['sujimatts',25,6.0,'single']
```
6. Declare a list variable named it_companies and assign initial values Facebook, Google, Microsoft, Apple, IBM, Oracle and Amazon.

```
it_companies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Oracle', 'Amazon']
```
7. Print the list using _print()_

```
```
8. Print the number of companies in the list

```
len(it_companies)
```
9. Print the first, middle and last company

```
```
10. Print the list after modifying one of the companies

```
>>> it_companies = ['Facebook', 'Google', 'Microsoft', 'Apple', 'IBM', 'Oracle', 'Amazon']
>>> it_companies[1] = 'Twitter' 
>>> print(it_companies)                                                                                          
['Facebook', 'Twitter', 'Microsoft', 'Apple', 'IBM', 'Oracle', 'Amazon']

```
11. Add an IT company to it_companies

```
>>> it_companies.append('Google')            
```
12. Insert an IT company in the middle of the companies list

```
>>> it_companies.insert(2, 'ABC')            
```
13. Change one of the it_companies names to uppercase (IBM excluded!)

```
```
14. Join the it_companies with a string '#;&nbsp; '

```
```
15. Check if a certain company exists in the it_companies list.

```
print('XYZ' in it_companies)
```
16. Sort the list using sort() method

```
>>> it_companies.sort()        
>>> print(it_companies)
```
17. Reverse the list in descending order using reverse() method

```
>>> it_companies.sort(reverse=True)        
>>> print(it_companies)
```
18. Slice out the first 3 companies from the list

```
it_companies[3:] 
```
19. Slice out the last 3 companies from the list

```
>>> it_companies[:-3]  
```
20. Slice out the middle IT company or companies from the list

```
```
21. Remove the first IT company from the list

```
>>> it_companies.pop(0) 
```
22. Remove the middle IT company or companies from the list

```
```
23. Remove the last IT company from the list

```
>>> it_companies.pop(0) 
```
24. Remove all IT companies from the list

```
it_companies.clear()
```
25. Destroy the IT companies list

```
del it_companies
```
26. Join the following lists:

    ```py
    front_end = ['HTML', 'CSS', 'JS', 'React', 'Redux']
    back_end = ['Node','Express', 'MongoDB']
    ```
    ```
    product = front_end + back_end
    ```

27. After joining the lists in question 26. Copy the joined list and assign it to a variable full_stack. Then insert Python and SQL after Redux.

```
full_stack = product.copy()
full_stack.insert(3,'AAA')
```

### Exercises: Level 2

1. The following is a list of 10 students ages:

```sh
ages = [19, 22, 19, 24, 20, 25, 26, 24, 25, 24]
```

- Sort the list and find the min and max age
```
>>> ages.sort()
>>> min(ages) 
19
>>> max(ages) 
26
```
- Add the min age and the max age again to the list
```
>>> ages.append(min(ages)) 
>>> ages.append(max(ages)) 
```
- Find the median age (one middle item or two middle items divided by two)
```
>>> middle = int(len(ages) / 2)
>>> print(ages[middle]) 
24
```
- Find the average age (sum of all items divided by their number )
```
>>> sum(ages) 
>>> sum(ages) / len(ages)
```
- Find the range of the ages (max minus min)
```
>>> for i in range(min(ages),max(ages)):   
...  print(i)
... 
19
20
21
22
23
24
25
>>
```

