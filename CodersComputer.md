# Notes: The Coder's Computer

The following are some notes as to why and how coder's select and use certain text editors.

## **Tools for Writing Code**

### What is a text editior?

A text editor is any program where one writes code. A major key for a text editor is that it does not contain formatting options. No need to **bold** or *italicize* text. This disqualifies Microsoft Word. At the end of the day, you can write code in any text editor, but there are features that can help you be more productive, efficient, and less prone to errors. Some of these features are:

  - Code Completion
  - Syntax Highlighting
  - Visual Themes
  - Extensions
  
#### Code Completion

  - This is when you begin to type a command or function and the text editior recognizes what you are doing and provides a drop down with possible choices. Very helpful for 
  speed, or maybe if you forgot the exact name of something. 
  - Also helps with bracket and quotation closing management.

#### Syntax Highlighting

  - This feature colors different *types* of code different colors. This allows the user to see what code is commented out, what is a function, what is a variable, an object,
  and so forth. 
 
#### Visual Themes
 
  - You need really cool dark modes so when your co-workers walk by they think you are using some super advanced software that they don't know about.
  - That was a joke. While they do look cool, the purpose of visual themes is really to be easier on the eyes since you will be staring at the screen for long periods of time.

#### Extensions

  - Extensions are like plugins that you can add for more functionality. 
  - Since these extensions can help you grow the capabilities of your text editor as you progress in your career, it is important to select one with a good selection of extensions from the start, so you do not find yourself needing to switch text editors too often later.
 
### What is an IDE?

- IDE stands for *Integrated Development Environment*.
- An example is [PyCharm](https://www.jetbrains.com/pycharm/).
- This is a software suite with text editing capabilities but also more, such as:
  - Debugger
  - Code Compiler
  - File Manager
  
## **Using the Terminal**

### The Command Line

The Linux terminal (or Windows WSL) is essentially the file management system of your computer without the GUI manager like Windows Explorer. 

- Perhaps the most useful command is **pwd**, which will show you the absolute path of where you are currently located.

Speaking of absolute path, this is like the entire file path copied from the URL line in Windows Explorer. On the other hand, the relative path is just the name of the folder you are are referring to, within the scope of the current location. 

- For example, absolute path of a "Pictures" folder could be C://Documents/MyStuff/Pictures, and the relative path (if located in C://Documents/MyStuff) would just be Pictures. If you were located at absolute path C://Documents, then the relative path would be MyStuff/Pictures. And so forth.

#### More Useful Commands

- To show the contents of a folder, use the command **ls**, which stand for *list*. Example: **ls C://Documents/MyStuff/Pictures**.

- To change directories, use **cd**. This is the same as the Windows command for the same task.

  - For example, if located in C://Documents, and you wanted to move to the Downloads folder, you would type **cd C://Downloads**.
  
### Files

Linux does not use file extensions, like Windows does. No more .txt, .exe,.jpg, etc. Instead, the OS looks inside the file to know what type of file it is and thus how to treat it.

- If you want to see what file type a given file is, use the command **file[path]**.

### Case Sensitive

Linus is case sensitive. So, for example you could have have two Documents folders in the same directory - one called *Documents* and one called *documents*.
  
