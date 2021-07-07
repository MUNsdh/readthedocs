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

For example, the following statements do the same function but in different languages. They all output "Hello World!" to the terminal if a variable (explained later) is equal to 1.

**Java**

.. code-block:: java

  if(x == 1){
  	System.out.print("Hello World!");
  }

**C**

.. code-block:: c

  if(x == 1){
  	printf("Hello World!");
  }

**Python**

.. code-block:: python

  if x == 1:
  	print("Hello World!")

Notice how the print statement ends in a semicolon (;) in both Java and C. One of the main features of Python syntax that sets it apart is that it does not use a symbol to denote the termination of an instruction. Also, unlike most languages, where code blocks are wrapped in curly braces (notice the if statement syntax), Python relies on indentation to define which block a statement belongs to. Indentation, which is always encouraged to use in other languages, is required in Python and contributes to the readability of Python scripts.

The following subsections go through the syntax of the most common python statements.

Variables
^^^^^^^^^

Variables are reserved memory spaces defined by the programmer to hold a specific value. The value can be a number, a character, text, or an object (refer to the introduction part for more information about object-oriented programming). In many languages, the type of the variable needs to be explicitly defined when declaring that variable. However, Python automatically decides the variable type when it is assigned a value.

In this example, variable a is an integer, b is a floating value, and c is a string of text. The value on the right side of the = operator is assigned the variable (operand) on the left side. Notice how keywords (int, float, and String in other languages) are not used to specify the data type

.. code-block:: python

  a = 2021
  b = 3.14
  c = "Hello World!"

The video below discusses Python variables with more examples.

.. raw:: html

  <iframe width="560" height="315" src="https://www.youtube.com/embed/cQT33yu9pY8" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

|

Conditions
^^^^^^^^^^

Conditions are statements that allow the programmer to decide which commands to run based on certain criteria. Conditions in Python are defined using the *if* statement, which can be used standalone to make a decision. *elif* and *else* keywords can be used to extend an *if* statement.

.. code-block:: python

  grade = 78

  if grade > 90:
  	print("Excellent")
  elif grade<90 and grade>50:
  	print("Passed")
  else:
  	print("Failed")

*elif* can be used as many times as required to define multiple cases and what to do in each. The testing criteria is called an expression. An expression can have one :python:`grade > 90` or more conditional statements :python:`grade<90 and grade>50`. All conditional statements must be met for an expression to be evaluated as TRUE and for the following command to run. If none of the expressions are TRUE, then *else* defines what code to run.

Check this video for another example.

.. raw:: html

  <iframe width="560" height="315" src="https://www.youtube.com/embed/42MBMSOZgD4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

|

Loops
^^^^^

Commands are typically run once when defined, but loops allow the programmer to run a block of code more than one time. There are two types of loops in Python: a *for* loop, and a *while* loop. The *for* loop is used to iterate over a set of items or run a code for a specified number of times. The *while* loop, however, continues running until a certain condition is no longer met.

.. code-block:: python

  letters = ["a", "b", "c", "d"]
  for x in letters:
  	print(x)
  print("Done!")

In this example, *x* is called the iterating variable, and *letters* is the sequence. *x* is assigned every value in letters one at a time, and the code inside the loop is executed each time. When the list ends, the code after the loop runs in the regular sequence.

.. code-block:: python

  n = 5
  while n < 50:
  	print(n)
  	n = (n–2) * 2
  print("Done!")

Similar to an *if* condition, a *while* loop also uses an expression :python:`n < 50` that defines when the loop should continue running. If the condition is no longer met, the loop breaks, and the code after the loop executes in the regular sequence.

This video covers loops in more depth.

.. raw:: html

  <iframe width="560" height="315" src="https://www.youtube.com/embed/6iF8Xb7Z3wQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

|

Comments
^^^^^^^^

