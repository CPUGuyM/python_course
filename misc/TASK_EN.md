## IF expression
1. Print out table of truth for expressions:

```
	x and y
	x or y
	x and not y
	(x or z) and (y or z)
```

For `x, y, z = 0 or 1`

2. How infinite can loop look like?


## Loops and If expression

1. Input some number in to your program and 
check if number is prime.

2. Print out all prime numbers from some
defined range.

3. Run in your program in infinit loop on each step 
of ask for user to input some value. If new value 
is equal to letter 'q' finish your program.

4. Find out sum of all Fibonacci  numbers 
which is less than 4000000.

5. Find out all Pythagorean triple in defined range.

## Function

1. Write fucntion without arguments, which 
prints out hello messsga with you'r name

2. Write function with one string argument. 
Function should print out argument

3. Write function which is calculation square value 
of its argument and return reuslt.

4. Write function calculating 
factorial (n! = 1 * 2 * 3 *...* n) of its argument 

5. Write function calculating 
N-th Fibonacci number. Parametr N should 
be function argument.

5. Write function calculating 
N-th Fibonacci number. Parametr N should 
be function argument (recursive).

6. Write function calulating N-th number of arithmetic progression, 
step of progression sould pass to function as argument (default value of for step should be 1)

```
# to define default argument value so called named argumnets
def some_function(arg_without_default_value, arg_with_default_value=1):
   # do some work
   # ...

# you can use it than
some_function(12, 13) # it will run function some_function 
		      # with arg_without_default_value=12, arg_with_default_value=13

# or
some_function(12) # it will run function some_function
		  # with arg_without_default_value=12, arg_with_default_value=1

# or
some_function(12, arg_with_default_value=7) # it will run function some_function
		  			    # with arg_without_default_value=12, arg_with_default_value=7


# order of arguments is important! First should be defined arguments withour default value! 

```

7. Write function to reverese the list 

```
# list could be defined as 
l = [] # empty list
l = [1,2] #ist with two items 1, 2
# to appenda value to list
l.append(3)
l.append(4)
# after that list will be looks like [1,2,3,4]

def revert_list(l):
   # your code which is reverting list l
   # and will return l 

print(revert_list(l))
# will print 4,3,2,1
```

## List, slice tuples, generator, string

Operation |	Result 
----------|----------------
s[i] = x | item i of s is replaced by x
s[i:j] = t | slice of s from i to j is replaced by the contents of the iterable t	 
del s[i:j] | same as s[i:j] = []	 
s[i:j:k] = t | the elements of s[i:j:k] are replaced by those of t	(1)
del s[i:j:k] | removes the elements of s[i:j:k] from the list	 
s.append(x) | appends x to the end of the sequence (same as s[len(s):len(s)] = [x])	 
s.clear() | removes all items from s (same as del s[:])	(5)
s.copy() | creates a shallow copy of s (same as s[:])	(5)
s.extend(t) or s += t | extends s with the contents of t (for the most part the same as s[len(s):len(s)] = t)	 
s *= n | updates s with its contents repeated n times	(6)
s.insert(i, x) | inserts x into s at the index given by i (same as s[i:i] = [x])	 
s.pop([i]) | retrieves the item at i and also removes it from s	(2)
s.remove(x) | remove the first item from s where s[i] == x	(3)
s.reverse() | reverses the items of s in place	(4)

