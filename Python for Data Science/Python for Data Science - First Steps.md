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

![upgrading pip](https://codeswag.co.uk/wp-content/uploads/2020/01/up-to-date-pip.png)


**Next, Type the following and press enter**
`pip install jupyter`  

![installing jupyter](https://codeswag.co.uk/wp-content/uploads/2020/01/installjupyter.png)  

And that’s it! you’re ready to use Jupyter.

##### Running Jupyter Notebook
I recommend creating a folder for all your notebooks on your computer. This can also be done within the Jupyteri interface.  

To run Jupyter simply open your terminal and type the following and press enter. It will open a window in your browser after.  

`jupyter notebook`  

![run jupyter](https://codeswag.co.uk/wp-content/uploads/2020/01/run-jupyter.png)


##### Your First Program
As is customary we are going to write a **“Hello World!”** program. 
Navigate to the folder you created and then select new then Python3. A new window will be opened thereafter. 

![new program](https://codeswag.co.uk/wp-content/uploads/2020/01/new-note.png)

**In the next window, type `print(“Hello, World!”)` then click run**  
![the new notebook](https://codeswag.co.uk/wp-content/uploads/2020/01/first-book.png)  

**Your window should look like this afterward:**
![the output you should get](https://codeswag.co.uk/wp-content/uploads/2020/01/hello-jupyter.png)  

Congratulations! You have just run your first program with Jupyter Notebook.  


##### Additional Information  

Jupyter is made of cells and has two modes:
**Edit Mode**: When you write your code
**Command Mode**: When you run the code 

Lastly, below the __Help__ menu is a list of very useful keyboard shortcuts that will greatly improve your workflow.

