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

### Inequality: the not equal to operator (!=)**

The ```!=``` (not equal to) operator compares the values of two operands, too. Here is the difference: if they are equal, the result of the comparison is ```False```. If they are not equal, the result of the comparison is ```True```.

🧠 My perspective: I really don't get the point of the inequality operator. I know it has importance and will probably will
show itself to be really useful in the future but as of right now it has be questioning why ever concept in code is black and white.

### Comparison operators: greater than**

```>``` (greater than) operator. 

The greater than operator ```>``` compares two values to determine whether the value on the left is greater than the value on the right.

It returns a **Boolean value**: It returns a **Boolean value**: It returns either ```True``` or ```False```.

### Comparison operators: greater than or equal to**

```>=``` (greater than or equal to).

The >= operator checks whether the value on the left is greater than OR equal to the value on the right.

It returns a **Boolean value**: It returns a **Boolean value**: It returns either ```True``` or ```False```.

### Comparison operators: less than**

```<``` (less than) operator.

The ```<``` operator checks whether the value on the **left is smaller than** the value on the right.

It returns a **Boolean value**: It returns a **Boolean value**: It returns either ```True``` or ```False```.

### Comparison operators: less than or equal to**

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

## 3.1.8-13 Analyzing code samples

# 3.1.4 Loops in Python











