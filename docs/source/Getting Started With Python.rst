Getting Started With Python
===========================

.. role:: java(code)
  :language: java

.. role:: c(code)
  :language: c

.. role:: python(code)
  :language: python

**By the end of this section, students should be able to:**

- Understand variables, their types, and how to use them in Python
- Use if..elif...else statement to specify certain conditions for running code
- Differentiate between for and while loops
- Learn the common naming, indentation, and commenting practices when coding in Python
- Appreciate the importance of following coding conventions and practices in every project

Syntax
------

The syntax is the rules that define how statements are created in a programming language. As stated before, Python syntax is usually straightforward and intuitive. Some statements in Python may look similar to those in other languages like Java and C; however, Python simplifies coding much more.

For example, the following statements do the same function but in different languages. They all output “Hello World!” to the terminal if a variable (explained later) is equal to 1.

**Java**

.. code-block:: java

  if (x == 1){
  	System.out.print(“Hello World!”);
  }

**C**

.. code-block:: c

  if (x == 1){
  	printf(“Hello World!”);
  }

**Python**

.. code-block:: python

  if x == 1:
  	print(“Hello World!”)

Notice how the print statement ends in a semicolon (;) in both Java and C. One of the main features of Python syntax that sets it apart is that it does not use a symbol to denote the termination of an instruction. Also, unlike most languages, where code blocks are wrapped in curly braces (notice the if statement syntax), Python relies on indentation to define which block a statement belongs to. Indentation, which is always encouraged to use in other languages, is required in Python and contributes to the readability of Python scripts.

The following subsections go through the syntax of the most common python statements.

Variables
^^^^^^^^^

Variables are reserved memory spaces defined by the programmer to hold a specific value. The value can be a number, a character, text, or an object (refer to the introduction part for more information about object-oriented programming). In many languages, the type of the variable needs to be explicitly defined when declaring that variable. However, Python automatically decides the variable type when it is assigned a value.

In this example, variable a is an integer, b is a floating value, and c is a string of text. The value on the right side of the = operator is assigned the variable (operand) on the left side. Notice how keywords (int, float, and String in other languages) are not used to specify the data type

.. code-block:: python

  a = 2021
  b = 3.14
  c = “Hello World!”

The video below discusses Python variables with more examples.

.. raw:: html

  <iframe width="560" height="315" src="https://www.youtube.com/watch?v=cQT33yu9pY8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Conditions
^^^^^^^^^^

Conditions are statements that allow the programmer to decide which commands to run based on certain criteria. Conditions in Python are defined using the “if” statement, which can be used standalone to make a decision. “else” and “elif” keywords can be used to extend an “if” statement.

.. code-block:: python

  grade = 78

  if grade > 90:
  	print(“Excellent”)
  elif grade < 90 and grade > 50:
  	print(“Passed”)
  else:
  	print(“Failed”)

Elif can be used as many times as required to define multiple cases and what to do in each. The testing criteria is called an expression. An expression can have one ( grade > 90) or more conditional statements (grade < 90 and grade > 50). All conditional statements must be met for an expression to be evaluated as TRUE and for the following command to run. If none of the expressions are TRUE, then Else defines what code to run.

Check this video for another example.

.. raw:: html

  <iframe width="560" height="315" src="https://www.youtube.com/watch?v=42MBMSOZgD4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Loops
^^^^^

Commands are typically run once when defined, but loops allow the programmer to run a block of code more than one time. There are two types of loops in Python: a “for” loop, and a “while” loop. The “for” loop is used to iterate over a set of items or run a code for a specified number of times. The “while” loop, however, continues running until a certain condition is no longer met.

.. code-block:: python

  letters = [“a”, “b”, “c”, “d”]
  for x in letters:
  	print(x)
  print(“Done!”)

In this example, “x” is called the iterating variable, and “letters” is the sequence. “x” is assigned every value in letters one at a time, and the code inside the loop is executed each time. When the list ends, the code after the loop runs in the regular sequence.

.. code-block:: python

  n = 5
  while n < 50:
  	print(n)
  	n = (n – 2) * 2
  print(“Done!”)

Similar to an “if” condition, a while loop also uses an expression (n < 50) that defines when the loop should continue running. If the condition is no longer met, the loop breaks, and the code after the loop executes in the regular sequence.

This video covers loops in more depth.

.. raw:: html

  <iframe width="560" height="315" src="https://www.youtube.com/watch?v=6iF8Xb7Z3wQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Comments
^^^^^^^^

