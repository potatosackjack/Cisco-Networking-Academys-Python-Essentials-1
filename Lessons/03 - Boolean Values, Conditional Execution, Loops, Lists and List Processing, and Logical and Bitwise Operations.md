## Expectations 

I still haven't written a program that can be sold as a SaaS product, so with that said, I'm still in it.

The topics for this module are Boolean Values, Conditional Execution, Loops, Lists and List Processing, and Logical and Bitwise Operations. Out of all of those, the only topic I feel like I've seen before is Boolean.

I've skimmed across topics like conditionals and loops before, but not enough to say that I could explain them to someone else.

Overall, I'm a little nervous to dive in. In the last module, there were a few topics that held me up and required me to watch a few YouTube videos, but overall, I seemed to get the big picture.

I'm expecting this module to challenge me, but I'm still in it and looking forward to seeing how much of it I can actually understand and retain.

# 3.0. Making decisions in Python

## Module 3.0 — Section Summary

**1. Boolean Values & Logical Operations**

**Boolean Values:** `True` and `False` are Boolean data types.
**Comparison Operators:** Used to compare values, such as `==`, `!=`, `<`, `>`, `<=`, and `>=`.
**Logical Operators:** Used to combine or reverse conditions, such as `and`, `or`, and `not`.

**2. Conditional Execution**

**`if` Statements:** Run code when a condition is `True`.
**`else` Clauses:** Run code when the `if` condition is `False`.
**`elif` Branches:** Check additional conditions when previous conditions are `False`.

**3. Loops (Iteration)**

**`while` Loops:** Repeat a block of code as long as a condition remains `True`.
**`for` Loops:** Repeat a block of code for each item in a sequence, such as a list or range of numbers.
**Loop Control:** `break` exits a loop, while `continue` skips the current iteration and moves to the next one.

**4. Lists & List Processing**

**Creating Lists:** Collections of items are stored inside square brackets `[]`.
**Indexing & Slicing:** Used to access individual elements or sections of a list.
**List Methods:** Used to add, remove, or modify items in a list, such as `.append()`, `.insert()`, and `.pop()`.

**5. Bitwise Operations**

**Bitwise Operations:** Work directly with the binary representation of integers.
Common bitwise operators include `&` (**AND**), `|` (**OR**), `^` (**XOR**), `~` (**NOT**), `<<` (**left shift**), and `>>` (**right shift**).

*Google Gemini*

## 3.1.1 Questions and answers

Computers ultimately operate using binary information. Computers can absolutely do much more than this now, 
especially with AI but Ttaditional programs make decisions by evaluating conditions and reacting to the result

Program asks a question
        ↓
Computer evaluates it
        ↓
True or False
        ↓
Program reacts

## 3.1.2 Comparison: equality operator

The **equality operator** ```==``` compares two values to see if they are equal.
It is a binary operator with left-sided binding. It needs two arguments and checks if they are equal.

It produces a **Boolean value**:

**True** → the values are equal.
**False** → the values are not equal.

The equality operator ```==``` isn't to be confused with the equal operator ```=```.

```=``` assigns a value.
```==``` asks whether two values are equal.

## 3.1.3 Exercises

```2 == 2``` is ```True```.

2 is equal to 2. Python will answer True.

```2 == 2.``` is ```True```.

Python is able to convert the integer value into its real equivalent, and consequently, the answer is True.

```1 == 2``` is ```False```.

The answer will be (or rather, always is) False.

## 3.1.4 Operators

### Equality: the equal to operator (==)

The ```==``` (equal to) operator compares the values of two operands. If they are equal, the result of the comparison is ```True```. If they are not equal, the result of the comparison is ```False```.

### Inequality: the not equal to operator (!=)

The ```!=``` (not equal to) operator compares the values of two operands, too. Here is the difference: if they are equal, the result of the comparison is ```False```. If they are not equal, the result of the comparison is ```True```.

🧠 My perspective: I really don't get the point of the inequality operator. I know it has importance and will probably will
show itself to be really useful in the future but as of right now it has be questioning why ever concept in code is black and white.

### Comparison operators: greater than

```>``` (greater than) operator. 

The greater than operator ```>``` compares two values to determine whether the value on the left is greater than the value on the right.

It returns a **Boolean value**: It returns a **Boolean value**: It returns either ```True``` or ```False```.

