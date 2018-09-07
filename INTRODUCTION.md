# Introduction to python, a complementary to our programming course intro.

After successfully installing python to your computer hello world is always a great way to check if everything installed correctly.

## Table of contents

1. [Basic - introduction](#basics)
2. [if/else statements](#statements)
3. [string](#string)
4. [Loops](#loops)
5. [Using libraries](#libraries)


# Basics

## Hello World!
the classic,  
Output `hello world!` in console.  

Tips: if you really need help, google [Python output](http://lmgtfy.com/?q=Python+output)

## Assign two numbers.

assign two variables with.
```python
a = 10
b = 5

# math, a + b = c

print c

# Output = 15
```

## Add two numbers.

Output `a + b = c`

Tips: use input to assign values to `a` and `b` then output the sum of them.

## Find the square root.

Output example `sqrt(9) = 3`

Tips: Use multiplication.

## Calculate area of a triangle

Output example: `The area of the triangle is 7.50` (input base = 5, height = 3)

Tips: input base and height. Use float for right formatting.

## Swap two variables.

Here is some help: 
```python
X = "variable1"
Y = "variable2"

# Your code

print("value of X after the swap is: %d", X) # Should print "Variable2"
print("value of Y after the swap is: %d", Y) # Should print "Variable1"
```
Tips: Use a temp variable.

## Convert Kilometers to Miles.
Output example: `10.00 Kilometers equals 6.21 Miles`

Tips: Conversion factor is 0.621371

## Write a program to concatenate following dictionaries to create a new one.
Example output
```bash
Input
dic1={1:10, 2:20}
dic2={3:30, 4:40}
dic3={5:50,6:60}
Output
{1: 10, 2: 20, 3: 30, 4: 40, 5: 50, 6: 60}
```

## Sum all the items in a dictionary.
Example output
```bash
Input {'data1':100,'data2':-54,'data3':247}
Output 293
```

## password validation
Write a program to check the validity of a password (input from users).
Validation :
At least 1 letter between [a-z] and 1 letter between [A-Z].
At least 1 number between [0-9].
At least 1 character from [!$#@].
Minimum length 6 characters.
Maximum length 16 characters.
```bash
Input:
D4T3@abo!

Output:
Valid password
```

## Remove duplicates in list.
Example output
```bash
Input = [10,20,30,20,10,50,60,40,80,50,40]
Output [10, 20, 30, 50, 60, 40, 80]
```

# statements

## Is a number negative or positive?
Output example `-5 is negative`

Tips: Input a number, then use [if statement](http://anh.cs.luc.edu/handsonPythonTutorial/ifstatements.html) to check it and printout the answer.

## Check Leap year.
This is a brain teaser..

Output ´1920 is a leap year´

Tips: Leap year is every 4th year, years ending with 00 is not a leap year, except every 400 year.

# Loops

## Loop patterns
Reconstruct the following patterns:
```bash
1
22
333
4444
55555
666666
7777777
88888888
999999999
```

using a [nested for-loop](https://www.tutorialspoint.com/python/python_nested_loops.htm).
```bash
* 
* * 
* * * 
* * * * 
* * * * * 
* * * * 
* * * 
* * 
*
```
```bash
* *
* * * *
* * * * * *
* * * * 
* * 
* * * * 
* * * * * *
* * * *
* * 
```

## Convert Decimal to Binary
Example output: `23 = 10111`
This one might be tricky without google. It's doable if you know your binaries well.

Convert Decimal to Binary is pretty simple with the help of recursion.


## Fibonacci
Fibonacci is a recurring sequence, it's a greate test of logics and a first glance of recursion.
Recursion is when you call your method from within your method. Huh.., what are you talking about?!

Let's give you an example:
```python
def recursive(a):
    if a <= 1:
        print 'last output: 1'
    else:
        print(a)
        recursive(a - 1)
````

 Print 10..1 with help of recursion
recursive(10)
```
Output:
```python
10
9
8
7
6
5
4
3
2
last output: 1
```

Now here is the challange, input a value and print the fibonacci sequence up to n:th term.

Tips: From wikipedia; `For all integers n>1, Fib(n):=Fib(n-1) + Fib(n-2).`

# libraries

## Simple guessing game with random number
Generate a random number with the help of the `random` library
Have the user guess the number, continue to guess untill it's right.
For your own sanity, limit the number interval to be somewhat reasonable.

Tips: use a while loop.

## Print calendar month
Sounds more challanging right?  
Output example
```bash
    August 2018
Mo Tu We Th Fr Sa Su
       1  2  3  4  5
 6  7  8  9 10 11 12
13 14 15 16 17 18 19
20 21 22 23 24 25 26
27 28 29 30 31
```
This is very easy with the help of the library *surprice surprice* `calendar`

Tips: Here again, google is your friend. Sometimes reading a long documentation of a library can be intriguing..
Google more specific will give you a better example: ["print calendar month with python"](https://www.tutorialspoint.com/How-to-print-calendar-for-a-month-in-Python).

## Write a program to generate all permutations of a list.
This will become very hand later in other courses ;)

example output
```bash
input [1,2,3]
Output [(1, 2, 3), (1, 3, 2), (2, 1, 3), (2, 3, 1), (3, 1, 2), (3, 2, 1)]
```

Tips: `import itertools`

# String
## Palindrome word?

Example output: `"anna" is a palindrome.`

Input a string and check if the revese of the string matches.

Tips: use `reversed()`

## Palindrome string?

Example output: `"Murder for a jar of red rum" is a palindrome.`

Close to 1a but you have to handle whitespace.
What about uppercase, how do you handle this?

Tips: use `str.replace()`

EXTRA: Here is some challanges for you. can my manage to clear these as palindromes with your program.
* Borrow or rob?
* Yo, banana boy!
* Ed, I saw Harpo Marx ram Oprah W. aside.

## Split a sentence and sort words in alphabetic order.

Example output
```bash
Input: "Hello my name is Albin"
Output:
Albin
Hello
is
my
name
```

Tips: make a list of words, then use sort().

## Count even and odd numbers
Input a number is Integers, separated with commas (,)
Output number of even numbers and numbers of odd numbers.

Example output
```python
numbers = (1, 2, 3, 4, 5, 6, 7, 8, 9) #a tuple of numbers

Output
Numbers of even numbers: 4
Numbers of odd numbers: 5
```


Tips: use the egular expression library `re` [google it ;)](https://docs.python.org/2.7/library/re.html).

## Write a program to find common items from two lists.
Example solution
```python
input
car1 = "Volvo", "BMW", "SAAB", "Tesla"
car2 = "Lada", "Tesla", "Volvo", "Renault"
output
{'Volvo', 'Tesla'}
```

## Write a program to get the difference between the two lists
Example solution
```python
input
car1 = "Volvo", "BMW", "SAAB", "Tesla"
car2 = "Tesla", "Volvo"
output
{'BMW', 'SAAB'}
```

## Write a program to find the largest number in list.
Example output
```bash
largest_num_in_list([6, 12, -3, 0, 2, -12])
return 12
```


## Caesar encryption solution.
N.B: In cryptography, a Caesar cipher, also known as Caesar's cipher, the shift cipher, Caesar's code or Caesar shift, is one of the simplest and most widely known encryption techniques.
It is a type of substitution cipher in which each letter in the plaintext is replaced by a letter some fixed number of positions down the alphabet.
For example, with a left shift of 3, D would be replaced by A, E would become B, and so on.
The method is named after Julius Caesar, who used it in his private correspondence.

Example output
```bash
plaintext:  defend the east wall of the castle
ciphertext: efgfoe uif fbtu xbmm pg uif dbtumf
```

## Convert roman numbers to a integer.
Example output
```bash
input:
'MMMCMLXXXVI'
'MMMM'
'C'
output:
3986                                                                                                          
4000                                                                                                          
100
```
Tips: define a dictionary of all roman numbers to it's equivalent integer.
`output += rom_dict[input[i]] - 2 * rom_dict[input[i - 1]]`

## More will be added later! :) 
