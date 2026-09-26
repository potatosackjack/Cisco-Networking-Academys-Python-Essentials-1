## Expectations

As I mentioned in my expectations section for Module 01, I had made it to the middle of Module 02, 
which, after reviewing the material, I realized was inaccurate.

I'm just now noticing that the first section of this module is pretty in-depth. Maybe I was speeding 
through it the first time because I hadn't yet understood how to properly put information into a 
repository.

Taking notes and documenting my process in a repository has changed a big part of how I process 
information. I now take notes on every section instead of simply noting highlighted information or 
concepts that stood out to me.

With that said, my expectations have changed. When I began building my Markdown file for Module 01 
and slowed down, I noticed how much information I had actually been missing.

I expect that this time around, I'll have a better grasp of concepts like **parameters** and 
**arguments**. That's not to say I haven't watched a million videos in between my note-taking 
reboot, but I do believe there's a sense of rhythm that develops when the note-taking process has 
order and sequence.

I imagine I'll get stuck at times, but I'll just add those concepts to the bin of things to turn 
into flashcards and review, like **interpreters vs. compilers**.

I imagine new terms and syntax will initially become soft information, but with consistent study and 
repetition, that information will become more solid and eventually feel natural.

# 2.1 Section 2 The "Hello World!" Program
## 2.1.1 Your very first program

```
print("Hello World!")
```
this first program consists of: 
- the word print
- an opening parenthesis
- a quotation mark
- a line of text: Hello, World!
- another quotation mark
- a closing parenthesis

Each element carrying an important role

## 2.1.2 The print() function

Print in the line of text below is a function 
```
print("Hello World!")
```
That doesn't mean that wherever the word appears it is always a function name.

A function (in this context) is a separate part of the computer code able to:
- cause some **effect** (e.g., send text to the terminal, create a file, draw an image, play a sound, etc.) Unheard of in mathematics this is why functions in code are considered more dynamic. 
- valuate a value (e.g., the square root of a value or the length of a given text) and return it as the function's **result**.

Moreover, many Python functions can do the above two things together. ‒ some Python functions don't need any argument.

**Where do the functions come from?**
-  From Python itself (it is built-in)
-  Python's add-ons named modules
-  Write them indepedently

Print function is self-evident

## 2.1.3 Function arguments
As we said before, a function may have:

- an effect (Example: something appears on the screen)
- a result (Example: ```x = len("Python")``` produces the result 6) 
There's also a third, very important, function component ‒ the **argument(s)**.

🔑 If you want to deliver one or more arguments to a function, you place them inside the parentheses. If you're going to use a function which doesn't take any argument, you still have to have the parentheses.

**String as the print() function's argument**

String: a data type used to represent text. It is essentially a sequence of characters (which can include letters, numbers, symbols, and spaces) bundled together as a single unit.

```
print("Hello, World!")
 ↑          ↑
function    argument
```
The string is *Hello, World!*

Almost anything you put inside the quotes will be taken literally, not as code, but as **data**.

🧠 My honest perception: The world argument was making grasping the concept very difficult because I instinctively couldn't
separate the idea from a argument in regards to a disagreement. 

So 

I did research on the word argument and the word comes from the Latin word *argumentum*, meaning "logical proof, evidence, or token." It stems from the Latin Root word *arguere*, which means "to make clear, make known, or prove."  
↓  
Old French: The term entered Old French as arguement in the 13th century, meaning reasoning or an accusation.  
↓  
It appeared in English early 14th century (recorded before 1325 in legal texts like the Statutes of the Realm). At this time, it meant a statement or set of reasons offered in support of a proposition or to establish a truth.  
↓  
By the 1590s, the word expanded to mean a subject of debate or discussion.  

## 2.1.4 Function invocation**

It basically means:

Calling a function so that it actually runs.

### Start with a function

Suppose we define a function:

```python
def greet():
    print("Hello!")
```

At this point, Python has **defined** the function, but it hasn't run it.

Think:

"Here's a function called `greet`. Remember what it does."

### Now invoke the function

```python
greet()
```

That is a **function invocation**.

You're telling Python:

"Run the `greet` function now."

The result:

```text
Hello!
```

Why call it "invocation"?

**Invoke = call upon something to perform an action.**

So:

**Function invocation = calling a function to execute it.**

You may hear these terms used almost interchangeably:

* **Call a function**
* **Invoke a function**
* **Function call**
* **Function invocation**

They're referring to essentially the same action.

