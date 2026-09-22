## Expectations

At this point, I've already begun the modules and have made it to the middle of Module 2. However, I can still reflect on what I expected when starting Module 1.

I expected Python's syntax to be a lot like JavaScript, but so far, Python seems to be much simpler.

I'm getting ahead of myself by talking about Module 2, though. Keeping my expectations focused on the topics covered in Module 1, I had already tried downloading Python before, so some of that information was somewhat familiar to me.

However, I didn't know about Dutch programmer **Guido van Rossum**, who created Python, or how adaptable he designed the language to be.
  
# 1.0. Welcome to Python Essentials 1

Syllabus:

- the universal concepts of computer programming. 
- the syntax and semantics of the Python language. 
- practical skills in resolving typical implementation challenges. 
- how to use the most important elements of the Python Standard Library. 
- how to install your runtime environment. 
- how to design, develop, test, and debug simple Python programs.    

The four modules:

**Module 1:**
Introduction to Python and computer programming

**Module 2:**
Data types, variables, basic input-output operations, and basic operators

**Module 3:**
Boolean values, conditional execution, loops, lists and list processing, logical and bitwise operations

**Module 4:**
Functions, tuples, dictionaries, exceptions, and data processing.

## 1.1. Section 1 Introduction to Programming
**1.1.1 How does a computer program work?**
My understanding: Computers don't inherently know they are doing but are able to calculate and give outputs based on the level of their program. 

*ChatGPT's Clarification:
Computers don't inherently understand what they're doing, but they can calculate and produce outputs based on the instructions provided by a program.*

The important distinction is “understand” vs. “execute.” Another name for a programming language is executable 

Perspective a. A program is a set of instructions that the computer executes (carries out).
Perspective b. Programs contain instructions that a computer executes to perform tasks and produce outputs.

Program: “Computer, display Hello.”
Computer: executes that instruction → Hello

**1.1.2 Natural languages vs. programming languages**

Computers have their own language called machine language

A complete set of known commands is called an **instruction list**, sometimes abbreviated to **IL**
↳ Different types of computers may vary depending on the size of their ILs, and the instructions could be completely different in different models. (Ties into 1.1.1)


**1.1.3 What makes a language?**
The four elements that make up a language 

1. Alphabet

The alphabet is the set of symbols that a language allows you to use.

In programming, this can include:

Letters: A-Z, a-z. 
Numbers: 0-9. 
Symbols: +, -, =, (,), etc.  

2. A Lexis

Lexis is the collection of words or basic elements that make up a language.

In Python, examples include:
```
print  
if  
else  
while  
True  
```
3. Syntax

Syntax is the set of rules for how those words and symbols must be arranged.

For example:  
```
print("Hello")
```

4. Semantics

Semantics refers to the meaning or behavior of correctly written code-in other words, what the code actually does when it is executed.

**1.1.4 Machine language vs. high-level language**

Machine language is the language the computer speaks at at it's core were talking 0 and 1 or better said binary. On the other hand we have high level languages that are computer languages still but they use more recognizable symbols and characters making giving the computer instructions to execute easier. 

*ChatGPT's Clarification: Machine language is the language a computer's processor executes at its core. It is represented as binary data—ultimately patterns of 0s and 1s. On the other hand, we have high-level programming languages, which are still languages for giving computers instructions, but they use more recognizable words, symbols, and conventions. This makes it much easier for humans to write and understand instructions that the computer can eventually execute.*

Machine language:

```
Computer-oriented → difficult for humans to read → binary instructions
```
High-level language:

```
Human-oriented → easier for humans to read/write → eventually translated into lower-level instructions
```

A program written in a high-level programming language is called a **source code** (in contrast to the machine code executed by computers). Similarly, the file containing the source code is called the **source file**.

Source code = the code itself.
Source file = the file containing the code.

🆘**1.1.5 Compilation vs. Interpretation**

Computers have two different ways of transforming a program from a high-level programming language into machine language:

**Compilation**
A compiler takes your source code and translates it into another form—often machine code—before the program runs.

Think:
```
Your source code → Compiler → Machine code →  Computer
```

**Interpretation**
An interpreter reads your source code and performs the instructions through an interpreter while the program is running.

Think:
```
Your source code → Interpreter → Executes it → Computer
```

**1.1.6 What does the interpreter do?**

