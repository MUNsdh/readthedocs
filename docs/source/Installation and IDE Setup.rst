Installation and IDE Setup
==========================

.. role:: python(code)
   :language: python

**By the end of this section, students should be able to:**

- Install Python and troubleshoot the Path variable issue
- Use a terminal window to run Python code through the interpreter or from a script

Installing Python
-----------------

Python is available for different environments, including Windows, Mac, and Linux. Python 3 distributions can be downloaded from the official Python website.

**Windows**

#. Go to the `official Python website <https://www.python.org>`_

#. From the Downloads menu, click Windows

   .. figure:: ../_static/images/python_website.png
    :align: center

#. Under Stable Releases, click to download the Windows installer (32-bit or 64-bit depending on your system) for the Python release you want. Ideally, you would want to download the latest stable release

   .. figure:: ../_static/images/download_windows.png
    :align: center

#. When downloading is done, double-click the file to run the installer

#. Check the box that says “Add Python 3.x.x to PATH”. This allows Windows to find the Python interpreter when running Python code

   .. figure:: ../_static/images/install_windows_1.png
    :align: center

#. Click Install Now

   .. figure:: ../_static/images/install_windows_2.png
    :align: center

**Mac**

#. Go to the `official Python website <https://www.python.org>`_

#. From the Downloads menu, click Mac OS X

#. Under Stable Releases, click to download the macOS 64-bit installer. Ideally, you would want to download the latest stable release. If your Macbook is uses an Intel processor (Macbook version 2019 or older), download the Intel installer. If it is using Apple Silicon (Macbook version 2020 or newer), opt for the Universal2 installer

#. When downloading is done, double-click the file to run the installer

#. Follow the instructions and click Continue until it shows the installation destination

#. Click Install

**Ubuntu**

#. Open a new terminal window

#. Type the following command to install Python 3.
   .. code-block:: bash

    sudo apt-get install python3.x

   Replace x with the desired Python release. You can find the latest release number on the `official Python website <https://www.python.org>`_

   .. figure:: ../_static/images/install_ubuntu.png
    :align: center


**Other Linux Systems**

Check `this <https://opensource.com/article/20/4/install-python-linux>`_ tutorial on how to configure and build Python from the source code

Setting Up Python
-----------------

Python should be set up and ready to use after installation. To make sure Python is set up correctly, try to check the installed Python version using a terminal window.

**Windows**

#. Open the start menu

#. Search for Command Prompt and open a new window

#. Type the following command and press enter

   .. code-block:: python

    python --version

.. figure:: ../_static/images/set_up_windows.png
  :align: center

**Mac**

#. Click on the magnifying glass in the top bar to open the Spotlight finder

#. Type Terminal and open a new window

#. Type the following command and press enter

   .. code-block:: python

    python3 --version

**Linux**

#. Depending on your system, search for Terminal in the applications menu. Common shortcuts include Ctrl+Alt+T or Alt+T

#. Type the following command and press enter

   .. code-block:: python

    python3 --version

.. figure:: ../_static/images/set_up_ubuntu.png
  :align: center

The command should output “Python 3.x.x”, the version of Python you installed. If you get any errors, a probable cause is that Python is not added to the system’s PATH variable. Check `this <https://www.techwalla.com/articles/how-to-set-your-python-path>`_ tutorial on how to solve this issue on Windows, Mac, and Linux.

Running Python Code
-------------------

You can interact directly with the Python interpreter through a terminal. To do that, open a new terminal/cmd window, type the following command, and press enter.

**Windows**

.. code-block:: python

  python

**Mac/Linux**

.. code-block:: python

  python3

You can then write code to be directly executed by the interpreter. Try entering :python:`print(5/2)` and check the output.

**Windows**

.. figure:: ../_static/images/run_windows_1.png
  :align: center

**Linux**

.. figure:: ../_static/images/run_ubuntu_1.png
  :align: center

