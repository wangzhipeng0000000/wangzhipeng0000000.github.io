git clone  https://github.com/wangzhipeng0000000/wangzhipeng0000000.github.io/blob/main/README.md
cd wangzhipeng0000000.github.io
echo "hello world" > ndex.html
git add --all
git commit -m "Initial commit"
git push -u origin main
jupyter:
  kernelspec:
    display_name: Python 3.11.1 64-bit
    language: python
    name: python3
  language_info:
    codemirror_mode:
      name: ipython
      version: 3
    file_extension: .py
    mimetype: text/x-python
    name: python
    nbconvert_exporter: python
    pygments_lexer: ipython3
    version: 3.11.1
  nbformat: 4
  nbformat_minor: 4
  vscode:
    interpreter:
      hash: aee8b7b246df8f9039afb4144a1f6fd8d2ca17a180786b69acc140d282b71a49
---

<div class="cell code" execution_count="8">

``` python
PART 1 : 
1、question:campare the students in TAMS and BUND ,and find out who are better in math
   purpose:to find out which major requires higher math level
2、sample:collge SAT score from Tableau demo
   2013 asian men TAMS & 2013 asian men BUND
   variable:the major
   the statistic : math score
   quantitative or categorical:quantitative
3、assumption:TAMS students do better in math than BUND students
4、resourse:the statistic in github raw csv
5、if the time and money are enough,I would choose more school to explore.
```

<div class="output error" ename="SyntaxError"
evalue="invalid decimal literal (2966126372.py, line 2)">

      Cell In[8], line 2
        1、question:campare the students in TAMS and BUND ,and find out who are better in math
        ^
    SyntaxError: invalid decimal literal

</div>

</div>

<div class="cell markdown">

PART 2 : import pandas as pd df =
pd.read_csv(<https://github.com/prasertbs/basic-dataset/commit/1bfede4aebc25db5d38a6712a28cec03d09a7f69>)
df.head(5)

</div>

<div class="cell code" trusted="true">

``` python
PART 3 :
campare the math scores of 2013 asian men in TAMS & 2013 asian men in BUND
```

</div>

<div class="cell code" execution_count="7" trusted="true">

``` python
import pandas as pd
df = pd.read_csv(https://github.com/prasertbs/basic-dataset/commit/1bfede4aebc25db5d38a6712a28cec03d09a7f69)
df.head(5)
```

<div class="output error" ename="SyntaxError"
evalue="invalid decimal literal (1539317104.py, line 2)">

      Cell In[7], line 2
        df = pd.read_csv(https://github.com/prasertbs/basic-dataset/commit/1bfede4aebc25db5d38a6712a28cec03d09a7f69)
                                                                           ^
    SyntaxError: invalid decimal literal

</div>

</div>

<div class="cell code">

``` python
TAMS                BUND
530                400.4
577.7              405.6
583                431.6
583                436.8
598.9              462.8
```

</div>

<div class="cell code" execution_count="6">

``` python
(df[df['Major'] == ['TAMS']['Math']).head(5)
```

<div class="output error" ename="SyntaxError"
evalue="closing parenthesis ')' does not match opening parenthesis '[' (97410733.py, line 1)">

      Cell In[6], line 1
        (df[df['Major'] == ['TAMS']['Math']).head(5)
                                           ^
    SyntaxError: closing parenthesis ')' does not match opening parenthesis '['

</div>

</div>

<div class="cell code" execution_count="5">

``` python
(df[df['Major'] == ['BUND']['Math']).head(5)
```

<div class="output error" ename="SyntaxError"
evalue="closing parenthesis ')' does not match opening parenthesis '[' (1925996197.py, line 1)">

      Cell In[5], line 1
        (df[df['Major'] == ['BUND']['Math']).head(5)
                                           ^
    SyntaxError: closing parenthesis ')' does not match opening parenthesis '['

</div>

</div>

<div class="cell code" execution_count="2">

``` python
import matplotlib.pyplot as plt
import seaborn as sns
plt.rcParams['figure.figsize'] = [10,5]
sns.set()
```

<div class="output error" ename="ModuleNotFoundError"
evalue="No module named 'matplotlib'">

    ---------------------------------------------------------------------------
    ModuleNotFoundError                       Traceback (most recent call last)
    Cell In[2], line 1
    ----> 1 import matplotlib.pyplot as plt
          2 import seaborn as sns
          3 plt.rcParams['figure.figsize'] = [10,5]

    ModuleNotFoundError: No module named 'matplotlib'

</div>

</div>

<div class="cell code" execution_count="3">

``` python
sns.histplot(df,x='TAMS',y='math score')
plt.show()
```

<div class="output error" ename="NameError"
evalue="name 'sns' is not defined">

    ---------------------------------------------------------------------------
    NameError                                 Traceback (most recent call last)
    Cell In[3], line 1
    ----> 1 sns.histplot(df,x='TAMS',y='math score')
          2 plt.show()

    NameError: name 'sns' is not defined

</div>

</div>

<div class="cell code" execution_count="4">

``` python
sns.histplot(df,x='BUND',y='math score')
plt.show()
```

<div class="output error" ename="NameError"
evalue="name 'sns' is not defined">

    ---------------------------------------------------------------------------
    NameError                                 Traceback (most recent call last)
    Cell In[4], line 1
    ----> 1 sns.histplot(df,x='BUND',y='math score')
          2 plt.show()

    NameError: name 'sns' is not defined

</div>

</div>
