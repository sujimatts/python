getting inputs
  first_name = input('What is your name: ')
  age = input('How old are you? ')

operators
  print('a + b = ', total)
  print('a - b = ', diff)
  print('a * b = ', product)
  print('a / b = ', division)
  print('a % b = ', remainder)
  print('a // b = ', floor_division)
  print('a ** b = ', exponentiation)

  1 1 1 1 1
  2 1 2 4 8
  3 1 3 9 27
  4 1 4 16 64
  5 1 5 25 125

  n = 1
  while n <= 5:
      print(n, n ** 0, n ** 1, n ** 2, n ** 3)
      n += 1

  string formatting
  (old_method) formated_string = 'I am %s %s. I teach %s' %(first_name, last_name, language)
  (new_method) formated_string = 'I am {} {}. I teach {}'.format(first_name, last_name, language)

  language = 'Python'
  last_letter = language[-1]
  print(last_letter) # n

  print(language.capitalize()) 

lists
  fruits = ['banana', 'orange', 'mango', 'lemon']
  ing item ina list : fruits[0] = 'avocado'
  Checking Items in a List: 'banana' in fruits
  Slicing Items from a List: all_fruits = fruits[0:4] 
  Adding Items to a List : fruits.append('apple')
  Inserting Items into a List: fruits.insert(2, 'apple')
  Removing Items from a List: fruits.remove('banana')
  Removing Items Using Pop : fruits.pop(0)
  Removing Items Using Del : del fruits[0]
                              del fruits[1:3]
  Clearing List Items : fruits.clear()
  Copying a List : fruits_copy = fruits.copy()
  Joining Lists: list3 = list1 + list2
  Counting Items in a List: print(fruits.count('orange'))  
  Finding Index of an Item: print(fruits.index('orange')) 
  Reversing a List: fruits.reverse()
  Sorting List Items: fruits.sort(reverse=True)
                      fruits.sort()

Tuples
  create tuple: empty_tuple = tuple() or ()
  fruits = ('banana', 'orange', 'mango', 'lemon')
  accessing item:  fruits[0]
  Slicing tuples: fruits[0:4] 
  Changing Tuples to Lists: fruits = list(fruits)
  Checking an Item in a Tuple: print('orange' in fruits) # True
  Joining Tuples: Joining Tuples
  Deleting Tuples: del fruits

Sets
  create a set: st = set()
  fruits = {'banana', 'orange', 'mango', 'lemon'}
  Accessing Items in a Set: print('mango' in fruits ) # True
  Adding Items to a Set: fruits.add('lime')
  Removing Items from a Set: fruits.remove('banana')
  Clearing Items in a Set: fruits.clear()
  Deleting a Set: fruits.clear()
  Converting List to Set: Converting List to Set
  Joining Sets: st1.update(st2)

Dictionaries
  Creating a Dictionary: dct = {'key1':'value1', 'key2':'value2', 'key3':'value3', 'key4':'value4'}

          person = {
            'first_name':'Asabeneh',
            'last_name':'Yetayeh',
            'age':250,
            'country':'Finland',
            'is_marred':True,
            'skills':['JavaScript', 'React', 'Node', 'MongoDB', 'Python'],
            'address':{
                'street':'Space street',
                'zipcode':'02210'
            }
            }

    Accessing Dictionary Items: print(person['first_name']) # Asabeneh
                                  print(person['skills'][0])  # JavaScript
    Adding Items to a Dictionary: person['job_title'] = 'Instructor'
    Modifying Items in a Dictionary: person['first_name'] = 'Eyob'
    Checking Keys in a Dictionary: print('key5' in person) # False
    Removing Key and Value Pairs from a Dictionary: person.pop('first_name')        # Removes the firstname item
    Changing Dictionary to a List of Items: dct.clear()
    Deleting a Dictionary: del dct
    Copy a Dictionary: dct.copy()
    Getting Dictionary Keys as a List: keys = dct.keys()
    Getting Dictionary Values as a List: values = dct.values()

