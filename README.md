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
    3). we can not use the keywords(like if、and、else...) to name the variable
    4). begin and end with double underline has a special meaning, we should avoid when name a variable, like the '__init__' means a class
    5). when we use the variable, we must initialize it
    6). use the 'del variable' to delete a variable  
  4. Line connector  
    If the character is too many in one line code when we writing the code, we can use the line connector '\' to write the character in many lins  

## Object  
  1. one Object is composed by identity、type、value  
    identity: is to uniquely identifying the object, we can use the function: id(obj) to return the obj's identity  
    type: represents the type of data the object stores, use the function: type(obj) return the obj's tpye  
    value: represents the information of the data that stored by the object, use the function: print(obj) can get the value of object  
  
  2. Quote  
  3. Identifier  
    1). module and bag name: all lower case, like: math  
    2). function name: all lower case, different words use the '_' to connect, like: my_name  
    3). class name: the first alphabet is capital of every words, (Hump principle） like: MyPhone  
    4). constant： all capital, like: MAX_SPEED  
  4. Type of Data  
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
         14) use the join to concatenate multiple strings  
         15） format():  
         example code1:  
```
         a= "name is :{0}, age is :{1}, address is {2}"  
         a.format('ray', 18, 'beijing')  
         # '>>>'means the result of the code!  
         >>> the result is : name is ray, age is 18, address is beijing  
```

         example code2:  

```
           "I am {0}, The number I like is {1:*>8}".format('ray', '666') 
           # '>>>'means the result of the code!
           >>> result: I am ray, The number I like is **666***  
```  
         15) Mutable string:  
         example code:  
```
             import io  
             s = "hello,sxt"  
             sio = io.StringIO(s)  
             sio.getvalue()  
             # '>>>'means the result of the code!
             >>> hello,sxt  
             sio.seek(7)  
             sio.write('g')  
             sio.getvalue()  
             # '>>>'means the result of the code!
             >>> hello,gxt  
 ```
  5. Comparison operator： ==、!=、>、<、>=、<=  
      The difference between is and ==  
        is: judge the two identifiers is or not the same object(Memory address)  
        ==: judge the value of object is same or not, it as use the method: '__eq__()'  
      notice: the number in -5 ~ 256 will be putted into cache for reuse  
  6. Logical Operators： or、and、not  
  7. print()  
    when we want the new print() is the same line with the previous print(), we can use the way print('aa', end='') to achieve  

## Sequence
  1. sequence is a way to store the data  
  2. string、list、tuple、dictionary、set is all sequence  
  3. list:  
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
    18). Two-dimensional list:  
    
    ```  
    listName = [['rogy', 18, 'beijing'], 
                ['ray', 20, 'kunming'], 
                ['jon', 22, 'changsha']]  
        for m in range(3):  
            for n in range(3):  
                print(listName[m][n], end='\t')  
        print()  
    ```
  
  4. Tuple
     1). the method of create a tuple: tupleName = (element, )(remeber: if there is only one element of a tuple, we must add a ',' in the end); tupleName = tuple()  
     2). notice: a tuple can not be revised; and the other methods is like a list  
     3). zip()  
       ```  
       a = [10, 20, 30]  
       b = [40, 50, 60]  
       c = [70, 80, 90]  
       d = zip(a, b, c)  
       list(d)  
       # '>>>'means the result of the code!
       >>> [(10, 40, 70), (20, 50, 80), (30, 60, 90)]  
       ```  
  5. Dictionary  
     1). the method of create a dictionary: dictName = {} or dictName = dict(name='rogy', age=18)  
     2). zip()  
        ```  
        keys = ['name', 'age', 'job']  
        values = ['rogy', 18, 'teacher']  
        d = dict(zip(keys, values))  
        d  
        # '>>>'means the result of the code!
        >>> {'name':'rogy', 'age':18, 'job':'teacher'}  
        ```
     3). dictName = {key1:value1, key2:value2,...}(in a dict, the key only can be appear once)  
     4). dictName[key1] = value1 or dictName.get(key1) = value1(in this way, if the key is not existence， is will return None, the first way will return a error)  
     5). dictName1.update(dictName2)  
     6). del(dictName[key])  