The interpreter reads the source code in a way that is common in Western culture: from top to bottom and from left to right. There are some exceptions

If the compiler finds an error, it finishes its work immediately. The only result in this case is an error message. (Ties to 1.1.5)

The interpreter will inform you where an error is located and what caused it. However the messages may be misleading because an interpreter isn't able to follow intentions so while it detects errors it may miss their real cause. 

For example if you try to use a function that does exist in a high level language it may show you an the error but it wont show you what you intended to use in that space.  

*ChatGPT's Clarification:An interpreter can identify and report errors in a program, often indicating where the error occurred and providing information about what went wrong. However, its error messages can sometimes be misleading because the interpreter cannot know the programmer's intentions. It can identify the problem it encounters, but it may not be able to identify the underlying mistake that caused it.*

In confusion I asked ChatGPT if the built-in interpreter is the red highlights for errors in side the code editor?

*ChatGPT's Clarification: The red highlights you see in a code editor are usually produced by the editor's syntax checker, linter, or language-analysis tools. They're not necessarily the Python interpreter itself.*

*Think of it as two related things:*

1. Code editor
*Looks at your code and can warn you about problems while you're typing.*

2. Python interpreter
*Actually processes and executes your Python program when you run it.*

For example:
```
pritn("Hello")
```

*Your editor might immediately put a red underline under pritn.*

*Then, when you actually run the program, Python's interpreter may produce:*

```
NameError: name 'pritn' is not defined
```

So:

🔴 *Red underline: “Hey, I think there's a problem here.”*  
▶️ *Interpreter: “I actually tried to execute this and here's the error I encountered.”*


**1.1.7 Compilation vs. Interpretation – Advantages and Disadvantages**

**Compilation**

A compiler translates the source code into another form, often machine code, before the program is executed.

**Advantages:**

The program can run efficiently after compilation.
Many errors can be detected before the program runs.
The compiled program can often run without needing the original source code.

**Disadvantages:**

You generally have to compile the program before running it.
Compilation can take time, especially for large programs.
The resulting program may need to be compiled separately for different computer architectures.

**Interpretation**

An interpreter processes and executes the program through an interpreter during execution.

**Advantages:**

You can often run code immediately without creating a separate executable first.
Errors can be identified as the program reaches the problematic code.
It can make testing and experimenting with code convenient.

**Disadvantages:**

Execution can involve additional processing by the interpreter.
You need the appropriate interpreter/runtime available to execute the program.
An error may not be discovered until the program reaches the problematic instruction.
Simple way to remember

**Compilation:** Translate first → execute afterward.
**Interpretation:** Process/execute through the interpreter as the program runs.

## 1.2. Section 2 Introduction to Python
**1.2.1 Python – a tool, not a reptile**

Python is a widely-used, interpreted(Ties in 1.1.5-1.1.7), object-oriented, and high-level programming language with dynamic semantics, used for general-purpose programming.

Python programming language comes from an old BBC television comedy sketch series called **Monty Python's Flying Circus**.

**1.2.2 Who created Python?**
Guido van Rossum

**1.2.3 A hobby programming project**
December 1989 Guido van Rossum was looking for a "hobby" programming project that would keep me occupied during the week around Christmas.  
↳Python was created in attempt to write a new scripting language that would appeal to Unix/C hackers 

In 1999, Guido van Rossum defined his goals for Python:
  - easy and intuitive
  - open source
  - understandable
  - suitable for everyday tasks

**1.2.4 What makes Python so special?**
  - easy to learn
  - easy to teach
  - easy to use
  - easy to understand
  - easy to obtain, install and deploy
  - 🏷️FREE

**1.2.5 Python rivals?**
**Perl** – a scripting language originally authored by Larry Wall;
**Ruby** – a scripting language originally authored by Yukihiro Matsumoto.

**1.2.6 Where can we see Python in action?**
🧠 My honest perspection: Python can be found being used on the backend of computer programs and used to control devices. 

It's used extensively to implement complex Internet services like search engines, cloud storage and tools, social media and so on

