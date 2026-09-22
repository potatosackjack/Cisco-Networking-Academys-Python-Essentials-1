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

1.Alphabet

The alphabet is the set of symbols that a language allows you to use.

In programming, this can include:

Letters: A-Z, a-z. 
Numbers: 0-9. 
Symbols: +, -, =, (,), etc.  

2.A Lexis

Lexis is the collection of words or basic elements that make up a language.

In Python, examples include:
- print
- if
- else
- while
- True

3.Syntax

Syntax is the set of rules for how those words and symbols must be arranged.

For example:  
print("Hello")

4.Semantics

Semantics refers to the meaning or behavior of correctly written code-in other words, what the code actually does when it is executed.

**1.1.4 Machine language vs. high-level language**

Machine language is the language the computer speaks at at it's core were talking 0 and 1 or better said binary. On the other hand we have high level languages that are computer languages still but they use more recognizable symbols and characters making giving the computer instructions to execute easier. 

*ChatGPT's Clarification: Machine language is the language a computer's processor executes at its core. It is represented as binary data—ultimately patterns of 0s and 1s. On the other hand, we have high-level programming languages, which are still languages for giving computers instructions, but they use more recognizable words, symbols, and conventions. This makes it much easier for humans to write and understand instructions that the computer can eventually execute.*

Machine language:

Computer-oriented → difficult for humans to read → binary instructions

High-level language:

Human-oriented → easier for humans to read/write → eventually translated into lower-level instructions

A program written in a high-level programming language is called a **source code** (in contrast to the machine code executed by computers). Similarly, the file containing the source code is called the **source file**.

Source code = the code itself.
Source file = the file containing the code.

🆘**1.1.5 Compilation vs. Interpretation**

Computers have two different ways of transforming a program from a high-level programming language into machine language:

**Compilation**
A compiler takes your source code and translates it into another form—often machine code—before the program runs.

Think:
Your source code → Compiler → Machine code →  Computer

**Interpretation**
An interpreter reads your source code and performs the instructions through an interpreter while the program is running.

Think:
Your source code → Interpreter → Executes it → Computer+

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
pritn("Hello")

*Your editor might immediately put a red underline under pritn.*

*Then, when you actually run the program, Python's interpreter may produce:*

NameError: name 'pritn' is not defined

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

Notes...

## 1.3. Section 3 - Downloading and Installing Python

Notes...

## 1.4. Module 1 Completion Module Test

Notes...