### Comparison operators: greater than or equal to

```>=``` (greater than or equal to).

The >= operator checks whether the value on the left is greater than OR equal to the value on the right.

It returns a **Boolean value**: It returns a **Boolean value**: It returns either ```True``` or ```False```.

### Comparison operators: less than

```<``` (less than) operator.

The ```<``` operator checks whether the value on the **left is smaller than** the value on the right.

It returns a **Boolean value**: It returns a **Boolean value**: It returns either ```True``` or ```False```.

### Comparison operators: less than or equal to

```<=``` (less than or equal to).

The ```<=``` operator checks whether the value on the left is **less than OR equal** to the value on the right.

It returns a **Boolean value**: It returns either ```True``` or ```False```.

## Python Operator Priority

| Priority | Operator(s)          | What it does                                        | Example          |
| -------: | -------------------- | --------------------------------------------------- | ---------------- |
|        1 | `()`                 | Parentheses                                         | `(2 + 3)`        |
|        2 | `**`                 | Exponentiation                                      | `2 ** 3`         |
|        3 | `+x`, `-x`           | Unary plus/minus                                    | `-5`             |
|        4 | `*`, `/`, `//`, `%`  | Multiplication, division, floor division, remainder | `10 * 2`         |
|        5 | `+`, `-`             | Addition, subtraction                               | `10 - 3`         |
|        6 | `<`, `<=`, `>`, `>=` | Comparisons                                         | `5 >= 3`         |
|        7 | `==`, `!=`           | Equal / not equal                                   | `5 == 5`         |
|        8 | `not`                | Logical NOT                                         | `not True`       |
|        9 | `and`                | Logical AND                                         | `True and False` |
|       10 | `or`                 | Logical OR                                          | `True or False`  |


## 3.1.7 Making use of the answers

```if```, ```if-else```, and ```elif``` Statements
These are all ways to make Python make decisions based on conditions.

Once Python finds a true condition, it executes that block and doesn't continue checking the remaining elif/else blocks.

```
if       → check the first condition
elif     → check another condition
else     → if none of the conditions were true
```

**IF → ELSE IF → OTHERWISE**

# 3.2.0 Loops in Python
## 3.2.1 Looping your code with while

A ```while``` loop repeatedly executes instructions as long as a condition is true

The ```while``` structure basically says: 

```
WHILE this is true:
    DO this
    DO this
    DO this
    check again
```

A while loop generally follows this cycle:

```
Check condition
      ↓
   True?
   ↙    ↘
 Yes     No
  ↓       ↓
Run      Stop
code
  ↓
Update variable
  ↓
Check condition again
```

The condition is checked before every iteration, ```while``` loops are sometimes described as condition-controlled loops.
The loop continues while the condition is ```True``` and stops when the condition becomes ```False```.

## 3.2.2 An infinite loop

An infinite loop, also called an ```endless loop```, is a loop that never reaches a ```False``` condition.


A while infinite loop generally follows this cycle:

```
Check → True → Run → Check → True → Run → Check → True → ...
```

Generally something inside the loop needs to make progress toward the stopping condition..

## 3.2.3 The while loop: more examples

Example:

```
count = 1

while count <= 5:
    print(count)
    count += 1
```

Here's what happens:

1. ```count``` starts at ```1```.
2. Python **checks the condition**: count ```<= 5```.
3. Since it is ```True```, Python runs the loop body.
4. ```count``` increases by ```1```.
5. Python checks the condition again.
6. This continues until ```count <= 5``` becomes ```False```.

A ```while``` loop keeps running while its condition is ```True```.

## 3.2.5 Looping your code with ```for```

The ```for``` Loop in Python allows you to repeat code for each item ```in``` a collection or sequence. ```for``` is a built in Python keyword and a reserved word used to create a for loop, which allows you to iterate over a sequence (such as a list, tuple, dictionary, set, or string) or any other iterable object.

Example: 

Input:

```
names = ["James", "Sarah", "Mike", "Lisa", "John"]

for name in names:
    print("Hello", name)
```

Output: 

```
Hello James
Hello Sarah
Hello Mike
Hello Lisa
Hello John
```

Instead of writing print() five separate times, the for loop handles the **repetition** for you. Because it is a keyword, you cannot use it as a variable name, function name, or any other identifier in your code.