Conditionals
    If Condition
        a = 3
        if a > 0:
            print('A is a positive number')
        # A is a positive number

    If Else
      a = 3
      if a < 0:
          print('A is a negative number')
      else:
          print('A is a positive number')

    If Elif Else
      a = 0
      if a > 0:
          print('A is a positive number')
      elif a < 0:
          print('A is a negative number')
      else:
          print('A is zero')

    Short Hand
      a = 3
      print('A is positive') if a > 0 else print('A is negative') # first condition met, 'A is positive' will be printed

    Nested Conditions
      if condition:
          code
          if condition:
          code

    If Condition and Logical Operators
      a = 0
      if a > 0 and a % 2 == 0:
              print('A is an even and positive integer')
      elif a > 0 and a % 2 !=  0:
          print('A is a positive integer')
      elif a == 0:
          print('A is zero')
      else:
          print('A is negative')

    If and Or Logical Operators
      user = 'James'
      access_level = 3
      if user == 'admin' or access_level >= 4:
              print('Access granted!')
      else:
          print('Access denied!')


Loops
  While Loop
      count = 0
      while count < 5:
          print(count)
          count = count + 1
      #prints from 0 to 4

  Break and Continue - Part 1
      count = 0
      while count < 5:
          print(count)
          count = count + 1
          if count == 3:   #The above while loop only prints 0, 1, 2, but when it reaches 3 it stops.
              break

      count = 0
      while count < 5:
          if count == 3:
              continue
          print(count)
          count = count + 1   # The above while loop only prints 0, 1, 2 and 4 (skips 3).

  For Loop
      numbers = [0, 1, 2, 3, 4, 5]
      for number in numbers: # number is temporary name to refer to the list's items, valid only inside this loop
          print(number)       # the numbers will be printed line by line, from 0 to 5

  The Range Function
      for number in range(11):
      print(number)   # prints 0 to 10, not including 11

  ### DO THE EXERCISES https://github.com/sujimatts/python/blob/main/30-days-python/10_Day_Loops/10_loops.md


Functions
  Declaring and Calling a Function
            def add_two_numbers ():
                num_one = 2
                num_two = 3
                total = num_one + num_two
                print(total)
            add_two_numbers()
        
  Function Returning a Value - Part 1
          def generate_full_name ():
              first_name = 'Asabeneh'
              last_name = 'Yetayeh'
              space = ' '
              full_name = first_name + space + last_name
              return full_name
          print(generate_full_name())

  Function with Parameters
          def greetings (name):
              message = name + ', welcome to Python for Everyone!'
              return message

          print(greetings('Asabeneh'))


          def add_ten(num):
              ten = 10
              return num + ten
          print(add_ten(90))


  Passing Arguments with Key and Value
          def add_two_numbers (num1, num2):
              total = num1 + num2
              print(total)
          print(add_two_numbers(num2 = 3, num1 = 2)) # Order does not matter

  Function with Default Parameters
          def greetings (name = 'Peter'):
              message = name + ', welcome to Python for Everyone!'
              return message
          print(greetings())
          print(greetings('Asabeneh'))

Modules
    Creating a Module
        # mymodule.py file
        def generate_full_name(firstname, lastname):
            return firstname + ' ' + lastname

    Importing a Module
        # main.py file
        import mymodule
        print(mymodule.generate_full_name('Asabeneh', 'Yetayeh')) # Asabeneh Yetayeh

    OS Module
        # import the module
        import os
        # Creating a directory
        os.mkdir('directory_name')
        # Changing the current directory
        os.chdir('path')
        # Getting current working directory
        os.getcwd()
        # Removing directory
        os.rmdir()

    Sys Module
        import sys
        #print(sys.argv[0], argv[1],sys.argv[2])  # this line would print out: filename argument1 argument2
        print('Welcome {}. Enjoy  {} challenge!'.format(sys.argv[1], sys.argv[2]))

        # to exit sys
        sys.exit()
        # To know the largest integer variable it takes
        sys.maxsize
        # To know environment path
        sys.path
        # To know the version of python you are using
        sys.version

    Statistics Module
        from statistics import * # importing all the statistics modules
        ages = [20, 20, 4, 24, 25, 22, 26, 20, 23, 22, 26]
        print(mean(ages))       # ~22.9
        print(median(ages))     # 23
        print(mode(ages))       # 20
        print(stdev(ages))      # ~2.3
    Math Module
        import math
        print(math.pi)           # 3.141592653589793, pi constant
        print(math.sqrt(2))      # 1.4142135623730951, square root
        print(math.pow(2, 3))    # 8.0, exponential function
        print(math.floor(9.81))  # 9, rounding to the lowest
        print(math.ceil(9.81))   # 10, rounding to the highest
        print(math.log10(100))   # 2, logarithm with 10 as base
    
    String Module
        import string
        print(string.ascii_letters) # abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ
        print(string.digits)        # 0123456789
        print(string.punctuation)   # !"#$%&'()*+,-./:;<=>?@[\]^_`{|}~

    Random Module
        from random import random, randint
        print(random())   # it doesn't take any arguments; it returns a value between 0 and 0.9999
        print(randint(5, 20)) # it returns a random integer number between [5, 20] inclusive

