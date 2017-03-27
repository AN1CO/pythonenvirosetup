# Set up Environment for Python on Mac

### You only have to do this once!

Go to your command line:

#### Step 1
`brew install python3`

This installs a fresh copy of Python 3 so it doesn't interfere with any Python that might be used on your system. Your computer ships with and uses Python to run, so you don't want to accidentally screw it up.

#### Step 2
`brew install tree`

Tree commands lists content in directories like a file tree, so it looks prettier and easier to read. This is just an add-on that will make things easier to read, not really necessary. More about tree commands [here](http://www.computerhope.com/unix/tree.htm).

#### Step 3
`pip3 install ipython`

iPython is a command shell, like Ruby's irb. The command shell that ships with Python sucks, so use this.
`pip3` is the command for Python3, this is important because you don't want to install stuff for the regular Python that is on your computer (you will get errors).

#### Step 4
`pip3 install virtualenv`

`pip3 install virtualenvwrapper`

virtualenv helps you create isolated environments for your Python. Every time you start a new project in Django or any other Python project, you will want to create a new environment for it. More about virtualenv commands [here](http://docs.python-guide.org/en/latest/dev/virtualenvs/).

#### Step 5
After installing everything, type this in your terminal:

if you don't have a bash profile file yet:
`touch ~/.bash_profile`

After you have it, open it up in Atom or whatever your preferred text editor is:
`atom ~/.bash_profile`

#### Step 6
<dl>
<dt>Copypasta this into your bash_profile and save:</dt>
  <dd>export VIRTUALENVWRAPPER_PYTHON=$(which python3)</dd>
  <dd>export VIRTUALENVWRAPPER_VIRTUALENV_ARGS='--no-site-packages</dd>
  <dd>export WORKON_HOME=$HOME/.virtualenvs</dd>
  <dd>export VIRTUALENVWRAPPER_LOG_DIR="$WORKON_HOME"</dd>
  <dd>source /usr/local/bin/virtualenvwrapper.sh</dd>
</dl>

#### Step 7 
Back in the terminal:

`source ~/.bash_profile`

#### Step 8

Great job you have your environment! Now install Django and start your project:

`mkdir django-dev`

`cd django-dev`

`mkvirtualenv -a . django-env`
Here you are creating a new virtual environment and naming it `django-env`. 
more on virtualenv commands [here](http://virtualenvwrapper.readthedocs.io/en/latest/command_ref.html).

#### Step 9

Here you can install Django! using regular `pip` command here is recommended:

`pip install django`

#### Step 10
Congrats you have your Python Environment set up!

Start using new environment with the [Django tutorial](https://docs.djangoproject.com/en/1.10/intro/tutorial01/).