🔑 My perspective: Not really mention in the chapter in detail but the ```in``` keyword is used as a membership operator. It checks if a value exists within a collection (like a list, string, tuple, set, or dictionary), or to iterate over a sequence within a for loop.

The Two Main Ways in is Used: 

1. Membership Testing (As an Operator)

When used between an element and a collection, it acts as a boolean operator. It returns True if the item is present and False if it is not.

```
# Checking a list
fruits = ["apple", "banana", "cherry"]
print("banana" in fruits)  # Output: True

# Checking a string (substring search)
print("cat" in "caterpillar")  # Output: True
```

*Note: You can also combine it with not to check for absence (not in).*

2. When paired with a for statement, in is used to sequentially step through each item in an iterable.

```
# Iterating over a sequence
for number in [1, 2, 3]:
    print(number)
```

While in looks for containment (whether something is inside a group), Python also has a separate keyword named is, which checks for object identity (whether two variables point to the exact same place in computer memory).

## 3.2.6 More about the ```for``` loop and the ```range()``` function with three arguments

A ```for``` loop is like a conveyor belt:


        ITEMS
          ↓
     ┌──────────┐
     │   ITEM 1 │ → perform action
     └──────────┘
          ↓
     ┌──────────┐
     │   ITEM 2 │ → perform action
     └──────────┘
          ↓
     ┌──────────┐
     │   ITEM 3 │ → perform action
     └──────────┘
          ↓
        DONE


```range```() has three parts:

```
range(start, stop, step)
```


Example:

```
range(2, 8, 3)
```

Part | Value | Meaning |
--- | --- | --- |
start | 2 | Start counting at 2 |
stop |8 | Stop before reaching 8 |
step | 3 | Add 3 each time

So Python generates:

```2 → 5 → 8```

But 8 is not included, because the **stop value is exclusive**.

Therefore, i takes these values:

```
i = 2
i = 5
```

## 3.2.8 The break and continue statements

```break``` → stop the entire loop.

```continue``` → skip the rest of the current iteration and start the next one.

```break``` – exits the loop immediately, and unconditionally ends the loop's operation; the program begins to execute the nearest instruction after the loop's body;

```continue``` – behaves as if the program has suddenly reached the end of the body; the next turn is started and the condition expression is tested immediately.

Both are Python keywords.

# 3.3.0 Logic and bit operations in Python

## Computer logic

Computer logic deals with the conjunction ```and``` and the disjunction ```or```. Both are called **logical operators** and are Python keywords. The and conjunction requires both conditions to be ```True```, while the or disjunction requires at least one condition to be ```True```.

```and``` → BOTH must be true:

```
True and True   → True
True and False  → False
False and True  → False
False and False → False
```

or → AT LEAST ONE must be true:

```
True or True   → True
True or False  → True
False or True  → True
False or False → False
```

Terminology point: **conjunction** and **disjunction** describe the logical operations; and and or are the Python keywords/operators that perform them.

The ```not``` operator is a Python logical operator that reverses the truth value of a condition.

The ```not``` operator reverses a Boolean value or the result of a condition. If the result is ```True```, not makes it ```False```; if the result is ```False```, not makes it ```True```.

| Original value | Apply `not` | Result  |
| -------------- | ----------- | ------- |
| `True`         | `not True`  | `False` |
| `False`        | `not False` | `True`  |

You can think of not as a ```Boolean switch```. Each time not is applied, it flips the Boolean value.

## 3.3.2 Logical expressions

There are two common relationships called De Morgan's laws:


```not (A and B)``` is equivalent to: ```(not A) or (not B)```

And:

```not (A or B)```is equivalent to: ```(not A) and (not B)```

Simple takeaway: not reverses the entire logical result when placed before a pairwise expression such as (A and B) or (A or B).

```
        AND / OR
           ↓
   True or False
           ↓
          NOT
           ↓
   opposite result
```

## 3.3.3 Logical values vs. single bits

Logical operators (```and```, ```or```, and ```not```) evaluate values as a whole rather than operating on individual bits. Bitwise operators, in contrast, operate on individual bits.