Error Types

      SyntaxError: 
      NameError:  name 'age' is not defined
      IndexError:  list index out of range [ACCESSING NOT EXISTING INDEX]
      ModuleNotFoundError: No module named 'maths'
      AttributeError: module 'math' has no attribute 'PI'
      KeyError: KeyError: 'county' [NO SUCH KEY]
      TypeError: unsupported operand type(s) for +: 'int' and 'str' [SUM OF INT AND STRING]
      ImportError: cannot import name 'power' from 'math'
      ValueError: invalid literal for int() with base 10: '12a'
      ZeroDivisionError:  division by zero

datetime

      import datetime
      print(dir(datetime))

      from datetime import datetime
      now = datetime.now()
      print(now)                      # 2021-07-08 07:34:46.549883
      day = now.day                   # 8
      month = now.month               # 7
      year = now.year                 # 2021
      hour = now.hour                 # 7
      minute = now.minute             # 38
      second = now.second
      timestamp = now.timestamp()
      print(day, month, year, hour, minute)
      print('timestamp', timestamp)
      print(f'{day}/{month}/{year}, {hour}:{minute}')  # 8/7/2021, 7:38

Exception Handling
      try:
          print(10 + '5')
      except:
          print('Something went wrong')



      try:
          name = input('Enter your name:')
          year_born = input('Year you born:')
          age = 2019 - int(year_born)
          print('You are {name}. And your age is {age}.')
      except TypeError:
          print('Type error occur')
      except ValueError:
          print('Value error occur')
      except ZeroDivisionError:
          print('zero division error occur')
      else:
          print('I usually run with the try block')
      finally:
          print('I alway run.')

    
    Enumerate (to get the index of each item in the list.)
        
        for index, item in enumerate([20, 30, 40]):
        print(index, item)

    Zip    #combine lists when looping through them

        fruits = ['banana', 'orange', 'mango', 'lemon', 'lime']                    
        vegetables = ['Tomato', 'Potato', 'Cabbage','Onion', 'Carrot']
        fruits_and_veges = []
        for f, v in zip(fruits, vegetables):
            fruits_and_veges.append({'fruit':f, 'veg':v})

        print(fruits_and_veges)

Regular Expressions

      import re
      re.match(): searches only in the beginning of the first line of the string and returns matched objects if found, else returns None.
      re.search: Returns a match object if there is one anywhere in the string, including multiline strings.
      re.findall: Returns a list containing all matches
      re.split: Takes a string, splits it at the match points, returns a list
      re.sub: Replaces one or many matches within a string

      txt = 'I love to teach python and javaScript'
      match: match = re.match('I love to teach', txt, re.I)
      matches = re.findall('language', txt, re.I)
      match_replaced = re.sub('Python|python', 'JavaScript', txt, re.I)
      print(re.split('\n', txt)) # splitting using \n - end of line symbol [it will become a list]


