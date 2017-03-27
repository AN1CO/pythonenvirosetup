# Set up Environment for Python on Mac

### You only have to do this once!

In the terminal:

##### Step 1
`brew install python3`

This installs a new clean copy of Python 3 so it doesn't interfere with any Python that might be used on your system.

##### Step 2
`brew install tree`

Tree commands lists content in directories like a file tree, so it looks prettier and easier to read. This is just an add-on that will make things easier to read, not really necessary. More about tree commands [here](http://www.computerhope.com/unix/tree.htm).

##### Step 3
`pip3 install ipython`

iPython is a command shell, like Ruby's irb. The command shell that ships with Python sucks, so use this.
`pip3` is the command for Python3, this is important because you don't want to install stuff for the regular Python (you will get errors).

##### Step 4
`pip3 install virtualenv`
`pip3 install virtualenvwrapper`

virtualenv helps you create isolated environments for your Python. Every time you start a new project in Django or any other Python project, you will want to create a new environment for it. More information about commands for it [here](http://docs.python-guide.org/en/latest/dev/virtualenvs/).

##### Step 5
After installing everything, type this in your terminal:

`atom ~/.bash_profile`

if you don't have a bash profile file yet:
`touch ~/.bash_profile`

then open it up in Atom or whatever your preferred text editor is.

######Step 6######


######Step 7######