| Type        | Operators          | How they work                          |                             
| ----------- | ------------------ | -------------------------------------- |
| **Logical** | `and`, `or`, `not` | Treat values/conditions as a **whole** |                        
| **Bitwise** | `&`, `, `^`, `~`   | Work on **individual bits**            |

## 🆘 3.3.4 Bitwise operators

There are four operators that allow you to **manipulate single bits of data**. They are called **bitwise operators**.

Here are all of them:

- & (ampersand) ‒ bitwise conjunction;
- | (bar) ‒ bitwise disjunction;
- ~ (tilde) ‒ bitwise negation;
- ^ (caret) ‒ bitwise exclusive or (xor).

**& — Bitwise AND**

The ```&``` operator produces ```1``` only when both corresponding bits are ```1```.

| A | B | A `&` B |
| - | - | ------- |
| 0 | 0 | 0       |
| 0 | 1 | 0       |
| 1 | 0 | 0       |
| 1 | 1 | **1**   |

**| — Bitwise OR**

The ```|``` operator produces ```1``` when at least one of the corresponding bits is ```1```.

| A | B | A ```\|``` B |
|---|---|---|
| 0 | 0 | 0 |
| 0 | 1 | 1 |
| 1 | 0 | 1 |
| 1 | 1 | 1 |

**^ — Bitwise XOR**

```^``` means **exclusive OR**. It produces 1 when the two corresponding bits are different.

| A | B | A `^` B |
| - | - | ------- |
| 0 | 0 | 0       |
| 0 | 1 | **1**   |
| 1 | 0 | **1**   |
| 1 | 1 | 0       |

Bitwise operators work on the individual bits of integer values.

**Bitwise Operation: ```~``` — Bitwise NOT**

The ```~``` operator is called **bitwise NOT**. Unlike ```&```, ```|```, and ```^```, it works with **one integer at a time**.

It **flips every bit**:

- 0 becomes 1
- 1 becomes 0

Summary: 

| Operator | Name        | What it does                      |                                    |
| -------- | ----------- | --------------------------------- | ---------------------------------- |
| `&`      | Bitwise AND | `1` if **both** bits are `1`      |                                    |
| `        | `           | Bitwise OR                        | `1` if **at least one** bit is `1` |
| `^`      | Bitwise XOR | `1` if the bits are **different** |                                    |
| `~`      | Bitwise NOT | **Flips every bit**               |                                    |

## 🆘 3.3.5 How do we deal with single bits?

## 🆘 3.3.6 Binary left shift and binary right shift

The shift operators are essentially ways of manipulating an integer by moving its binary digits rather than directly performing multiplication or division.

| Operator | Name        | Direction | Basic effect            |
| -------- | ----------- | --------- | ----------------------- |
| `<<`     | Left shift  | ←         | Multiply by powers of 2 |
| `>>`     | Right shift | →         | Divide by powers of 2   |

Example:

```
20 >> 1
```

Binary:

```
20 = 10100

10100 >> 1
       ↓
01010
```

01010 is 10 in decimal. 


# 3.4.0 Lists
## 3.4.1 Why do we need lists?

A **list** lets you store multiple values together in one variable.

Example:

```
List: [10, 20, 30, 40]

1st cycle → number = 10 → print(10)
2nd cycle → number = 20 → print(20)
3rd cycle → number = 30 → print(30)
4th cycle → number = 40 → print(40)
             ↓
          List ends
```

Python lists can store almost any type of value:

Numbers: ```numbers = [10, 20, 30, 40]```   
Strings: ```names = ["John", "Sarah", "Mike"]```  
Booleans: ```answers = [True, False, True, True]```   
Python lists can store a mixture of types: ```items = ["John", 25, True, 3.14]```   
Lists can even contain other lists:  

```
students = [
    ["John", 20],
    ["Sarah", 22],
    ["Mike", 19]
]
```

Lists become especially useful when you have many pieces of related data that you want to work with using loops, indexing, adding/removing items, etc.

A **list** can hold as many values as your computer's available memory allows.

## 3.4.2 Indexing lists

Lists are written inside square brackets `[]`. The individual items inside the brackets are called **elements**.

Each element has an **index**, which identifies its position in the list. Python uses **zero-based indexing**, meaning the first element has an index of `0`.

The indexes increase from left to right. For example:

```python
numbers = [10, 20, 30, 40]
```

```text
Element:  10    20    30    40
Index:     0     1     2     3
```

The basic format of a list is to give the list a variable name, followed by `=`, and then place the elements inside square brackets:

```python
variable_name = [element1, element2, element3]
```

## 3.4.3 Accessing list content 

**Accessing elements**

To access an element in a **list**, use its **index** inside square **brackets** after the list's variable name.

For example:

```
numbers = [10, 20, 30, 40]

