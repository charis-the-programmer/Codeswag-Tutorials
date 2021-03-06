## Data Python Science with Python  

In the previous article, I mentioned that to do well in Data Science you required three main things; Math and statistics, programming, and business knowledge.

In this article I’ll go over the programming language we’ll be using; Python and setting up the environment for this series on Data Science.


### Python - An Overview 

#### What is Python?
Python is an open-source, general-purpose high-level programming language.

I’ll break this down.


##### Open-source
This means it is free. Python has a large and active community. Its source code is easily accessible, and because of this community and all its contributors, the language is constantly growing and upgrading. This is the main reason Python is cross-platform – it is available on just about all operating systems: Windows, Mac, and Linux.

#####  General-purpose 
There is a wide range of fields where Python could be applied. Apart from how we’ll be using it, it can be used for web programming through the Django framework, GUIs with the Tkinter to mention a few.

##### High-level language
This is a bit more technical.
Computers can run programs written in low-level languages, also called machine languages. These are difficult for a human to write in and understand. It is, therefore, more sensible to write programs in a high-level language. 

>**High-level language**: a programming language that enables a programmer to write programs that are independent of a particular type of computer. These languages are high-level because they are closer to human languages.  
>
>**Low-level language**: a programming language that is close to writing actual machine code.(binary, hexadecimal)

**To summarize**:      
What makes Python a powerful, often preferred over other programming languages, would be the following:
- Python is free and constantly updated.
- It is a programming language that can be used in multiple domains.
- Calculation processing does not require too much time.
 
These reasons will help us answer the following question. 


### Why use Python for Data Science?
- Python is a simple programming language to learn. It is designed to be highly readable, with clear-cut syntax.
- Its massive range of libraries helps make the task of Data Science that much easier. (TensorFlow, NumPy, Pandas)
- It is a very powerful and robust language.
- It allows developers to create programs and get prototypes running quickly, making the development process much faster.
- It can easily be ported to other languages if needed.

>**Libraries**: These are a collection of functions or methods that allows you to perform many actions without rewriting code.


### Getting Started - Jupyter Notebook
There are a plethora of editors and IDEs you can use for your Data Science work. For the sake of these tutorials, well be making use of the Jupyter Notebook.  

Jupyter Notebook is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations, and narrative text. 


#### Why Jupyter
- The Jupyter Notebook already comes with Python installed.
- It is well equipped for the demonstration of programming concepts.
- Unlike an editor that opens a separate window when you run your code, all your output is in the same window allowing quicker reviewing of code
- You can have explanations of your code right there in markdown


##### Installing Jupyter Notebook  

Once you have python installed, open your command line or terminal. (we will use pip that comes with python)  

First, ensure you have the latest version of pip. Type the following and press enter:  

`pip install --upgrade pip` 