## Select Structure
  1. Single Branch Selection Structure:(if...)  
  2. Double Branch Selection Structure:(if...else...)  
  3. Ternary conditional operator: (condition is True if condition expression else condition is False)  
  4. Multi-branch selection structure:(if...elif...elif...else...)  
  5. Select structure nesting: (if...if...else...else...; must notice the indentation)  
  example code:  
  ```
  score = int(input("Please entry a number in 0-100："))  
  degree = "ABCDE"  
  num = 0  
  if score>100 or score<0:  
    score = int(input("Wrong input! Please entry a new number in 0-100:"))  
  else:  
    num = score//10  
    if num<6:  
      num=5
      
    print("score is {0},degree is {1}".format(score,degree[9-num]))
  ```
  
## Cycle Structure
  1. while  
  2. for  
  3. Iterable object：sequence, dictionary, iterator, generator  
  4. Nested loop：  
  ```
  for x in range(5):
    for y in range(5):
      print(x, end="\t")
    print()  # newline
  ```
  
  ```
  for m in range(1, 10):
    for n in range(1, m+1):
      print("{0}*{1} = {2}".format(m, n, (m*n)), end="\t")
    print()
  ```
  
  5. break and continue  
  6. Loop optimization  
    1). reduce calculations inside the loop  
    2). in the nested loop, reduce the caculation of the inner loop  
    3). using local variables  
    
  7. zip()  
  ```
  names = ('rogy', 'ray', 'tom')
  ages = (18, 22, 20)
  cities = ('beijing', 'tianjin', 'shanghai')
  
  for name, age, city in zip(names, anges, cities):
    print("name is {0}, age is {1}, city is {2}".format(name, age, city))
  
  for i in range(3):
    print("name is {0}, age is {1}, city is {2}".format(names[i], ages[i], cities[i]))
  ```
  8. Comprehension  
    1). list comprehension:  
      ```  
      y = [x for x in range(1,5)]  
      print(y)  
      m = [x*2 for x in range(1, 50) if x%5 == 0]  
      print(m)  
      cells = [(row, col) for row in range(1, 10) for col in range(1, 10)]  
      print(cells)  
      ```  
    2). dictionary comprehension:  
      ```  
      my_text = " i love you, i love set, i love gaoqi"  
      char_count = {c: my_text.count(c) for c in my_text}  
      print(char_count)  
      ```  
    3). set comprehension:  
      ```  
      b = {x for x in range(1, 100) if x%9 == 0}  
      print(b)  
      ```  
    4). generator comprehension:  
    notice: one generator only can run once  
      ```  
      gnt = (x for x in range(10) if x%9==0)  
      for x in gnt:  
        print(x, end=" ")  
      ```  
     practise:  
      ```  
      import turtle  

      my_colors = ['red', 'yellow', 'green', 'black', 'pink']  
      t = turtle.Pen()  
      for i in range(12):  
        t.goto(0, -i*10)  # 0, -100, -200, -300, -400  
        t.pendown()  
        t.color(my_colors[i%len(my_colors)])  
        t.circle(20 + i*10)  # 100, 200, 300, 400  
        t.penup()  
      turtle.done()  # 程序执行完毕，窗口任然在  
      ```  
    practise2:  
    
      ```  
      import turtle  
      t = turtle.Pen()  
      # 画棋盘  
      t.speed(0)  
      for i in range(19):  
        t.penup()  
        t.goto(-180, 180-i*20)  
        t.pendown()  
        t.goto(180, 180-i*20)  

      for j in range(19):  
        t.penup()  
        t.goto(-180+j*20, 180)  
        t.pendown()  
        t.goto(-180+j*20, -180)  
      turtle.done()  
      ```  

## Function