print(numbers[0])
```

Output:

```10```

Because the first **element** has an **index** of "0", "numbers[0]" accesses the first element.

```
print(numbers[1])  # 20
print(numbers[2])  # 30
print(numbers[3])  # 40
```

Remember: The ```index``` tells Python which **element** you want to access.

🔑 The ```len()```function takes the list's name as an argument, and returns the number of elements currently stored inside the list (in other words ‒ the list's length).


## 3.4.4 Removing elements from a list

**Removing elements**

Elements can be removed from a list in several ways.

Using ```del```

The ```del``` statement can remove an element by its index:

```
numbers = [10, 20, 30, 40]
del numbers[1]
  
print(numbers)
```
  
Output:  
  
```
[10, 30, 40]
```

The element "20" was removed because it was at index "1".

You can also use a **negative index**:

```
del numbers[-1]
```

This removes the last element.

Using **.remove()**
  
The ```.remove()``` method removes an element by its value rather than its index:

```
numbers = [10, 20, 30, 40]
numbers.remove(20)

print(numbers)
```

Output: ```[10, 30, 40]```

Here, Python searches for the value "20" and removes it.

Remember:

- del numbers[1]" → removes the element at index 1
- numbers.remove(20)" → removes the element with the value 20

```.remove()``` only removes the first matching **element** it finds, starting from the left.

If you want to remove every occurrence of a particular value, you can use a while loop with ```.remove()```:


```
numbers = [10, 20, 30, 20, 40, 20]

while 20 in numbers:
    numbers.remove(20)

print(numbers)

```

Output: ```[10, 30, 40]```

## 3.4.5 Negative indices are legal

**Negative indexes**

Python also allows you to use negative indexes to access elements starting from the end of the list.

The last element has an index of "-1", the second-to-last has an index of "-2", and so on.

**Element**:   10     20     30     40
**Index**:      0      1      2      3
**Negative**:  -4     -3     -2     -1

For example:

```
print(numbers[-1])  # 40
print(numbers[-2])  # 30
print(numbers[-3])  # 20
print(numbers[-4])  # 10
```

So:

- "numbers[0]" → first element
- "numbers[3]" → last element
- "numbers[-1]" → last element
- "numbers[-2]" → second-to-last element

Remember: Positive indexes count from the beginning, while negative indexes count from the end.

## 3.4.7 Functions vs. methods

**Methods** are technically functions that are associated with an object/class. As a beginner, however, the easiest distinction to remember is:

|  | Function | Method |
|--- | --- | --- |
| Called by | Its name | An object + |
| Example | len(numbers) | numbers.remove(20) |
| Associated with | General operation |A particular object/type |

## 3.4.8 Adding elements to a list: ```append()``` and ```insert()``` 

Python provides list methods for adding elements to an existing list. Two important ones are ```.append()``` and ```.insert()```.

 ```.append()``` vs. ```.insert()```

| Method | What it does |
|--------|--------------|
| append(x) |Adds x to the end of the list |
| insert(i, x) | Adds x at index i         |

Easy way to remember:  

```.append()``` → add to the end     
```.insert()``` → add at a specific position  

## 3.4.9 Making use of lists

A list is useful because it allows you to treat multiple related values as one collection.

You can then:

- Access individual elements
- Change elements
- Add elements
- Remove elements
- Loop through the elements
- Process the collection as a whole

That's what makes lists so useful for things like sorting numbers, storing names, keeping track of scores, and processing data.

Example: 

```
my_list = [10, 1, 8, 3, 5]
total = 0

for i in range(len(my_list)):
    total += my_list[i]

print(total)
```

# 3.5 Sorting simple lists: the bubble sort algorithm
## 3.5.1 The bubble sort

Bubble sort compares neighboring elements and swaps them when they are in the wrong order.

**The basic idea**

```
Compare neighboring elements
        ↓
Are they in the wrong order?
        ↓
     Yes → Swap them
        ↓
Move to the next pair
        ↓
Repeat
```

## 3.5.2 Sorting a list



