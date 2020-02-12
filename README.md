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
  ###1. Indentation  
    The different lines code that have the same indentation(like 4 space) is the same code block; this likes the java use the {} express a code block. More rules of the python we can scan the "[PEP-8](https://www.python.org/dev/peps/pep-0008/)" to know.
   ###2. Comment  
    1). One line comment: use the #  
    2). Multi-line comments: use the """xxx"""  
   ###3. How to name the Variable  
    1). we only use the "alphabet、number and _ "to name a variable in the python, and only can begin with "alphabet and _ "  
    2). the capital alphabet is different with the lower case alphabet  
    3). we can not use the keywords(like if、and、else...) to name the variable
    4). begin and end with double underline has a special meaning, we should avoid when name a variable, like the '__init__' means a class
    5). when we use the variable, we must initialize it
    6). use the 'del variable' to delete a variable
   ###4. Line connector  
    If the character is too many in one line code when we writing the code, we can use the line connector '\' to write the character in many lins  

## Object  
   ###1. one Object is composed by identity、type、value  
  identity: is to uniquely identifying the object, we can use the function: id(obj) to return the obj's identity  
  type: represents the type of data the object stores, use the function: type(obj) return the obj's tpye  
  value: represents the information of the data that stored by the object, use the function: print(obj) can get the value of object  
  
   ###2. Quote  
   ###3. Identifier  
    1). module and bag name: all lower case, like: math  
    2). function name: all lower case, different words use the '_' to connect, like: my_name  
    3). class name: the first alphabet is capital of every words, (Hump principle） like: MyPhone  
    4). constant： all capital, like: MAX_SPEED  
    
   ###4. Type of Data  
    int (use the function int() to implementing type conversion to int)  
    float  
    bool  
    str：1) Create a string with single or double quotes  
         2) len() is to get the long of the str  
         3) Escape character: \n newline; \t Tabs; \r enter; \' single quotes; \" double quotes  
         4) method: str() is conver the other type of data to str  
         5) The essence of a string is a sequence of characters, so we can use '[0]' '[1]'...to extract each character  
         6) String immutable, we can use the method replace() to change the value and get a new string  
         7) slice string: '[start, end: step]' to intercept a string(it include the start element not include the end element)  
         8) split(): Splits a string into multiple substrings using the specified delimiter  
         9) join(): the way is like '  "*".join(a)  '  
         10) strip()  
         11) capitalize()、title()、upper()、lower()、swapcase()  
         12) center()、ljust()、rjust()  
         13) isalnum()、isalpha()、isdigit()、isspace()、isupper()、islower()  
         14） format():   
         example1: a= "name is :{0}, age is :{1}, address is {2}"; a.format('ray', 18, 'beijing') >>> the result is : name is ray, age is 18, address is beijing  
         example2: "I am {0}, The number I like is {1:*>8}".format('ray', '666') >>> result: I am ray, The number I like is **666***  
         15) Mutable string:  
         example:  
             >>>import io  
             >>>s = "hello,sxt"  
             >>>sio = io.StringIO(s)  
             >>>sio.getvalue()  
             hello,sxt  
             >>>sio.seek(7)  
             >>>sio.write('g')  
             >>>sio.getvalue()  
             hello,gxt  
   ###5. Comparison operator  
    ==、!=、>、<、>=、<=  
    the difference between is and ==  
      is: judge the two identifiers is or not the same object(Memory address)  
      ==: judge the value of object is same or not, it as use the method: '__eq__()'  
      notice: the number in -5 ~ 256 will be putted into cache for reuse  
   ###6. Logical Operators  
    or、and、not  
   ###7. print()  
    when we want the new print() is the same line with the previous print(), we can use the way print('aa', end='') to achieve  

## Sequence
  1. sequence is a way to store the data  
  2. string、list、tuple、dictionary、set is all sequence  
   ###3. list:  
    1). list.append(x)  
    2). list.extend(alist)  
    3). list.insert(index, x)  
    4). list.remove(x)  
    5). list.pop(index, x)  
    6). list.clear()  
    7). list.index(x)  
    8). list.count(x)  
    9). len(list)  
    10). list.reverse()  
    11). list.sort()  
    12). list.copy()  
    13). the method of adding elements to a list: listName.append(element), + (listName = listName + 50), extend(list), listName.insert(index, element), *(multiplication)  
    14). delete the element from a list: del listName[1], pop(index)(this method can return the element that we delete; if the index is none, it means delete the last element), listName.remove(element)(this method is to delete the element that it first appearance, if the element is not presence, it will return a error)  
    15). the access of a list: listName[index](if the index is out of range, it will return a error), listName.index(element, [start, [end]]), listName.count(element) (get the element occurrence times in the list), len(listName), element in list (judge the element is in or not in the list)  
    16). the slice of list: listName[start: end: step]  
    17). the sort of a list: listName.sort()(ascending order), listName.sort(reverse=True) (descending), random.shuffle(listName) {all of the up method is change the presence list}; listName.sorted() (this method is to create a new list to save the result)  
    18). Two-dimensional list: listName = [['rogy', 18, 'beijing'], ['ray', 20, 'kunming']] (listName[0][0] = rogy)  
    '''  
    listName = [['rogy', 18, 'beijing'], ['ray', 20, 'kunming'], ['jon', 22, 'changsha']]  
        for m in range(3):  
            for n in range(3):  
                print(listName[m][n], end='\t')  
        print()  
    '''
  
   ###4. Tuple
     1). the method of create a tuple: tupleName = (element, )(remeber: if there is only one element of a tuple, we must add a ',' in the end); tupleName = tuple()
