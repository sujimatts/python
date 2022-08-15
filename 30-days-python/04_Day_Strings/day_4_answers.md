1.	Concatenate the string 'Thirty', 'Days', 'Of', 'Python' to a single string, 'Thirty Days Of Python'.
```
string =  ['Thirty', 'Days', 'Of', 'Python']
print (' '.join(string))
```
2.	Concatenate the string 'Coding', 'For' , 'All' to a single string, 'Coding For All'.
```
string =  ['Coding', 'For' , 'All']
print (' '.join(string))
```
3.	Declare a variable named company and assign it to an initial value "Coding For All".
```
company = "Coding For All"
```
4.	Print the variable company using print().
```
print(company)
```
5.	Print the length of the company string using len() method and print().
```
print(len(company))
```
6.	Change all the characters to uppercase letters using upper() method.
```
print(company.upper())
```
7.	Change all the characters to lowercase letters using lower() method.
```
print(company.lower())
```
8.	Use capitalize(), title(), swapcase() methods to format the value of the string Coding For All.
```
print(company.capitalize())
print(company.title())
print(company.swapcase())

```
9.	Cut(slice) out the first word of Coding For All string.
```
print(company[6:]) 
```
10.	Check if Coding For All string contains a word Coding using the method index, find or other methods.
```
print(company.find('Coding')) 
```
11.	Replace the word coding in the string 'Coding For All' to Python.
```
print(company.replace('Coding', 'Python'))
```
12.	Change Python for Everyone to Python for All using the replace method or other methods.
```
print(company.replace('all', 'everyone'))
```
13.	Split the string 'Coding For All' using space as the separator (split()) .
```
print(company.split())
```
14.	"Facebook, Google, Microsoft, Apple, IBM, Oracle, Amazon" split the string at the comma.
```
print("Facebook, Google, Microsoft, Apple, IBM, Oracle, Amazon".split(',')) 
```
16.	What is the character at index 0 in the string Coding For All.
17.	
```
print(company[0])
```
18.	What is the last index of the string Coding For All.
```
print(company[-1])
```
19.	What character is at index 10 in "Coding For All" string.
```
print(company[10])
```
20.	Create an acronym or an abbreviation for the name 'Python For Everyone'.
```
string = 'Python For Everyone'
print(''.join(i[0] for i in string.split()))
```
21.	Create an acronym or an abbreviation for the name 'Coding For All'.
```
string = 'Coding For All
print(''.join(i[0] for i in string.split()))
```
22.	Use index to determine the position of the first occurrence of C in Coding For All.
```
string = 'Coding For All'
to_find = 'C'
print(string.index(to_find)) 
```
23.	Use index to determine the position of the first occurrence of F in Coding For All.
```
string = 'Coding For All'
to_find = 'F'
print(string.index(to_find)) 
```
24.	Use rfind to determine the position of the last occurrence of l in Coding For All People.
```
string = 'Coding For All People'
to_find = 'l'
print(string.rfind(to_find)) 

```
25.	Use index or find to find the position of the first occurrence of the word 'because' in the following sentence: 'You cannot end a sentence with because because because is a conjunction'
```
string = 'You cannot end a sentence with because because because is a conjunction'
to_find = 'because'
print(string.index(to_find)) 

```
26.	Use rindex to find the position of the last occurrence of the word because in the following sentence: 'You cannot end a sentence with because because because is a conjunction'
```
string = 'You cannot end a sentence with because because because is a conjunction'
to_find = 'because'
print(string.rindex(to_find)) 
```
27.	Slice out the phrase 'because because because' in the following sentence: 'You cannot end a sentence with because because because is a conjunction'
```
string = 'You cannot end a sentence with because because because is a conjunction'
to_delete = 'because'
print(string.replace(to_delete, '')) 
```
28. Does 'Coding For All' end with a substring coding? 
```
string = 'Coding For All'
to_find = 'coding'
print(string.endswith(to_find)) 
```
29. '   Coding For All      '  , remove the left and right trailing spaces in the given string.
```
string = '   Coding For All      '
print(string.strip())
```
30. Which one of the following variables return True when we use the method isidentifier():
30DaysOfPython
thirty_days_of_python
```
string = '30DaysOfPython'
print(string.isidentifier())
>> False

string = 'thirty_days_of_python'
print(string.isidentifier())
>> True
```

31. The following list contains the names of some of python libraries: ['Django', 'Flask', 'Bottle', 'Pyramid', 'Falcon']. Join the list with a hash with space string.
```
library = ['Django', 'Flask', 'Bottle', 'Pyramid', 'Falcon']
print('# '.join(library)
```
32. Use the new line escape sequence to separate the following sentences.
I am enjoying this challenge.
I just wonder what is next.
```
print('I am enjoying this challenge. \nI just wonder what is next.') 
```
33. Use a tab escape sequence to write the following lines.
Name      Age     Country   City
Asabeneh  250     Finland   Helsinki
```
print('Name\tAge\tCountry\tCity\nAsabeneh\t250\tFinland\tHelsinki')
```
34. Use the string formatting method to display the following:
radius = 10
area = 3.14 * radius ** 2
The area of a circle with radius 10 is 314 meters square.
35. Make the following using string formatting methods:
8 + 6 = 14
8 - 6 = 2
8 * 6 = 48
8 / 6 = 1.33
8 % 6 = 2
8 // 6 = 1
8 ** 6 = 262144
```
```