1. Crete list of numbers from 0 to 100 (by loop and by list comprehension)
2. Crete list of squares of previous list (by loop and by list comprehension)
3. Crete list of odd elements of previous list (by loop and by list comprehension)
4. We have a string: `rewlkdfsklgjdflkjglkdsfjgkldfsjglkjeroitewuiotujdigjsdfklg;klsdfgkl;jsdfkl;gjldk;sfjgjlk;sdfjlk;gjsdfl;kgl;kdsfjgl;kjsdfl;kgjl;sdfkjg;lkjsdflbvjdfslkglkrewjhtiowerjutioerutopiytuilyhjdsfl;kghjl;sdkf;gjdffffffffflkgjlkdfjglkasjdfoitweigheripjgierglisjdfkjlghsdfkj;l;hgkljasdhfglk;hsdfkjlghlk;sdfhg;kljsdflkgjlk;sdfjgl;ksdfjl;kgjsdfl;kjglk;sdfjgkjsdfl;kgjs;dlkfjgoiw3eujtio34wuytiergoijherjhlgjsdflkjgkl;dfjgkl;sdfjkl;gjsdf;lkjg;lsjeriotuerl;kjdsfkl;jgh;lksdfjg;lksdfjg;lksdfkjg;lkjreopyulidsjfl;kghjs;ldkjg;lkkjr5l;h;kljyhkl;rirtiririiiiiiiiiiiiiierwtsj;kldfjg;lksdfjgl;ksdjfl;gj;lsdfjg;lk` - remove all repated chars print string with unique chars.
5. What sub sequance of repeated letters is longest?
6. Write function which deleting some defined letter from string test it on previous string
7. We have list of some integer numbers - 2,3,3,45,4,23,43,54,34,5,32,423,4,23542354,3422,243,4,3,3,254,5643,3233,3,3,4,43,2,423,3,3,45,5,43,2,1,4,34234,34,3,342,23,4543,534,32423,23,4,4,4,3,423,3245,23,3,34254,235,234,5,235,4,345,235,23,5523,5,234,52,67,756,76,57,345,23,31,7,8,56,346,345,756,4343,754,674,8,568,9,65,34,3,5474,5687,56,2,3 - calc summ of this numbers
8. Find out max/min elements of previous list
9. Sort list by buble sort (write by yours)
10. Write programm which is asking user to how many Fibonacci numbers it should generate and than generate it.
11. Write function which is generating matrix as list of list (by loop and generator)
12. Write fuction for transposing matrix
13. Write fuction for summing of matrix
14. Write fuction for multipliyng of matrix
15. Write function for resolve of System of linear equations by [Gauss method](https://en.wikipedia.org/wiki/Gaussian_elimination).

## Map

Map - is key, value storage. To create map you need init your var with {}

```
# in python map defines like this
my_map = {}
# you can put value into map as 

my_map['some_key'] = 'some value'

# key could be any hashable object

```
### Task

1. Genrate map for storing phonebook, by name you should find phone number.
2. Write function for checking if number for particular name is exist in phonebook.
3. Write script which read input from user and show phne number for particular person if it exists
4. Write function for concatenate of two dicts `concatenate(dict1, dict2)` and returning concatenated dict.

## Set

Set is object which has number of unique elements. To create set you need write `set()`
```
# Create set
s = set()
>>> {}

# crete set from list
s = set([1,2,3,4,5])
>>> {1,2,3,4,5}

```
### Task

1. Create list with repeated elements and than create set from it.
2. Define operation under sets (union, intersection, difference of two sets) - **don't use standart**, do it yourself. 
3. Find simplest way to delete all repasted chars from thsi string - 'rewlkdfsklgjdflkjglkdsfjgkldfsjgliiiiiiiiiierwtsj;kldfjg;lksdfjgl;ksdjfl;gj;lsdfjg;lk'    

## Work with file
To open file for read you can use function [`open`](https://docs.python.org/3.6/library/functions.html#open) e.g.

```
# first argument indicates path to file include name of file, second mode of of opening file usualy it's
# equal to r - for reading, w - for writing, a - for appending to the end of the file. For more info see doc.
# you can use simultaneously several mode e.g. 'rw' - means that file will be open for read and write
my_file = open('path to file', 'r')

# To read all file you can use functuion read, it will return string wit contentt of file
file_content = my_file.read()

# you can read file line by line just using for loop
for line in my_file:
	# do smth
	...
# To write smth to file you need open file in write mode
my_file = open('path to file', 'w')

str_to_put = "To be, or not to be, that is the question…"

# this function will write to end of file 
my_file.write(str_to_put)

# DON'T forget to close file after work is finished

my_file.close()


# NOTE if you're open file file in w - write mode all content will be erased, TO add into file new you need use a - append mode
```

#### Task

1. Write script which is doing several math operation: sum, div, mult, subtraction with imputed number
2. When script starting it should ask user to imput name, than operation which he want to compute, and two arguments.
3. Write logger for your program. Logger should write all operation of your program into a file e.g.
```
def logger(operation_name, lef_arg, right_arg):
	# open file
	# make string, string should starts with user name
	# put to file
	# close file
	...

def mult(a, b):
	logger('mult', a, b)
	return a * b
```

### OOP tasks
1. Create class for several different animals type. Yuor calass should contain several atributes and several public methods.  What common among your classes could you highlight?
2. Highlight common part of your classes into one absttract interface.


# Final Task
Write program calculator. Main aim of program is to process arithmetical expression and show result e.g.:
```
1 + 2
>>> 3
```   
It also should be possible define variables e.g.:
```
x=2*(4+2)
x
>>> 12
```
And use them after definition e.g.:
```
y = 12
x = 10
z = x * y
z
>>> 120
```
There are should be ability to create function. function definition: first reserved word `function` than name of function and in brackets all list of all needed arguments after `:` as delimiter of function declaration and definition e.g:
```
function pow2(x): x*x
```
After definition if function it will be available fo user
```
pow2(3)
>>> 9
```
It should be possible to see all available variables and function in context of program.
```
print
>>> x - variable
    y - variable
    z - variable

pow2 - function
```
If user write `quit`. Calculator should close. Don't forget to process all possible exceptions e.g. division by zero. Or using not defined vars.
