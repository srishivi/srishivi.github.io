<h1> Python basics </h1>

- To make a script
  - #!/usr/bin/python
  - chmod +x test.py     # This is to make file executable
  -./test.py
  
- To take user input
  -raw_input("\n\nPress the enter key to exit.")
  
- Python has five standard data types −
  - Numbers
  - String
  - List
  - Tuple
  - Dictionary
 
 - Printing String and Sub Strings
   
    str = 'Hello World!'

    print str          # Prints complete string
    print str[0]       # Prints first character of the string
    print str[2:5]     # Prints characters starting from 3rd to 5th
    print str[2:]      # Prints string starting from 3rd character
    print str * 2      # Prints string two times
    print str + "TEST" # Prints concatenated string
    
  - Python Lists
    - Python Lists are like arrays in java. However the difference is lists can hold data of different data types.
    - A list contains items separated by commas and enclosed within square brackets [].
    - list = [ 'abcd', 786 , 2.23, 'john', 70.2 ]
             tinylist = [123, 'john']

        print list          # Prints complete list
        print list[0]       # Prints first element of the list
        print list[1:3]     # Prints elements starting from 2nd till 3rd # [786 , 2.23]
        print list[2:]      # Prints elements starting from 3rd element
        print tinylist * 2  # Prints list two times
        print list + tinylist # Prints concatenated lists
        
  - Python Tuples
    - A tuple is another sequence data type that is similar to the list. 
    - A tuple consists of a number of values separated by commas.
    - Tuples are enclosed within parentheses.
    - The main differences between lists and tuples are: Lists are enclosed in brackets ( [ ] ) and their elements and size can be changed, while tuples are             enclosed in parentheses ( ( ) ) and cannot be updated.   
    - Tuples can be thought of as read-only lists.  
    - The following code is invalid with tuple, because we attempted to update a tuple, which is not allowed.   
      #!/usr/bin/python

      tuple = ( 'abcd', 786 , 2.23, 'john', 70.2  )
      list = [ 'abcd', 786 , 2.23, 'john', 70.2  ]
      tuple[2] = 1000    # Invalid syntax with tuple
      list[2] = 1000     # Valid syntax with list
      
  - Python Dictionary
    - Python's dictionaries are kind of hash table type.
    - Consist of key-value pairs.
    - A dictionary key can be almost any Python type, but are usually numbers or strings.
      Values, on the other hand, can be any arbitrary Python object.
    - Dictionaries are enclosed by curly braces {} and values can be assigned and accessed using square braces [].
    -  ```#!/usr/bin/python

        dict = {}
        dict['one'] = "This is one"
        dict[2]     = "This is two"

        tinydict = {'name': 'john','code':6734, 'dept': 'sales'}


        print dict['one']       # Prints value for 'one' key
        print dict[2]           # Prints value for 2 key
        print tinydict          # Prints complete dictionary
        print tinydict.keys()   # Prints all the keys
        print tinydict.values() # Prints all the values
        This produce the following result −

        This is one
        This is two
        {'dept': 'sales', 'code': 6734, 'name': 'john'}
        ['dept', 'code', 'name']
        ['sales', 6734, 'john']```
