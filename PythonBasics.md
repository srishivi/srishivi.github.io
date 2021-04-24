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
   
    ```str = 'Hello World!'

    print str          # Prints complete string
    print str[0]       # Prints first character of the string
    print str[2:5]     # Prints characters starting from 3rd to 5th
    print str[2:]      # Prints string starting from 3rd character
    print str * 2      # Prints string two times
    print str + "TEST" # Prints concatenated string```
    
    - Raw Strings : print r'\n' prints \n and print R'\n'prints \n
    
  - Python Lists
    - Python Lists are like arrays in java. However the difference is lists can hold data of different data types.
    - A list contains items separated by commas and enclosed within square brackets [].
    - ```list = [ 'abcd', 786 , 2.23, 'john', 70.2 ]
         tinylist = [123, 'john']

        print list          # Prints complete list
        print list[0]       # Prints first element of the list
        print list[1:3]     # Prints elements starting from 2nd till 3rd # [786 , 2.23]
        print list[2:]      # Prints elements starting from 3rd element
        print tinylist * 2  # Prints list two times
        print list + tinylist # Prints concatenated lists```
        
  - Python Tuples
    - A tuple is another sequence data type that is similar to the list. 
    - A tuple consists of a number of values separated by commas.
    - Tuples are enclosed within parentheses.
    - The main differences between lists and tuples are: Lists are enclosed in brackets ( [ ] ) and their elements and size can be changed, while tuples are             enclosed in parentheses ( ( ) ) and cannot be updated.   
    - Tuples can be thought of as read-only lists.  
    - The following code is invalid with tuple, because we attempted to update a tuple, which is not allowed.   
      ```#!/usr/bin/python

      tuple = ( 'abcd', 786 , 2.23, 'john', 70.2  )
      list = [ 'abcd', 786 , 2.23, 'john', 70.2  ]
      tuple[2] = 1000    # Invalid syntax with tuple
      list[2] = 1000     # Valid syntax with list```
      
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
       
      - Dictionaries have no concept of order among elements. It is incorrect to say that the elements are "out of order"; they are simply unordered.
  
  - Data type conversion can be simply done as str(x)
    where x is to be converted to String format.
    
  - Operations
    - Floor devision // is the division in which the result after division is rounded off. Only the integer value is kept
    - 7//4 = 1
    - but if one of the operand is negative, values are rounded off towards negative infinity
    - -7//4 = -2
    - Python membership operator :
      - Python’s membership operators test for membership in a sequence, such as strings, lists, or tuples. 
      - Evaluates to true if it finds a variable in the specified sequence and false otherwise.
        x in y, here in results in a 1 if x is a member of sequence y.
      - Python identity operator :
        - Evaluates to true if the variables on either side of the operator point to the same object and false otherwise.

  - Loops
    - While loop
    - For loop
    - Nested loop

   - While loop
     - A while loop statement in Python programming language repeatedly executes a target statement as long as a given condition is true.
     - If the else statement is used with a while loop, the else statement is executed when the condition becomes false.
     - ```#!/usr/bin/python

            count = 0
            while count < 5:
               print count, " is  less than 5"
               count = count + 1
            else:
               print count, " is not less than 5" ```
             
     - For loop
       - can be used to iterate over a loop or string.
       - ``` #!/usr/bin/python

          for letter in 'Python':     
             print 'Current Letter :', letter
       - If the else statement is used with a for loop, the else statement is executed when the loop has exhausted iterating the list.

      - Loop control statements 
        - Loop control statements change execution from its normal sequence.
        - When execution leaves a scope, all automatic objects that were created in that scope are destroyed.
        
        - break statement
          - the break statement brings you out of the loop.
        - contine statement
          - continue statement sends the flow to the check condition statement of the loop.
          - Causes the loop to skip the remainder of its body and immediately retest its condition prior to reiterating.
        - pass statement
          - It is used when a statement is required syntactically but you do not want any command or code to execute.

  - Python supports formatted strings.
    ```#!/usr/bin/python

      print "My name is %s and weight is %d kg!" % ('Zara', 21)```
      
  - Triple Quotes
    - Python's triple quotes comes to the rescue by allowing strings to span multiple lines, including verbatim NEWLINEs, TABs, and any other special characters.
    - The syntax for triple quotes consists of three consecutive single or double quotes.
    - ```#!/usr/bin/python

        para_str = """this is a long string that is made up of
        several lines and non-printable characters such as
        TAB ( \t ) and they will show up that way when displayed.
        NEWLINEs within the string, whether explicitly given like
        this within the brackets [ \n ], or just a NEWLINE within
        the variable assignment will also show up.
        """
        print para_str```
        
    - <h1> Date and Time </h1>
      - Time in seconds since the epoch can be found as
        ``` print(time.loaltime(time.time()))```
      - To get formatted time in String format.
        - time.asctime(time.localtime(time.time()))
     
     - <h1> Functions </h1>
         - functions in python are pass by reference.
         - 
            
                 
                  # Function definition is here
                  def changeme( mylist ):
                     "This changes a passed list into this function"
                     mylist.append([1,2,3,4]);
                     print "Values inside the function: ", mylist
                     return

                  # Now you can call changeme function
                  mylist = [10,20,30];
                  changeme( mylist );
                  print "Values outside the function: ", mylist

                  # Here, we are maintaining reference of the passed object and appending values in the same object. So, this would produce the following result −
                  Values inside the function:  [10, 20, 30, [1, 2, 3, 4]]
                  Values outside the function:  [10, 20, 30, [1, 2, 3, 4]] ```
          
        - When passed value is not altered.
               
                  ``` #!/usr/bin/python
                  # Function definition is here
                  def changeme( mylist ):
                     "This changes a passed list into this function"
                     mylist = [1,2,3,4]; # This would assig new reference in mylist
                     print "Values inside the function: ", mylist
                     return

                  # Now you can call changeme function
                  mylist = [10,20,30];
                  changeme( mylist );
                  print "Values outside the function: ", mylist ```
          
          
    -  The parameter mylist is local to the function changeme. Changing mylist within the function does not affect mylist. The function accomplishes nothing             and finally this would produce the following result −
          - Values inside the function:  [1, 2, 3, 4]
            Values outside the function:  [10, 20, 30]
            
     - <h2> Function arguments </h2>
          - You can call a function by using the following types of formal arguments −

            - Required arguments : Regular functions
            - Keyword arguments : here arguments can be passed with the variable name while calling the functions.
            - Default arguments : here default arguments are provided in the function definition. Also parameter are passed with the key name.
            - Variable-length arguments. : def fun (var1 , * var2) ; All the extra variable passed is assigned to the tuple.
            
      - <h2> Anonymous Functions </h2>
        - These functions are called anonymous because they are not declared in the standard manner by using the def keyword. 
        - You can use the lambda keyword to create small anonymous functions.
        - An anonymous function cannot be a direct call to print because lambda requires an expression.
        
