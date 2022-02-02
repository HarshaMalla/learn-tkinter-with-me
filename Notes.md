# <mark>The Tkinter Module </mark>





## What is Tkinter ?

Tkinter provides Python applications with an easy-to-program user interface. Tkinter supports a collection of Tk widgets that support most application needs. Tkinter is the Python interface and GUI toolkit for Tcl/Tk. Tcl/Tk is the scripting , graphics facility and Tkinter was a pre-installed library in python , so we don't need to install manually. 

## What are Widgets in Tkinter?

Widgets in Tkinter are the elements of GUI application which provides various controls (such as Labels, Buttons, ComboBoxes, CheckBoxes, MenuBars, RadioButtons and many more) to users to interact with the application.



## Ok , Let's create a  small Tkinter window for better understanding

```python
from tkinter import *
root = Tk()
root.title("Demo_program")

label = Label(root, text ="Hello World !").pack()

root.mainloop()


```

#### Don't Panic here's the comments for code :)

### Code Comments :

1. <mark>from tkinter import *</mark>
   
   From module Tkinter import everything or all (*)

2. <mark>root = Tk()</mark>
   
   Tkinter works by starting a tcl/tk interpreter under the covers, and then translating tkinter commands into tcl/tk commands. The main window and this interpreter are intrinsically linked, and both are required for a tkinter application to work.**"Creating an instance of `Tk` initializes this interpreter and creates the root window."**

3. <mark>root.title("Demo_program")</mark>
   
   Title of the main window ( Take a look at output window below for clear clarification)

4. <mark>label = Label(root, text ="Hello World !").pack()</mark>
   
   Label is what output will be shown on the window , The pack() geometry manager **organizes widgets in blocks before placing them in the parent widget**

5. <mark>root.mainloop()</mark>
   
   root. mainloop() is **a method on the main window which we execute when we want to run our application**. This method will loop forever, waiting for events from the user, until the user exits the program

#### Output :

![](C:\Users\91944\AppData\Roaming\marktext\images\2022-02-02-21-05-49-image.png)