Comments help annotate code or add other information in natural language. Comments are not Python code; they are ignored by the interpreter. Comments are marked using the hash (#) symbol at the beginning of a line, and the font color turns gray in this case.

.. code-block:: python

  # This code prints "Hello World!"
  print("Hello World!")


Best Practices
--------------

Every programming language has a set of recommended guidelines to improve the quality of codes. `Python Enhancement Protocol <https://www.python.org/dev/peps/pep-0008>`_, or PEP 8, is a document written by Guido van Rossum, the creator of Python, to provide guidelines on how to write proper Python code (recall that Python is focused on readability). Unlike syntax, these guidelines are not mandatory to follow; the code will still work without them. However, using the styling guidelines helps programmers write a cleaner, more efficient code that is easier to edit, maintain, and debug. This is especially important for team projects, where the code is being edited and developed by programmers of different perspectives; every line of code written by one person should clearly communicate its purpose to the rest of the team members.
Below are some of the essential guidelines to follow for beginners. You can also check `this <https://realpython.com/python-pep8>`_ article which goes into more guidelines and styling details.

Naming
^^^^^^

Naming involves variables, methods, functions, classes, and any other structure you declare in your code. Following the naming guidelines and choosing descriptive names contribute massively to code readability. The key naming rules are:

- Names of variables, functions, and methods are lowercase, and words are separated by an underscore

.. code-block:: python

  class_size = 13
  def distance_from_origin (x, y):
  	return sqrt(x^2 + y^2)

- Constants are all uppercase, and words are separated by an underscore

.. code-block:: python

  EARTH_GRAVITY = 9.81

- Classes’ names are camel case (capitalize the first letter of every word), and words are not separated

.. code-block:: python

  class DogBreed:

When choosing a name for your variable or function, make sure it clearly and concisely describes what it represents. For example, naming a variable *x* or *a* does not tell much about the information that object holds.

.. code-block:: python

  a = 1.25

If you revisit your code later, you would probably not remember why you created the variable. A clearer name would be

.. code-block:: python

  apples_unit_price = 1.25

Now other programmers who did not participate in developing the code can recognize the variable

Indentation
^^^^^^^^^^^

As mentioned before, indentation in Python defines what code block a statement belongs to. So, it is very important to use the right number of tabs to avoid bugs and unexpected results.
For example, these two code give different outputs:

.. code-block:: python

  student_grade = 40
  if student_grade > 50:
  	print("Student Passed")
  	print("Done")

  # Outputs nothing

|

.. code-block:: python

  student_grade = 40
  if student_grade > 50:
  	print("Student Passed")
  print("Done")

  # Outputs Done

In the first case, the statement :python:`print("Done")` belongs to the if statement because it is indented so that it is inside the if block. In the second case, it outside the if statement block, so it is not affected by the condition statement.

Multiple Line Spanning
^^^^^^^^^^^^^^^^^^^^^^

Sometimes, a single statement can be too long to fit in one line. On a small editor window, the statement will break into multiple lines, which is called line-wrapping. PEP 8 recommends keeping lines shorter than 79 characters to improve readability.

.. code-block:: python

  long_statement = "This is a very long statement that exceeds 79 characters and should span more than one line."

  def add_new_student(first_name, last_name, date_of_birth, email, phone_number, year_group):
    pass

The two statements above need to be broken into at least two lines. If the code is contained inside a bracket, like in the second case, then it can simply be divided by a newline. Otherwise, a backslash is needed.

.. code-block:: python

  long_statement = "This is a very long statement \
                		that exceeds 79 characters \
                		and should span more than one line."

    def add_new_student(first_name, last_name,
			                  email, phone_number,
			                  date_of_birth, ear_group):
        pass

Spacing
^^^^^^^

Whitespace and blank lines improve the visually appeal of your code. Whitespace is mainly used in the following cases:

- After a comma

.. code-block:: python

  distance_from_origin(10, 20)

- Surrounding an operator (=, >, <, and, or, …)

.. code-block:: python

  if grade > 90:    # Yes
  if grade>90:      # No

If the equal sign is used to assign values to function arguments, then spaces should not be used

.. code-block:: python

  def filter_by_price(max_price=25):
    pass

Also, when combining operators, spaces are used for the lower priority operator only.

.. code-block:: python

  if grade<90 and grade>50:         # Yes
  if grade < 90 and grade > 50:     # No


A blank line is used to separate functions and methods. It can also be used by the programmer when needed to separate steps in a block of code.

.. code-block:: python

  def distance_from_origin(x, y):
	   return sqrt(x^2 + y^2)

  def average_of(x, y):
	   return (x+y) / 2

Commenting
^^^^^^^^^^

Comments should be made throughout the code as a way of documentation. Programmers need to state what certain functions do, their arguments, variables, and the purpose of a loop or a condition. Commenting is specifically important in team projects as it helps collaborators understand the code and how it should be used. Also, a programmer revisiting their old code will benefit from having comments explaining the code’s functionality.
A comment starts with a hash and space "# " and should be indented in the same way as the statement it describes. Comments can also be written in the same line as the code and are called inline comments. The 79-character rule also applies to comments, where a comment can be broken by another hash as a new line.

.. code-block:: python

  grade = 78	# Student’s final test grade

  # Condition to print the current state of a student
  # based on their grade in the final test
  if grade > 90:
  	print("Excellent")
  elif grade<90 and grade>50:
  	print("Passed")
  else:
  	print("Failed")

For documenting a function or a class, the text should be enclosed in quotation marks, and hashes are not used.

.. code-block:: python

  """
  Calculates and returns the distance of a coordinate point
  from the origin using the 2D distance formula.
  x: x-coordinate of the endpoint
  y: y-coordinate of the endpoint
  """
  def distance_from_origin(x, y):
  	return sqrt(x^2 + y^2)


Self-directed Learning Resources
--------------------------------

This tutorial briefly covered basic Python syntax for the purpose of demonstrating ideas and concepts. Below is a list of recommended resources for beginners to start learning Python coding and write complete functional programs.

YouTube Channels
^^^^^^^^^^^^^^^^

`CS Dojo <https://www.youtube.com/playlist?list=PLBZBJbE_rGRWeh5mIBhD-hhDwSEDxogDg>`_

CS Dojo by YK offers a complete playlist of videos for beginners. It covers the basics of Python (syntax, conditions, and loops), and there is an exercise in the end.

`Telusko <https://www.youtube.com/playlist?list=PLsyeobzWxl7poL9JTVyndKe62ieoN-MZ3>`_

A more comprehensive, well-organized course that covers Python from beginner basics to intermediate levels

`Programming with Mosh <https://www.youtube.com/watch?v=_uQrJ0TkZlc>`_

This is a 6-hour-long Python tutorial for beginners. The video is divided into multiple sections so that you can skip to certain topics.


Online Courses
^^^^^^^^^^^^^^

`Programming for Everybody - coursera <https://www.coursera.org/learn/python>`_

A great course by the University of Michigan that teaches everyone the basics of Python programming. There is also a more advanced course offered after this level.

`Introduction to Computer Science and Programming Using Python – edX <https://www.edx.org/course/introduction-to-computer-science-and-programming-7>`_

Course offered by MIT and covers not only Python programming but also computational thinking and data science for beginners.

`Python Basic Tutorial – tutorialspoint <https://www.tutorialspoint.com/python/index.htm>`_

This non-video course is suitable for beginners and can be used as a quick reference to check syntax or structures.


Books
^^^^^

`Learn Programming in Python with Cody Jackson <https://www.amazon.ca/Learn-Programming-Python-Cody-Jackson-ebook/dp/B07L1NHCHC>`_

This book introduces the basics of Python syntax, variables, functions, classes, and more. It also discusses software development and testing methods.

`Python Crash Course, 2nd Edition <https://www.amazon.ca/dp/1593279280>`_

Teaches you the fundamentals of Python and allows you to apply them using three projects in the second half of the book.

`Python Pocket Reference <https://www.amazon.ca/dp/1449357016>`_

A pocket guide that contains information about Python syntax and statements, special functions, and common libraries for you to review.
