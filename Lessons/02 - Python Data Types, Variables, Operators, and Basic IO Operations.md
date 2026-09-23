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


