---
title: "Lab: GitHub, VS Code, Python"
published: true
morea_id: experience-install-WADT
morea_type: experience
morea_summary: "Installing, configuring, and test running a local development tools"
morea_sort_order: 1
morea_start_date: 
  "Section 1": "2024-08-28T10:30"
  "Section 2": "2024-08-29T10:30"
morea_labels:
 - In Class Lab
---

{% assign repo = "ITM352_" %}
{% assign m =  "now" | date: "%-m" | times: 1 %}
{% if m <= 5 %}
{% assign repo = repo | append: "S" %}
{% else %}
{% assign repo = repo | append: "F" %}
{% endif %}
{% assign year = site.time | date: '%y' %}
{% assign repo = repo | append: year | append: "_repo" %}

# Lab objectives
After completing this lab you should be set up with and understand how to make use of the programming and development tools we will be using. In particular:
- Set up a GitHub repo for your labs and assignments. Understand the use of a repository.
- Understand what VS Code is and how to use it
- Understand what Python programs are and using VS Code to develop them

# Instructions
Try to do as many of the exercises as possible, in the order listed. You may skip an exercise if it is impossible to accomplish the task described (for technical reasons). If you have trouble with an exercise, contact the instructor for help – do not just skip the exercise! You may work with a partner, but each of you must submit your individual work. Work should be done electronically on this document (cut and paste as needed but be careful of incorrect characters). Anything that involves code should be tried out in VS Code before submitting (you may cut and paste directly from VS Code). Submit work before the next class. If you cannot submit by this time, try to do so as soon as possible.

For exercises that do not ask specific questions but have you perform tasks, copy any code you created and the output as your answer to the exercise.

# Submission
 **COPY this entire page and paste it, with your answers, into the Laulima assignment submission box for this assignment**

###  1. Creating and using a local repository
**If you have not installed the git tools or GitHub Desktop skip this exercise. Just create a folder on your desktop called  `{{ repo }}`**

  - Go to GitHub.com, sign in using your github account and select your `hello-world` repo (that you created from the [Hello World GitHub guide](https://guides.github.com/activities/hello-world/)). Go to Settings and change the repo name to `{{ repo }}`. Change the README.md if you wish. Also in the Settings page, go to the "Danger Zone" and change the repo "Make private" if it is not already set this way. Add the instructor and TA as contributors.
  - Clone this repo and open it in VS Code. You can clone it in GitHub or use GitHub desktop (or any other way you wish that works). 

*What is the URL for your GitHub `{{ repo }}`?*

*What is the path to the local `{{ repo }}`?*

###  2. Using VS Code to create a Python program
VS Code is a file editor designed to help build applications (code). Applications are built from files with instructions that the server and browser process. Let try making a simple "hello world" program and viewing it in a terminal.

  - In the repo folder, create a new folder inside called `Lab1`, create file in this folder `<your Last_First name>_hello.py`. Edit this file and put 
```Python
print("Hello from <your first name>!")
```
 **Don't forget to save this file after you make changes!**

  - Open an integrated terminal window in VS Code (you may find it easier to right-click on the file in VS Code and Open in Integrated Terminal). Type the following in the terminal:

```bash
python <your Last_First name>_hello.py 
```
  *Explain here why you see text in the terminal window. Where did this come from?*

  - Edit the file and delete the closing quote mark. Click on the PROBLEMS tab next to the TERMINAL tab in bottom VS Code window.
  
  *Explain why you see the code underlined in red and some messages in the PROBLEMS :*

  - Click on the TERMINAL window and try executing the program again. 
  
     *Explain why you see the Hello from <your first name>! and there are errors messages*

  -Put the closing quote mark back. In VS Code file manager right-click in explorer/finder, change the file extension from `.py` to `.txt`. 

  *Explain why the color of the code changed and what you can do to get it back to what you saw opreviously*

  - In the terminal, execute the program again
  - ```bash
python <your Last_First name>_hello.txt 
``` 
  
  *Explain why the code did not run and what you need to do to fix it* 

  - Change the file extension back to `.py`

  *Explain why you **do** get the Intellisense help for Python now*

###  3. Using a terminal (or command line) to access the operating system
Sometimes you will need to do more specific or detailed tasks that would be difficult or inconvenient to do through a GUI. A terminal window provides a command line interface to your operating system. There are many different types of *shell environments* such as `sh`, `csh`,`bash`, `zsh`,`cmd`, `powershell` that run in a terminal. These all have similar functionality and similar commands, but they may vary in the particular command language and syntax they use. You will find it very useful to be familiar with the basic shell commands. We will explore a few basic file system commands here needed for this class. make sure you are in the `Lab1` folder.

  a) Open a terminal in VS Code (go to the Terminal menu -> New Terminal). Identify what shell is being used:
  ```

  ```

  b) Try each of the commands below, copy the result you get and explain what the command does:
  ```
pwd

ls

mkdir newdir

cd new*

touch test

mv test test.txt

rm test.txt

echo hello > hello.txt

cat h*.txt

cd ..

rm -r newdir

history
  ```

_**NOTE: if a command doesn't work for your particular shell, look up (or guess) what the command is supposed to do and then do a Google search to find out how to do it in your shell.**_

  c) Most shells support command history. What happens if you press the uparrow key? downarrow key?

  d) Most shells support file name expansion. Try `touch xxxx.txt` then `rm xx` then hit the TAB key. What happened?

###  4. Interactive Python
In the terminal window type the following:
```
python -i
```

Now try 
```Python
print("hey! I'm using Python interactively")
```
You can quit interactive Python with
```Python
exit()
```

###  5. Remote Repo
In GitHub Desktop view the changes made in you local repo. Commit and "push" these to your repository on GitHub. Go to github.com and verify your commits have been added.

*Explain the benefits of working locally and pushing changes to a remote repository*



