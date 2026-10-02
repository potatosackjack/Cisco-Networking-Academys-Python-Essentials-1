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

You can think of not as a ```Boolean switch```.