![upgrading pip](https://codeswag.co.uk/wp-content/uploads/2020/01/uppip.png)


**Next, Type the following and press enter**
`pip install jupyter`  

![installing jupyter](https://codeswag.co.uk/wp-content/uploads/2020/01/putjupyteer.png)  

And that’s it! you’re ready to use Jupyter.

##### Running Jupyter Notebook
I recommend creating a folder for all your notebooks on your computer. This can also be done within the Jupyteri interface.  

To run Jupyter simply open your terminal and type the following and press enter. It will open a window in your browser after.  

`jupyter notebook`  

![run jupyter](https://codeswag.co.uk/wp-content/uploads/2020/01/opnjupyter.png)


##### Your First Program
As is customary we are going to write a **“Hello World!”** program. 
Navigate to the folder you created and then select new then Python3. A new window will be opened thereafter. 

![new program](https://codeswag.co.uk/wp-content/uploads/2020/01/new-jupyter2.png)

**In the next window, type `print(“Hello, World!”)` then click run**  
![the new notebook](https://codeswag.co.uk/wp-content/uploads/2020/01/blank-jupyter.png)  

**Your window should look like this afterward:**
![the output you should get](https://codeswag.co.uk/wp-content/uploads/2020/01/finaloutput.png)  

Congratulations! You have just run your first program with Jupyter Notebook.  

### Example Programs with Jupyter Notebook

#### Check If Leap Year 
Run jupyter and like before, make a new notebook.  

First we'll explain what the progtram does and add soem information on the subject.

1. Select the dropdown that says **code** and change it to **markdown**  

![switch to markdown](https://codeswag.co.uk/wp-content/uploads/2020/01/newww.png)  

Here is a resource on markdown foramtting: [Markdown](https://guides.github.com/features/mastering-markdown/) 

2. Next, we write the explanation then press **Alt + Enter** to run and insert a cell below

![leapyear 1](https://codeswag.co.uk/wp-content/uploads/2020/01/leap1.png)

3. Writing the code
     First we need to get user input, type this line of code and press **Alt + Enter**: 
     ```py
     year = int(input("Enter a year to check: "))
    ```
    In the next cell we add the rest of the code for the program. Type this and press **Shift + Enter**:
    ```py
    if (year % 4) == 0:
        if (year % 100) == 0:
            if (year % 400) == 0:
               print("{0} is a leap year".format(year))
           else:
               print("{0} is not a leap year".format(year))
       else:
           print("{0} is a leap year".format(year))
    else:
       print("{0} is not a leap year".format(year))
    
    ```


![leapyear 2](https://codeswag.co.uk/wp-content/uploads/2020/01/leap2.png)

4. Running the program.  

   To run the program, select **Cell** in the menu bar then **Run All**

![leapyear 3](https://codeswag.co.uk/wp-content/uploads/2020/01/leap3.png)
You can find the source code of these examples [here](https://github.com/Psypher1/Codeswag-Tutorials/tree/master/Code%20Files)


#### Shipping Calculator
Run jupyter and make a new notebook

1. Explanation of the code.  

   Change the first cell to markdown> Explain the code then press **Alt+Enter***

![explaining the program](https://codeswag.co.uk/wp-content/uploads/2020/01/ship1.png)

2. Writing the code.  

   We start by declaring our variables. Type this aand press **Alt + Enter**:
   ```py
   purchaseAmt = 0
   shippingCharge = 0
   totalWithShipping = 0
   ```
   Then we will get user input.Type this and press **Alt + Enter**:
   ```py
   purchaseAmt = float(input("How much did you pay?: "))
   ```
![variables and input](https://codeswag.co.uk/wp-content/uploads/2020/01/ship2.png)

   After that we write more of the code. Type this and press **Alt + Enter**:
   ```py
   if purchaseAmt >= 50 :
       shippingCharge = 0
   else:
       shippingCharge = 10

   # Calculate total including shipping
   totalWithShipping = purchaseAmt + shippingCharge
   ```

   Lastly the code to get output
   ```py
   print("Your total, including shiping is: $%.2f" %totalWithShipping)
   ```
 ![code and output](https://codeswag.co.uk/wp-content/uploads/2020/01/ship3.png)

3. Running the program. 

   To run the program, do the excat same as the first example, select **Cell** in the menu bar then **Run All**

#### Solve Quadratic Equation  
Like in the previous example run Jupyter, make a new notebook an change the first cell to markdown

1. Explaining the equation and how to solve it.  

   First we explain our code and the eqaution
   
   To write  formaula and eqautions you have to enclose them in dollar signs: `$[equation]$` and to have them inline you enclose in two of them `$$[equation]$$`
   
   To have it ouput as shown, you have to write this in the markdown cell you made: `$$ ax^2 + bx + c = 0 $$`

    When you have entered the information for the first cell, press **Alt + Enter**
    
    Change this nnext cell to markdown. Here we will output how the equation is solved. Type this and press **Alt + Enter**:
    `$$ x = \frac{-b + \sqrt(b^2-4ac)}{2a} $$`
    
    `$$ x = \frac{-b - \sqrt(b^2-4ac)}{2a} $$`
    



![quadratic 1](https://codeswag.co.uk/wp-content/uploads/2020/01/quad1.png)

Here is a resource that explains how to write mathematical formulas in jupyter: [Jupyter Mathematical Formula](https://csrgxtu.github.io/2015/03/20/Writing-Mathematic-Fomulars-in-Markdown/)

2. Writing the code.  

   We are going to write a function for this program. We'll start by importing a module Type this:
   ```py
    import cmath
   ```
   Then type this for the function and press **Shift + Enter**:
   ```py
   def quad():
       a = int(input("Please enter the first coeffeicient: "))
       b = int(input("Please enter the second coeffeicient: "))
       c = int(input("Please enter the third coeffeicient: "))
    
        # calculate the discriminant
       disc = (b**2) - (4*a*c)
    
    # find two solutions
       sol1 = (-b-cmath.sqrt(disc))/(2*a)
       sol2 = (-b+cmath.sqrt(disc))/(2*a)
    
       print("\nThe positive value is {}".format(sol2) )
       print("The negative value is {}".format(sol1) )
   ```
   Press **Alt+ Enter** and in the next cell we call our function:
   ```py
   quad()
   ```
![quadratic 2](https://codeswag.co.uk/wp-content/uploads/2020/01/quad2.png)

3. Running the program.  

  To run the program do the same as in the first example,select **Cell** in the menu bar then **Run All**
![quadratic 3](https://codeswag.co.uk/wp-content/uploads/2020/01/quad3.png)




##### Additional Information  

Jupyter is made of cells and has two modes:  

**Edit Mode**: When you write your code.  

**Command Mode**: When you run the code. 

Lastly, below the __Help__ menu is a list of very useful keyboard shortcuts that will greatly improve your workflow.