**Where do arguments come in?**
This is where it connects to what you've already been studying.

Suppose:

```python
def greet(name):
    print("Hello", name)
```

`name` is a **parameter**.

Now:

```python
greet("potatosackjack")
```

You're **invoking** the function and providing `"potatosackjack"` as an **argument**.

```text
def greet(name):
          ↑
       parameter

greet("potatosackjack")
      ↑
    argument

greet("potatosackjack")
      ↑
function invocation
```

The function executes:

```text
Hello potatosackjack
```

One important distinction

Simply **writing a function definition** doesn't invoke it:

```python
def greet():
    print("Hello")
```

You're defining it.

Writing:

```python
greet()
```

**invokes it.**

So a great note for your studies would be:

Function invocation is the act of calling a function so that its instructions are executed. Arguments can be provided during the invocation to give the function the data it needs.

And this connects nicely to your earlier question about arguments: **an argument is something you provide during a function call/invocation.**

## 2.1.5   LAB   Working with the print() function

The ```print()``` command, which is one of the easiest directives in Python, simply prints out a line to the screen.

LAB:

**Instruction 1:** Use the ```print()``` function to print the line ```Hello, Python!``` to the screen. Use double quotes around the string.

Input: 

```
print("Hello,Python!")
```

Output:

```
Hello,Python!
```

**Instruction 2:** Having done that, use the ```print()``` function again, but this time print your first name.  

Input: 

```
print("Hello,Potatosackjack!")
```

Output:

```
Hello,Potatosackjack!
```

**Instruction 3:** Remove the double quotes and run your code. Watch Python's reaction. What kind of error is thrown?

Input: 

```
print(Hello,Potatosackjack!)
```

Output:

```
File "main.py", line 1
    print(Hello,Potatosackjack!)
                              ^
SyntaxError: invalid syntax
```

**Instruction 4:** Then, remove the parentheses, put back the double quotes, and run your code again. What kind of error is thrown this time?

Input: 

```
print"Hello,Potatosackjack!"
```

Output:

```
File "main.py", line 1
    print"Hello,Potatosackjack!"
                               ^
SyntaxError: invalid syntax

```
 
## 2.1.6 The print() function and its effect, arguments, and values returned

**What effect does the ```print()``` function cause?**
- takes its arguments
- converts them into human-readable form
- sends the resulting data to the output device (anything you put into the print() function will appear on your screen.)
  
**What arguments does ```print()``` expect?**
- Any. (ex. Strings, numbers, characters, logical values, objects)

**What value does the ```print()``` function return?**
- None.

## 2.1.7 Instructions 
Python's syntax is quite specific in this area. Unlike most programming languages, Python requires that there cannot be more than one instruction in a line.

A line can be empty (i.e., it may contain no instruction at all) but it must not contain two, three or more instructions. This is strictly prohibited.

**Example 1:** 

Input: 

```
print("The itsy bitsy spider climbed up the waterspout.")
print("Down came the rain and washed the spider out.")
```

Output:

```
The itsy bitsy spider climbed up the waterspout.
Down came the rain and washed the spider out.
```

The program invokes the ```print()``` function twice, this means that ```print()``` begins its output from a new line each time it starts its execution

This means that the instructions in the code are executed in the same order in which they have been placed in the source file.

**Example 2:** 

Input: 

```
print("The itsy bitsy spider climbed up the waterspout.")
print()
print("Down came the rain and washed the spider out.")
```

Output:

```
The itsy bitsy spider climbed up the waterspout.

Down came the rain and washed the spider out.
```

Notice the the empty print() invocation output an empty line/newline. 

## 2.1.8 Python escape and newline characters

The backslash ```(\)``` has a very special meaning when used inside strings ‒ this is called the escape character.

Its specific effect depends on the character that follows it.

**Backslash + another character = a special instruction or effect.**

These are called escape sequences

| Sequence | Meaning               |
| -------- | --------------------- |
| `\n`     | New line              |
| `\t`     | Tab                   |
| `\"`     | Double quotation mark |
| `\'`     | Single quotation mark |
| `\\`     | Literal backslash     |

Below is two use cases:

**Example 1:**

Input: 

```
print("The itsy bitsy spider\nclimbed up the waterspout.")
print()
print("Down came the rain\nand washed the spider out.")
```

Output:

```
The itsy bitsy spider
climbed up the waterspout.

Down came the rain
and washed the spider out.
```


**Example 2:**