This method is quick for testing commands, but we will be writing Python scripts in files as it is more organized.

**Windows**

#. Open a new Notepad window

#. Type in the following code

   .. code-block:: python

    for n in range (1, 10):
      print (n)

#. Save the file, selecting “All Files” for file type and changing the extension to .py

   .. figure:: ../_static/images/run_windows_3.png
      :align: center

#. Open the cmd, and enter the following command, replacing C:\\path with the path to your Python script

   .. code-block:: python

    python C:\path

.. figure:: ../_static/images/run_windows_4.png
   :align: center

**Mac/Linux**

#. Open a new Text Edit window

#. Type in the following code

   .. code-block:: python

    for n in range (1, 10):
      print (n)

#. Save the file, and change the extension to .py

   .. figure:: ../_static/images/run_ubuntu_2.png
    :align: center

#. Open the terminal, and enter the following command, replacing /path with the path to your Python script

   .. code-block:: python

    python3 /path

.. figure:: ../_static/images/run_ubuntu_3.png
   :align: center

Python IDEs and Interfaces
--------------------------

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec enim magna, pellentesque vitae congue non, tincidunt sed tortor. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Proin risus tortor, tempus et malesuada non, pretium quis tortor. Donec justo leo, egestas eget hendrerit vitae, auctor sit amet ipsum. Vestibulum sodales sed nisl quis volutpat. Integer sed odio tellus. Nam bibendum in elit ultricies pulvinar. Vivamus suscipit purus fringilla, hendrerit lectus at, dictum libero. Curabitur sed facilisis magna.

IDLE
^^^^

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec enim magna, pellentesque vitae congue non, tincidunt sed tortor. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Proin risus tortor, tempus et malesuada non, pretium quis tortor. Donec justo leo, egestas eget hendrerit vitae, auctor sit amet ipsum. Vestibulum sodales sed nisl quis volutpat. Integer sed odio tellus. Nam bibendum in elit ultricies pulvinar. Vivamus suscipit purus fringilla, hendrerit lectus at, dictum libero. Curabitur sed facilisis magna.

PyCharm
^^^^^^^

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec enim magna, pellentesque vitae congue non, tincidunt sed tortor. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Proin risus tortor, tempus et malesuada non, pretium quis tortor. Donec justo leo, egestas eget hendrerit vitae, auctor sit amet ipsum. Vestibulum sodales sed nisl quis volutpat. Integer sed odio tellus. Nam bibendum in elit ultricies pulvinar. Vivamus suscipit purus fringilla, hendrerit lectus at, dictum libero. Curabitur sed facilisis magna.

Atom
^^^^

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec enim magna, pellentesque vitae congue non, tincidunt sed tortor. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Proin risus tortor, tempus et malesuada non, pretium quis tortor. Donec justo leo, egestas eget hendrerit vitae, auctor sit amet ipsum. Vestibulum sodales sed nisl quis volutpat. Integer sed odio tellus. Nam bibendum in elit ultricies pulvinar. Vivamus suscipit purus fringilla, hendrerit lectus at, dictum libero. Curabitur sed facilisis magna.

Spyder
^^^^^^

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec enim magna, pellentesque vitae congue non, tincidunt sed tortor. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Proin risus tortor, tempus et malesuada non, pretium quis tortor. Donec justo leo, egestas eget hendrerit vitae, auctor sit amet ipsum. Vestibulum sodales sed nisl quis volutpat. Integer sed odio tellus. Nam bibendum in elit ultricies pulvinar. Vivamus suscipit purus fringilla, hendrerit lectus at, dictum libero. Curabitur sed facilisis magna.


**Exercise**

#. How do you check the currently installed version of Python on your machine?

#. Predict the output of the following code.

   .. code-block:: python

    print("5 Times Table")
    for n in range (1, 10):
      s = "5x" + str(n) + "=" + str(5*n)
      print(s)

   After that, type the script into a file and run it on your machine. Verify your prediction is correct.