*ChatGPT's Clarification:*
*- Web development — Building websites, web applications, and backend services.*  
*- Data analysis — Processing, organizing, and analyzing large amounts of data.*  
*- Artificial intelligence and machine learning — Developing AI models and applications.*  
*- Automation — Automating repetitive tasks, file management, data entry, and workflows.*  
*- Scientific computing — Performing calculations, simulations, and research.*  
*- Cybersecurity — Creating security tools, analyzing data, and automating security tasks.*  
*- Networking — Automating network configuration, monitoring systems, and working with network devices.*  
*- Software development — Creating desktop applications, tools, and utilities.*  
*- Game development — Creating games and game-related tools, particularly with libraries such as Pygame.*  
*- Web scraping — Collecting information from websites programmatically.*  
*- Database management — Connecting to, reading, modifying, and organizing database information.*  
*- Education — Teaching programming and computer science because Python's syntax is relatively accessible.*  
*- Finance and business — Analyzing financial data, automating processes, and building analytical tools.*  
*- DevOps and cloud computing — Automating deployments, infrastructure tasks, and system administration.*  
*- Internet of Things (IoT) — Programming and controlling certain devices and embedded systems.*  

**1.2.7 Why not Python?**
- low-level programming (Python can work with low-level languages, but Python is not designed to be a low-level language.)

*ChatGPT's Clarification: Python isn't well suited for low-level programming, rather than saying Python cannot interact with low-level languages.*

  languages such as C, C++, and Assembly give programmers much more direct control over things like:
  - Memory
  - CPU instructions
  - Hardware resources
  - Pointers and memory addresses
  - Operating-system interfaces
  - Performance optimization

- applications for mobile devices
Python has additional runtime overhead compared with languages designed for native mobile development. That extra layer isn't automatically terrible, but it can make Python less attractive for performance-sensitive mobile applications.

Python is also commonly used behind mobile apps—for example, a mobile app might communicate with a Python backend.

Simple takeaway: Python is a very high-level, general-purpose language. That makes it excellent when you want to accomplish things without dealing with lots of low-level details—but those same abstractions can make it less suitable when you need maximum hardware control, native integration, or performance.

**1.2.8 There is more than one Python**
There are two main kinds of Python, called Python 2 and Python 3.
Python 2 is an older version of the original Python.
These two versions of Python aren't compatible with each other.

Python 3 isn't just a better version of Python 2 – it is a completely different language, although it's very similar to its predecessor. When you look at them from a distance, they appear to be the same, but when you look closely, though, you notice a lot of differences.

**1.2.9 Python implementations**

🧠 My honest perception: A python implementation is a software language or translator. (However this WRONG)

*ChatGPT's Clarification: A Python implementation is software that acts as a translator and execution environment for programs written in Python*

🆘**Examples of Implementations**
| Name            | What it is                | Main idea                                              |
| --------------- | ------------------------- | ------------------------------------------------------ |
| **CPython**     | Python implementation     | Standard Python implementation, written primarily in C |
| **PyPy**        | Python implementation     | Python implementation featuring JIT technology         |
| **Jython**      | Python implementation     | Python for the Java/JVM ecosystem                      |
| **MicroPython** | Python implementation     | Python for microcontrollers/constrained devices        |
| **Cython**      | Language/compiler project | Python-like code compiled to C/C++                     |

## 1.3. Section 3 - Downloading and Installing Python

https://www.python.org/downloads/

To start your work, you need the following tools:
- editor
- console
- debugger

Besides its many useful components, the Python 3 standard installation contains a very simple but extremely useful application named **IDLE (Integrated Development and Learning Environment**).

IDLE opens a new window use to write and amend your code.

That window is the **editor window**. Its only purpose is to be a workplace in which your source code is treated. Do not confuse the editor window with the shell window. They perform different functions.

When you open IDLE, you can use: 
1. The Shell — This is where you can interact with Python immediately:  

```
>>> 2 + 2  
4
>>> print("Hello")    
Hello
```

2. The Editor — That's where you write an entire Python program:  

```
name = "John"
age = 25

print(name)
print(age)
```

🧠 My honest perception: lets say I download VS Code and then open a .py file, where is IDLE in that process?

*ChatGPT's Clarification: IDLE isn't automatically involved at all if you're using VS Code.*

```
Option A:
VS Code → CPython → Your program

Option B:
IDLE → CPython → Your program
```

Both VS Code and IDLE can provide an environment for writing and running Python, but they're different tools. VS Code and IDLE are development tools/editors. CPython is the Python implementation that actually provides the machinery for running Python code.


## 1.4. Module 1 Completion Module Test

First attempt: 70%
Second attempt: 80%