Input: 

```
print("Name:\tJohn\nAge:\t25")
```

Output:

```
Name:   John
Age:    25
```

A backslash ```(\)``` is a special character in Python that can give the following character a special meaning, most commonly inside strings. Sequences such as ```\n``` and ```\t``` are called escape sequences and represent things like a new line or tab.

## 2.1.9 Using multiple arguments

Feeding the ```print()``` function with more than one argument.

Input: 

```
print("The itsy bitsy spider" , "climbed up" , "the waterspout.")
```

Output:

```
The itsy bitsy spider climbed up the waterspout.
```

Two conclusions emerge from this example:

A ```print()``` function invoked with more than one argument outputs them all on one line;
the ```print()``` function puts a space between the outputted arguments on its own initiative.

## 2.1.10 Positional arguments
You can provide arguments based on their **position**:

```
introduce("Potatosackjack", 25)
```

Python essentially matches them like this:

```
name ← "Potatosackjack"
age  ← 25
```

The first argument goes to the first parameter, and the second goes to the second.

That's a positional argument because its meaning comes from the order you put it in.

## 2.1.11 Keyword arguments

Keyword arguments

Instead, you can explicitly tell Python which parameter you're giving a value to:

```
introduce(name="Potatosackjack", age=25)
```

Now you're using keyword arguments.

The keywords are:

```
name
age
```

Python can match the values directly:

```
name ← "Potatosackjack"
age  ← 25
```

The important idea is:

**A keyword argument identifies the parameter by its name rather than relying on its position.**

In other words a keyword argument is an argument passed to a function using the name of the parameter it should be assigned to. Unlike a positional argument, where the argument's meaning depends on its position, a keyword argument explicitly identifies its parameter, so the order does not matter.

There isn't one universal list of **keyword arguments** because keyword arguments depend on the **parameters a particular function accepts**. But here are some common ones you'll encounter in beginner Python:

* **`end`** — controls what `print()` displays after its output.

  ```python
  print("Hello", end=" ")
  ```

* **`sep`** — controls what `print()` puts between multiple values.

  ```python
  print("Hello", "World", sep="-")
  ```

* **`file`** — specifies where `print()` sends its output.

  ```python
  print("Hello", file=my_file)
  ```

* **`flush`** — controls whether `print()` immediately sends its output.

  ```python
  print("Loading...", flush=True)
  ```

* **`start`** — specifies the starting value for `range()`-like operations such as `enumerate()`.

  ```python
  enumerate(["a", "b"], start=1)
  ```

* **`key`** — tells functions such as `sorted()` what to use when determining how to sort items.

  ```python
  sorted(words, key=len)
  ```

* **`reverse`** — tells functions such as `sorted()` whether to reverse the order.

  ```python
  sorted(numbers, reverse=True)
  ```

The important thing is that **`end`, `sep`, `key`, `reverse`, etc. aren't automatically keyword arguments**. They are **parameter names** when defined by a function, and they become keyword arguments when you provide values using those names:

```python
print("Hello", end=" ")
sorted(numbers, reverse=True)
```

So don't try to memorize a giant list. **Learn the parameter names of the functions you're using.**


## 2.1.12   LAB   The print() function and its arguments

Modify the first line of code in the editor, using the sep and end keywords, to match the expected output. Use the two print() functions in the editor.

Input: 

```
print("Programming","Essentials","in", sep="***", end="...")
print("Python")
```

Output:

```
Programming***Essentials***in...Python
```

**end** — controls what print() displays after its output.
**sep** — controls what print() puts between multiple values.

## 2.1.14 SECTION SUMMARY

1. The print() function is a built-in function. It prints/outputs a specified message to the screen/console window.

2. Built-in functions, contrary to user-defined functions, are always available and don't have to be imported. Python 3.8 comes with 69 built-in functions. You can find their full list provided in alphabetical order in the Python Standard Library.

3. To call a function (this process is known as function invocation or function call), you need to use the function name followed by parentheses. You can pass arguments into a function by placing them inside the parentheses. You must separate arguments with a comma, e.g., print("Hello,", "world!"). An "empty" print() function outputs an empty line to the screen.

4. Python strings are delimited with quotes, e.g., "I am a string" (double quotes), or 'I am a string, too' (single quotes).

5. Computer programs are collections of instructions. An instruction is a command to perform a specific task when executed, e.g., to print a certain message to the screen.