Comments help annotate code or add other information in natural language. Comments are not Python code; they are ignored by the interpreter. Comments are marked using the hash (#) symbol at the beginning of a line, and the font color turns gray in this case.

.. code-block:: python

  # This code prints “Hello World!”
  print(“Hello World!”)

Best Practices
--------------

Commenting
^^^^^^^^^^

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec enim magna, pellentesque vitae congue non, tincidunt sed tortor. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Proin risus tortor, tempus et malesuada non, pretium quis tortor. Donec justo leo, egestas eget hendrerit vitae, auctor sit amet ipsum. Vestibulum sodales sed nisl quis volutpat. Integer sed odio tellus. Nam bibendum in elit ultricies pulvinar. Vivamus suscipit purus fringilla, hendrerit lectus at, dictum libero. Curabitur sed facilisis magna.

Naming
^^^^^^

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec enim magna, pellentesque vitae congue non, tincidunt sed tortor. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Proin risus tortor, tempus et malesuada non, pretium quis tortor. Donec justo leo, egestas eget hendrerit vitae, auctor sit amet ipsum. Vestibulum sodales sed nisl quis volutpat. Integer sed odio tellus. Nam bibendum in elit ultricies pulvinar. Vivamus suscipit purus fringilla, hendrerit lectus at, dictum libero. Curabitur sed facilisis magna.

Indentation
^^^^^^^^^^^

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec enim magna, pellentesque vitae congue non, tincidunt sed tortor. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Proin risus tortor, tempus et malesuada non, pretium quis tortor. Donec justo leo, egestas eget hendrerit vitae, auctor sit amet ipsum. Vestibulum sodales sed nisl quis volutpat. Integer sed odio tellus. Nam bibendum in elit ultricies pulvinar. Vivamus suscipit purus fringilla, hendrerit lectus at, dictum libero. Curabitur sed facilisis magna.

Multiple Line Spanning
^^^^^^^^^^^^^^^^^^^^^^

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec enim magna, pellentesque vitae congue non, tincidunt sed tortor. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Proin risus tortor, tempus et malesuada non, pretium quis tortor. Donec justo leo, egestas eget hendrerit vitae, auctor sit amet ipsum. Vestibulum sodales sed nisl quis volutpat. Integer sed odio tellus. Nam bibendum in elit ultricies pulvinar. Vivamus suscipit purus fringilla, hendrerit lectus at, dictum libero. Curabitur sed facilisis magna.

Testing
^^^^^^^

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec enim magna, pellentesque vitae congue non, tincidunt sed tortor. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Proin risus tortor, tempus et malesuada non, pretium quis tortor. Donec justo leo, egestas eget hendrerit vitae, auctor sit amet ipsum. Vestibulum sodales sed nisl quis volutpat. Integer sed odio tellus. Nam bibendum in elit ultricies pulvinar. Vivamus suscipit purus fringilla, hendrerit lectus at, dictum libero. Curabitur sed facilisis magna.

Self-directed Learning Resources
--------------------------------

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec enim magna, pellentesque vitae congue non, tincidunt sed tortor. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Proin risus tortor, tempus et malesuada non, pretium quis tortor. Donec justo leo, egestas eget hendrerit vitae, auctor sit amet ipsum. Vestibulum sodales sed nisl quis volutpat. Integer sed odio tellus. Nam bibendum in elit ultricies pulvinar. Vivamus suscipit purus fringilla, hendrerit lectus at, dictum libero. Curabitur sed facilisis magna.

Books
^^^^^

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec enim magna, pellentesque vitae congue non, tincidunt sed tortor. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Proin risus tortor, tempus et malesuada non, pretium quis tortor. Donec justo leo, egestas eget hendrerit vitae, auctor sit amet ipsum. Vestibulum sodales sed nisl quis volutpat. Integer sed odio tellus. Nam bibendum in elit ultricies pulvinar. Vivamus suscipit purus fringilla, hendrerit lectus at, dictum libero. Curabitur sed facilisis magna.

YouTube Channels
^^^^^^^^^^^^^^^^

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec enim magna, pellentesque vitae congue non, tincidunt sed tortor. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Proin risus tortor, tempus et malesuada non, pretium quis tortor. Donec justo leo, egestas eget hendrerit vitae, auctor sit amet ipsum. Vestibulum sodales sed nisl quis volutpat. Integer sed odio tellus. Nam bibendum in elit ultricies pulvinar. Vivamus suscipit purus fringilla, hendrerit lectus at, dictum libero. Curabitur sed facilisis magna.

Online Courses
^^^^^^^^^^^^^^

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec enim magna, pellentesque vitae congue non, tincidunt sed tortor. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Proin risus tortor, tempus et malesuada non, pretium quis tortor. Donec justo leo, egestas eget hendrerit vitae, auctor sit amet ipsum. Vestibulum sodales sed nisl quis volutpat. Integer sed odio tellus. Nam bibendum in elit ultricies pulvinar. Vivamus suscipit purus fringilla, hendrerit lectus at, dictum libero. Curabitur sed facilisis magna.
