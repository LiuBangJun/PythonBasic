# PythonBasic
## Python Introduction
  1. python is an Interpretive and Object-oriented Language
  2. Website：www.python.org
  3. Guido van Rossum invented the python in 1989 and published it in 1991.(the word 'Python' means 'boa constrictor', it's because the '[龟叔](https://baike.baidu.com/item/%E5%90%89%E5%A4%9A%C2%B7%E8%8C%83%E7%BD%97%E8%8B%8F%E5%A7%86/328361?fromtitle=Guido%20van%20Rossum&fromid=3225314&fr=aladdin)' likes the British TV Series "Monty Python and the Flying Circus")
  4. Python's feature: Readable; Succinct; Object-oriented; Free and Open source；Portability and Cross-platform; Plentiful Library；Scalability(Glue language).
  5. Application Range：Scientific Computing、Artificial intelligence、Web server and Website backend、GUI Develop(Graphical user interface development)、Game development、Mobile devices、Embedded devices、System operation and maintenance、Big Data、Cloud computing...
  6. Python Interpreter:  
      (1) CPython：This Interpreter is using the C Programming language to achieve，it's most commonly used;  
      (2) Jython：This Interpreter is using the Java Programming language to achieve，can directly import the Java libraries;  
      (3) IronPython：This Interpreter is used in the .net platform;  
      (4) PyPy：This Interpreter is using the python Programming language to achieve
  7. The Zen of Python, by Tim Peters  
      Beautiful is better than ugly.  
      Explicit is better than implicit.  
      Simple is better than complex.  
      Complex is better than complicated.  
      Flat is better than nested.  
      Sparse is better than dense.  
      Readability counts.  
      Special cases aren't special enough to break the rules.  
      Although practicality beats purity.  
      Errors should never pass silently.  
      Unless explicitly silenced.  
      In the face of ambiguity, refuse the temptation to guess.  
      There should be one-- and preferably only one --obvious way to do it.  
      Although that way may not be obvious at first unless you're Dutch.  
      Now is better than never.  
      Although never is often better than *right* now.  
      If the implementation is hard to explain, it's a bad idea.  
      If the implementation is easy to explain, it may be a good idea.  
      Namespaces are one honking great idea -- let's do more of those!  
## Development Environment of Python
  1. IDLE、Pycharm、wingIDE、IPython、Eclipse and others is the most commonly used Development environment when the programmers write code
  2. There is many ways in the website to tell us how to install the python or pycharm and others tools thar you want to use, so you can deal it by youself though the website(there is a question that we should notice when we install the software, we shoule use the english or pinyin as the installation path)
  3. IDLE is the official standard development environment for python，it will be installed when we install the python
  
## Python Syntax Structure
  1. Indentation  
    The different lines code that have the same indentation(like 4 space) is the same code block; this likes the java use the {} express a code block. More rules of the python we can scan the "[PEP-8](https://www.python.org/dev/peps/pep-0008/)" to know.
  2. Comment  
    1). One line comment: use the #  
    2). Multi-line comments: use the """xxx"""  
  3. How to name the Variable  
    1). we only use the "alphabet、number and _ "to name a variable in the python, and only can begin with "alphabet and _ "  
    2). the capital alphabet is different with the lower case alphabet  
  4. Line connector  
    If the character is too many in one line code when we writing the code, we can use the line connector '\' to write the character in many lins  

## Object  
  1. one Object is composed by identity、type、value  
  identity: is to uniquely identifying the object, we can use the function: id(obj) to return the obj's identity  
  type: represents the type of data the object stores, use the function: type(obj) return the obj's tpye  
  value: represents the information of the data that stored by the object, use the function: print(obj) can get the value of object  