6. In Python strings the backslash (\) is a special character which announces that the next character has a different meaning, e.g., \n (the newline character) starts a new output line.

7. Positional arguments are the ones whose meaning is dictated by their position, e.g., the second argument is outputted after the first, the third is outputted after the second, etc.

8. Keyword arguments are the ones whose meaning is not dictated by their location, but by a special word (keyword) used to identify them.

9. The end and sep parameters can be used for formatting the output of the print() function. The sep parameter specifies the separator between the outputted arguments, e.g., print("H", "E", "L", "L", "O", sep="-"), whereas the end parameter specifies what to print at the end of the print statement.

# 2.2 Python Literals
## 2.2.1 Literals – the data in itself

A literal is a value that you type directly into your code.

🧠 My honest perception: I don't know why I get stuck on such basic concepts. The terms used in programming are often
straightforward, but sometimes I get confused when concepts work together, overlap, or share similar
buzzwords in their definitions. To better understand what a **literal** is, I had to open up ChatGPT—no surprise!—and clarify the concept. Originally, I thought a literal was basically the same thing as a parameter. After several
examples from ChatGPT, including asking for an explanation using a math analogy, I started to get
the idea. My current understanding is that a **function** is a block of code that can take in a value, a
**parameter** is a variable defined within a function, and a **literal** is the actual value itself.

ChatGPT's Clarification: Yes — it's mostly accurate, and it's a good reflection of what you currently understand. There's just one small technical adjustment I'd make.

Your statement:

"a parameter is a variable defined within a function"

is understandable, but more precisely:

A parameter is a variable in a function's definition that receives a value when the function is called.

So I'd make your final sentence:

My current understanding is that a **function** is a block of code that can take in a value, a
**parameter** is a variable in a function's definition that receives a value when the function is
called, and a **literal** is a value written directly in the code.

That last part is important because "actual value itself" can be a little misleading.

For example:

```
greet ("Potatosackjack")
```

"Potatosackjack" is a literal because it's written directly into the code.

It's also an argument because you're passing it to greet().

So you can have:

**Literal** → describes what the value is/how it's written
**Argument** → describes the value's role when passed to a function
**Parameter** → the variable in the function definition that receives that value.

That's a really useful distinction to have in your Module 2 notes.

## 2.2.1 Integers

**Numbers in Python**

**Integer (int)** — A whole number with no decimal or fractional part.
-Examples: 1, 25, -10, 100

**Float (float)** — A number that can contain a decimal or fractional part.
-Examples: 3.14, 2.5, -0.75

Easy way to remember

**Integer** = whole number
**Float** = number with a decimal

And one important detail: a float doesn't have to have a fractional value that isn't zero. For example, 5.0 is still a float because it's written with a decimal point.

Both of these kinds of numbers differ significantly in how they're stored in a computer memory and in the range of acceptable values.

Python doesn't allow the interjection  of any characters that are not digits inside a number.

**Prohibited**: ```11,111,111```, or like this: ```11.111.111```, or even like this: ```11 111 111```.

It's clear that this provision makes it easier to read, especially when the number consists of many digits. However, Python doesn't accept things like these. It's prohibited. What Python does allow, though, is the use of underscores in numeric literals.*

Therefore, you can write this number either like this: ```11111111```, like: ```11_111_111```.

Note **Python 3.6** has introduced underscores in numeric literals, allowing for the placement of single underscores between digits and after base specifiers for improved readability. This feature is not available in older versions of Python.

**Negative numbers** in Python? You can write: ```-11111111```, or ```-11_111_111```.

Positive numbers are allowed to be preceded by a plus sign. Same number: ```+11111111``` and ```11111111```.

Python allows integers to be written as decimal, binary, octal, or hexadecimal numbers.

**Decimal** — base 10 → 25  
**Binary** — base 2 → 0b11001  
**Octal** — base 8 → 0o31  
**Hexadecimal** — base 16 → 0x19  

The important thing is that octal and hexadecimal are ways of writing integer values. They don't represent a different type of number in Python.

## 2.2.3 Floats

**Float (float)** — A number that can contain a decimal or fractional part.
-Examples: 3.14, 2.5, -0.75

Ensure that your number doesn't contain any commas at all.Python sees the comma as something that separates two pieces of information (For example separating two arguments).

Python lets you leave out a zero when that zero doesn't change the value of the number.

The decimal point is essential for recognizing floating-point numbers in Python.

Look at these two numbers:

```
6
6.0
```