File Handling
      "r" - Read - Default value. Opens a file for reading, it returns an error if the file does not exist
      "a" - Append - Opens a file for appending, creates the file if it does not exist
      "w" - Write - Opens a file for writing, creates the file if it does not exist
      "x" - Create - Creates the specified file, returns an error if the file exists
      "t" - Text - Default value. Text mode
      "b" - Binary - Binary mode (e.g. images)

  open & with open
      f = open('./files/reading_file_example.txt')
      txt = f.read()
      print(type(txt))
      print(txt)
      f.close()

      with open('./files/reading_file_example.txt') as f:
          lines = f.read().splitlines()
          print(type(lines))
          print(lines)

  read_modes

      f = open('./files/reading_file_example.txt')
      txt = f.read()  # read the whole text as string
      txt = f.read(10) # first 10 characters of the text file.
      f.readline() # read only the first line
      f.readlines() # read all the text line by line and returns a list of lines [as a list]
      f.read().splitlines() # Another way to get all the lines as a list is 

  updating file 
      with open('./files/reading_file_example.txt','a') as f:
          f.write('This text has to be appended at the end')
  Deleting Files
      import os
      if os.path.exists('./files/example.txt'):
          os.remove('./files/example.txt')
      else:
          print('The file does not exist')

  Changing JSON to Dictionary
      person_dct = json.loads(person_json)

  Changing Dictionary to JSON
      person_json = json.dumps(person, indent=4) # indent could be 2, 4, 8. It beautifies the json

  Saving as JSON File
      import json
      # python dictionary
      person = {
          "name": "Asabeneh",
          "country": "Finland",
          "city": "Helsinki",
          "skills": ["JavaScrip", "React", "Python"]
      }
      with open('./files/json_example.json', 'w', encoding='utf-8') as f:
          json.dump(person, f, ensure_ascii=False, indent=4)

  File with csv Extension
        import csv
        with open('./files/csv_example.csv') as f:
            csv_reader = csv.reader(f, delimiter=',') # w use, reader method to read csv
            line_count = 0
            for row in csv_reader:
                if line_count == 0:
                    print(f'Column names are :{", ".join(row)}')
                    line_count += 1
                else:
                    print(
                        f'\t{row[0]} is a teachers. He lives in {row[1]}, {row[2]}.')
                    line_count += 1
            print(f'Number of lines:  {line_count}')

  File with xlsx Extension
        import xlrd
        excel_book = xlrd.open_workbook('sample.xls)
        print(excel_book.nsheets)
        print(excel_book.sheet_names)

Web browser 
      import webbrowser 
      url_lists = [
          'http://www.python.org',
          'https://www.linkedin.com/in/asabeneh/',
          'https://github.com/Asabeneh',
          'https://twitter.com/Asabeneh',
      ]
      # opens the above list of websites in a different tab
      for url in url_lists:
          webbrowser.open_new_tab(url)

request_module
      get(): to open a network and fetch data from url - it returns a response object
      status_code: After we fetched data, we can check the status of the operation (success, error, etc)
      headers: To check the header types
      text: to extract the text from the fetched response object
      json: to extract json data Let's read a txt file from this website, https://www.w3.org/TR/PNG/iso_8859-1.txt.



      import requests
      url = 'https://restcountries.eu/rest/v2/all'  # countries api
      response = requests.get(url)  # opening a network and fetching a data
      print(response) # response object
      print(response.status_code)  # status code, success:200
      countries = response.json()
      print(countries[:1])  # we sliced only the first country, remove the slicing to see all countries

Web Scraping
    #To start scraping websites you need requests, beautifoulSoup4 and a website.

      import requests
      from bs4 import BeautifulSoup
      url = 'https://archive.ics.uci.edu/ml/datasets.php'

      response = requests.get(url)
      content = response.content # we get all the content from the website
      soup = BeautifulSoup(content, 'html.parser') # beautiful soup will give a chance to parse
      print(soup.title) # <title>UCI Machine Learning Repository: Data Sets</title>
      print(soup.title.get_text()) # UCI Machine Learning Repository: Data Sets
      print(soup.body) # gives the whole page on the website
      print(response.status_code)

      tables = soup.find_all('table', {'cellpadding':'3'})
      # We are targeting the table with cellpadding attribute with the value of 3
      # We can select using id, class or HTML tag , for more information check the beautifulsoup doc
      table = tables[0] # the result is a list, we are taking out data from it
      for td in table.find('tr').find_all('td'):
          print(td.text)