You may think that they are exactly the same, but Python sees them in a completely different way.

```6``` is an integer number, whereas ```6.0``` is a floating-point number.

**Scientific notation** is a way of writing very large or very small numbers in a shorter form. In Python, ```e``` is used to represent the power of 10.

Straightforward Python examples showing large, small, and negative numbers in scientific notation.

1. Large number

Input: 

```
number = 250000000
print(f"{number:e}")
```

Output:

```
2.500000e+08
```

That's Python's scientific notation for **250,000,000**.

2. Small number

Input: 

```
number = 0.0000025
print(f"{number:e}")
```

Output:

```
2.500000e-06
```

That's **0.0000025**.
The ```-06``` means the decimal point needs to move **6 places to the left**.

3. Negative number

```
number = -250000000
print(f"{number:e}")
```

Output:

```
-2.500000e+08
```
The **negative** sign tells you the number itself is negative.
Notice that the ```+08``` is separate—it describes the size of the number, not whether the number is positive or negative.

Python always chooses the more economical form of the number's presentation, and you should take this into consideration when creating literals.

## 2.2.4 Strings
A string is a sequence of characters enclosed in quotation marks.

```python
"Hello"
"Python"
"123"
```

Even `"123"` is a string because the quotation marks tell Python to treat the characters as **text**, rather than as the number 123.

**Simple way to remember**

**String** = text made up of characters.

Examples of characters include letters, numbers, spaces, and symbols:

```python
"Hello, world!"
"Python 3"
"$100"
```
In Python, an apostrophe (') and a quotation mark (") can both be used to create a string.

🔑 Remember the opening quotation or apostrophe is the beginning of the string and the closing quotation or apostrophe is the end of the string, however if you wanted to use quotation or apostrophe with in the string you would have to add a backslash in front of them to so Python isn't confused and prematurely wraps the string.

Example: 

```
"It's okay"       # ✅
'It\'s okay'      # ✅

'He said "Hi"'    # ✅
"He said \"Hi\""  # ✅
```
The quotes wrapping the string tell Python where the string starts and ends. If you use the same quote inside the string, Python may think you've ended the string.

## 2.2.5 Boolean values
The name comes from George Boole (1815-1864), the author of the fundamental work, The Laws of Thought, which contains the definition of Boolean algebra ‒ a part of algebra which makes use of only two distinct values: ```True``` and ```False```, denoted as ```1``` and ```0```.

computers know only two kinds of answers:

- Yes, this is true  
- No, this is false

These two Boolean values have strict denotations in Python. You cannot change anything ‒ you have to take these symbols as they are, including case-sensitivity.

```
True
False 
```

In Python, True and False can be compared because they have numerical values of 1 and 0. True is greater than False.

```True = 1``` → ```True > False``` → ```1 > 0``` → ```Is True greater than False?``` → ```True```  

```False = 0``` → ```True < False``` → ```1 < 0``` → ```Is True less than False?```  → ```False```

## 2.2.6   LAB   Python literals - strings

| Code | What it is |
|---|---|
| `"I'm"` | Regular string ✅ |
| `""learning""` | Invalid syntax ❌ |
| `"""Python"""` | Triple-quoted string ✅ |

The reason double quotes don't work is because Python sees the first "" as an empty string, then doesn't know what to do with learning, followed by another "".

**Triple quotes** (""") can be used to create a string. Everything between the opening and closing triple quotes is treated as part of the same string, including line breaks.

```
""" → START of the string
Python → the actual text
""" → END of the string
```
Their big advantage is that they can contain multiple lines. Python treats everything between the opening ```"""``` and closing ```"""``` as one string.

## 2.2.7 SECTION SUMMARY

1. **Literals** are notations for representing some fixed values in code. Python has various types of literals - for example, a literal can be a number (numeric literals, e.g., ```123```), or a string (string literals, e.g., "I am a literal.").

2. The **binary system** is a system of numbers that employs 2 as the base. Therefore, a binary number is made up of 0s and 1s only, e.g., ```1010``` is 10 in decimal.

Octal and hexadecimal numeration systems, similarly, employ *8* and *16* as their bases respectively. The hexadecimal system uses the decimal numbers and six extra letters.

3. **Integers** (or simply **ints**) are one of the numerical types supported by Python. They are numbers written without a fractional component, e.g., ```256```, or ```-1``` (negative integers).

4. **Floating-point** numbers (or simply **float**s) are another one of the numerical types supported by Python. They are numbers that contain (or are able to contain) a fractional component, e.g., ```1.27```.

5. To encode an apostrophe or a quote inside a string, you can either use the escape character, e.g., ```'I\'m happy.'```, or open and close the string using an opposite set of symbols to the ones you wish to encode, e.g., ``"I'm happy."``` to encode an apostrophe, and ```'He said "Python", not "typhoon"'``` to encode a (double) quote.

6. **Boolean values** are the two constant objects ```True``` and ```False``` used to represent truth values (in numeric contexts ```1``` is ```True```, while ```0``` is ```False```.


**Extra**  

There is one more, special literal that is used in Python: the ```None``` literal. This literal is a ```NoneType``` object, and it is used to represent the **absence of a value**. We'll tell you more about it soon.

# 2.3 Section 3 – Operators - data manipulation tools
## 2.3.1 Python as a calculator
Python to perform mathematical calculations just like you would with a calculator.

## 2.3.2 Basic operators

You can use the basic mathematical operators:


| Symbol | operation                         |
|--------|-----------------------------------|
| +      | Addition                          |
| -      | Subtraction                       |
| *      | Multiplication                    |
| /      | Division                          |
| //     | Integer division (floor division) |
| %      | Remainder (modulo)                |
| **     | Exponentiation                    |

**Addition Operator** 
In Python, the addition operator is ```+```. It tells Python to add two values together.

| Expression | Meaning | Result |
|---|---|---|
| `10 + 5` | Add numbers | `15` |
| `"Hello" + "World"` | Join strings | `"HelloWorld"` |

```+``` means add when you're working with numbers and join when you're working with strings.

**Subtraction Operator**
The subtraction operator in Python is the minus sign ```-```. It is used to subtract one value from another.

You cannot subtract strings, I'll produce a TypeError.

**Multiplication Operator**
The multiplication operator in Python is ```*```. It has a few different uses depending on what you're multiplying.

| Expression | What `*` does |
|---|---|
| `5 * 3` | Multiplies numbers |
| `2.5 * 4` | Multiplies decimals |
| `"Hi" * 3` | Repeats a string |
| `[1, 2] * 3` | Repeats a list |

**Division Operator**
The division operator in Python is ```/```. The / operator performs division and returns a floating-point number.
Even when the answer is a whole number, / normally gives you a float.

Example: 10 / 2 → 5.0

Just like the other arithmetic operators, you can divide variables:

```
total = 20
people = 4

print(total / people)
```

**Floor Division Operator** divides two numbers and rounds the result down to the next lowest whole integer (towards negative infinity).

- Positive results: ```7 / 3``` is ```2.333``..., which floors down to ```2```.
- Negative results: ```-7 / 3``` is ```-2.333```..., which floors down to ```-3``` (not -2).

**Remainder (modulo) Operator**
The modulo operator ```%``` tells you what is left over after division. 

Example: 

```
10 % 3
```

10 divided by 3 = 3, with 1 left over.

So:

```
10 % 3 = 1
```

So ```%``` → What's left over?

**Exponentiation Operator**
The exponentiation operator ```**``` is used to raise a number to a power.

```**``` → multiply a number by itself a certain number of times

## 2.3.3 Operators and their priorities
The phenomenon that causes some operators to act before others is known as the **hierarchy of priorities**.

🧠 Growing up, I learned the concept of PEMDAS to help with the order of operations. While I was always pretty decent at solving math problems, I just noticed a hiccup that probably played a big part in me finding certain equations difficult to solve. I was taught that you follow the order of PEMDAS from left to right. After doing some research during this study, I'm just now learning that **Parentheses → Exponents → Multiplication/Division → Addition/Subtraction** is the correct way to read it. The part I misunderstood was Multiplication/Division and Addition/Subtraction. Multiplication and division are performed left to right, and then addition and subtraction are also performed left to right. I always thought you followed the individual letters of PEMDAS in order, rather than treating multiplication and division, and addition and subtraction, as equal-priority operations. 

This is where **binding direction** becomes important. It helps explain why some operators are evaluated **left to right** while others are evaluated **right to left**.

**What does “binding” mean?**

Think of **binding** as an operator's tendency to "grab onto" the value next to it.

There are two important directions:

- **Left-to-right binding** → the operator works with the value to its **left first**, then continues toward the right.

- **Right-to-left binding** → the operator works with the value to its **right first**, then continues toward the left.

For example, addition is evaluated left to right:

```
10 - 3 - 2
```

Python reads this as:

```
(10 - 3) - 2
```

So:

```
7 - 2 = 5
```

It does **not** read it as:

```
10 - (3 - 2)
```

**But some operators go right to left**

Exponentiation is an important example:

2 ** 3 ** 2

Python evaluates this as:

```
2 ** (3 ** 2)
```

First:

```
3 ** 2 = 9
```

Then:

```
2 ** 9 = 512
``` 

So the answer is **512**, not 64.

**Why does this matter?**

This is one reason the **order of operations** isn't simply a matter of memorizing PEMDAS.

There are actually **two different** ideas involved:

**Precedence** tells you **which type of operator gets handled first**.

**Associativity** tells you **which direction operators of the same precedence are evaluated**.

So you can think of it like this:

**Precedence** = Which operator goes first?
**Associativity** = Which direction do we go when operators have the same precedence?

For your Module 2.3 notes, I'd actually use “**associativity**” rather than “binding” when you're talking specifically about **left-to-right vs. right-to-left**. That's the more precise programming term.

Python operator from highest priority to lowest priority (PEMDAS).

```
Parentheses
      ↓
Exponentiation
      ↓
Unary + / -
      ↓
* / // %
      ↓
+ -
```

Python operator precedence table, from highest priority to lowest priority.

| Priority | Operator(s)                                                      | Description                                      | Associativity |
| -------: | ---------------------------------------------------------------- | ------------------------------------------------ | ------------- |
|        1 | `()`                                                             | Parentheses                                      | —             |
|        2 | `**`                                                             | Exponentiation                                   | Right to left |
|        3 | `+x`, `-x`, `~x`                                                 | Unary plus, unary minus, bitwise NOT             | Right to left |
|        4 | `*`, `/`, `//`, `%`                                              | Multiplication, division, floor division, modulo | Left to right |
|        5 | `+`, `-`                                                         | Addition, subtraction                            | Left to right |
|        6 | `<<`, `>>`                                                       | Bitwise shifts                                   | Left to right |
|        7 | `&`                                                              | Bitwise AND                                      | Left to right |
|        8 | `^`                                                              | Bitwise XOR                                      | Left to right |
|        9 | `\|`                                                             | Bitwise OR                                       | Left to right |
|       10 | `in`, `not in`, `is`, `is not`, `<`, `<=`, `>`, `>=`, `==`, `!=` | Comparisons, membership, identity                | Left to right |
|       11 | `not`                                                            | Logical NOT                                      | Right to left |
|       12 | `and`                                                            | Logical AND                                      | Left to right |
|       13 | `or`                                                             | Logical OR                                       | Left to right |
|       14 | `if ... else`                                                    | Conditional expression                           | Right to left |
|       15 | `:=`                                                             | Assignment expression                            | Right to left |

## 2.3.4 SECTION SUMMARY

1. An **expression** is a combination of values (or variables, operators, calls to functions ‒ you will learn about them soon) which evaluates to a certain value, e.g., ```1 + 2```.

2. **Operators** are special symbols or keywords which are able to operate on the values and perform (mathematical) operations, e.g., the ```*``` operator multiplies two values: ```x * y```.

3. Arithmetic operators in Python: ```+``` (addition), ```-``` (subtraction), ```*``` (multiplication), ```/``` (classic division ‒ always returns a float), ```%``` (modulus ‒ divides left operand by right operand and returns the remainder of the operation, e.g., ```5 % 2 = 1```), ```**``` (exponentiation ‒ left operand raised to the power of right operand, e.g., ```2 ** 3 = 2 * 2 * 2 = 8```), ```//``` (floor/integer division ‒ returns a number resulting from division, but rounded down to the nearest whole number, e.g., ```3 // 2.0 = 1.0```)

4. A **unary** operator is an operator with only one operand, e.g., ```-1```, or ```+3```.

5. A **binary** operator is an operator with two operands, e.g., ```4 + 5```, or ```12 % 5```.

6. Some operators act before others - the **hierarchy of priorities**:

the ```**``` operator (exponentiation) has the highest priority;
then the unary ```+``` and ```-``` (note: a unary operator to the right of the exponentiation operator binds more strongly, for example ```4 **``` ```-1``` equals ```0.25```)
then: ```*```, ```/```, and ```%```,
and finally, the lowest priority: binary + and -.

7. Subexpressions in **parentheses** are always calculated first, e.g., ```15 - 1 * (5 * (1 + 2)) = 0```.

8. The **exponentiation** operator uses **right-sided binding**, e.g., ```2 ** 2 ** 3 = 256```.

# 2.4 - Variables
## 2.4.1 Variables – data-shaped boxes
Variables do not appear in a program automatically. As a developer, you must decide how many and which variables to use in your programs.

## 2.4.2 Variable names

If you want to give a name to a variable, you must follow some strict rules:

- the name of the variable must be composed of upper-case or lower-case letters, digits, and the character _ (underscore)

- the name of the variable must begin with a letter

- the underscore character is a letter

- upper and lower case letters are treated as different (a little differently than in the real world – Alice and ALICE are the same first names, but in Python they are two different variable names, and consequently, two different variables);

-the name of the variable must not be any of Python's reserved words

Python lets you use not only Latin letters but also characters specific to languages that use other alphabets.

Take a look at the list of words that play a very special role in every Python program.

```['False', 'None', 'True', 'and', 'as', 'assert', 'break', 'class', 'continue', 'def', 'del', 'elif', 'else', 'except', 'finally', 'for', 'from', 'global', 'if', 'import', 'in', 'is', 'lambda', 'nonlocal', 'not', 'or', 'pass', 'raise', 'return', 'try', 'while', 'with', 'yield']```

They are called keywords or (more precisely) reserved keywords. They are reserved because you mustn't use them as names: neither for your variables, nor functions, nor any other named entities you want to create.

The meaning of the reserved word is predefined, and mustn't be changed in any way.

## 2.4.3 How to create a variable

**Variable** = a name that refers to a value.

Example: 

Input:

```
var = 1
print(var)
```

Output:

```
1
```

## 2.4.4 How to use a variable
Create it → name it → use the name to access its value.

```
name = "John"   # create
print(name)     # use
```
## 2.4.5 How to assign a new value to an already existing variable

You can change the value of a variable by using the = sign again. Assignment creates or changes the value associated with a variable. So reassignment isn't necessarily "permanent"—you can always assign another value—but the variable itself only remembers its current value unless you stored the old value somewhere else.

Example:

```
age = 25
old_age = age

age = 26

print(age)      # 26
print(old_age)  # 25
```
## 2.4.8 Shortcut operators

| Shortcut  | Same as      | Meaning          |
| --------- | ------------ | ---------------- |
| `x += 5`  | `x = x + 5`  | Add 5            |
| `x -= 5`  | `x = x - 5`  | Subtract 5       |
| `x *= 5`  | `x = x * 5`  | Multiply by 5    |
| `x /= 5`  | `x = x / 5`  | Divide by 5      |
| `x %= 5`  | `x = x % 5`  | Get remainder    |
| `x **= 5` | `x = x ** 5` | Raise to a power |

# 2.5 Comments

A remark inserted into the program, which is **omitted at runtime**, is called a **comment**.
In Python, a comment is a piece of text that begins with a ```#``` (hash) sign and extends to the end of the line.

# 2.6 Interaction with the user
## 2.6.1 The input() function

The ```input()``` function allows your program to ask the user for information and receive their response.

```input()``` = **Input → Program receives information**.

One important thing, the ```input()``` returns the user's response as a string, even if they type a number.

For example:

```
age = input("How old are you? ")
```

If you enter 25, Python treats it as:


```"25"``` not: ```25```

If you actually need it as a number, you can convert it:

```
age = int(input("How old are you? "))
```

## 2.6.2 The input() function with an argument
The argument is called a prompt because it tells the user what information to enter.

Example: 

```
input("What is your name? ")
```

input() → the function
"What is your name? " → the argument
name → the variable that stores the user's response

## 2.6.3 The result of the input() function

The result of the input() function is a string.

This means that you mustn't use it as an argument of any arithmetic operation, e.g., you can't use this data to square it, divide it by anything, or divide anything by it.

## 2.6.4 The input() function – prohibited operations

Input() gives you text. If you want to perform mathematical operations on that input, you need to convert it to a number first.

**Common type conversions**
- String → Integer 
- String → Float
- Integer → String
- Integer → Float

## 2.6.6 More about input() and type casting


input() always gives you a string. input() gives you text. If you want to perform mathematical operations on that input, you need to convert it to a number first.

```
input()       → string
int(input())  → integer
float(input()) → float
```
## 2.6.5-6 Type casting (type conversions)

Type casting means converting a value from one data type to another.

## 2.6.7 String operators







