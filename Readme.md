# Setting up your development environment

Setting up your development environment is the process you undergo to get your comuputer ready for software development.
Programming can be done on any form of computer but most require some initial setup to have the languages
and tools of your choice installed and ready for use.

This first guide will involve setting up a Python development environment as the first few projects will use the
Python programming language. When later projects use a different language guides will be provided on how to install
those environments as well.

Each project will have a few key components:

* Project description
* Programming language and associated libraries
* Runtime environment
* Tests

Well actually every project is going to be packaged in a [Docker container](https://docs.docker.com/get-started/overview/)
so you don't technically have to install anything other than Docker to run these projects locally. Nevertheless you'll probably
want to run programs at some point that aren't in containers so we'll walk you through setting up a Python environment with:
* The Python programming language
* Poetry a tool for managing Python libraries and dependencies
* Docker desktop

We'll also suggest some IDEs you can try.

#### Mac users

Mac users will want to install [Homebrew](https://brew.sh/) to make it easier to install different languages and software packages

#### Windows users

Unfortunately most programming resources out there are written primarily for developers using a computer with a Unix based operating system.
That means many instructions you'll see may have less robust, out of date, or even missing instructions on how Windows users
can set up their development environment. However you don't need a Unix machine to code. I started with Windows and you certainly can too.

Here are a few options you have:

* Just develop on Windows anyways. Docker has support for Windows so you will be able to do all of these projects on Windows. 
Additionally most of the important technologies can be developed on Windows. Though you will want to become very familiar with
  [Powershell](https://docs.microsoft.com/en-us/powershell/) which is Windows version of the terminal. It can do everything you need
  but has different syntax than the Unix/Linux terminal shell programs use so you will have to adjust some scripts to get them
  to work on your machine. Just get comfortable searching "How do I do X in Powershell?"

* You could [set up a dual boot Linux installation](https://itsfoss.com/install-ubuntu-1404-dual-boot-mode-windows-8-81-uefi/)
on your computer. This would let you run both Windows and Linux on the same machine.
  
* You can use virtual machines like [Virtualbox](https://www.virtualbox.org/) as another way to run a different operating system
on your machine without doing a dual boot and partitioning your hard drive.
  

#### Linux users

If you use Linux as your operating system you've already learned how to install things through the terminal on your own and
troubleshoot when things go wrong.


## Git

Before we get started everyone needs to install [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git) if you have not already.
We will be using version control via Git for all projects.

## Installing Python

Python is an interpreted programming language. It is used for everything from basic scripts to web development to machine learning.
It is a great language to program in and a good choice to start with. I'd reccomend downloading the most recent version of Python.
As of this writing that is 3.9.5


Many computers running either Mac or Linux come with Python 2.7 the older and unsupported version of the langauge installed.
So we will want to install Python 3 which is the version we'll use for our Python projects.


[Download Python](https://www.python.org/downloads/)

###Installing a specific version of Python

One of the challenges with the Python programming languages is that sometimes a third party library or piece of software 
you need to use may require a different version of Python than your main installation has. 
So you may end up needed more than one version of Python on your computer. Virtual environments help with this problem
by providing a tool to switch between different Python environments seamlessly. 

[This article](https://akrabat.com/creating-virtual-environments-with-pyenv/) provides good instructions on how to set up
virtual environments on Linux and Mac

###Poetry

[Poetry](https://python-poetry.org/) is a package manager for Python. It is very helpful for managing dependencies within
your projects and virtual environments. Poetry works on Mac, Linux and Windows. Follow the link above and the installation 
instructions for your operating system. I prefer it over other Python package managers like Pip and Conda because I believe
that Poetry handles package management on version controlled projects better and makes it easier to collaborate with other developers.

## Installing Docker Desktop

Docker is a technology that let's you run programs in "containers." A container is a lightweight abstraction of an
operating system that you can run anywhere Docker is installed. I like to think of it as a tiny computer that I can setup
exactly how I need to run a specific piece of software. This is really helpful when it comes to developing, testing and deploying
software because you can simulate a lot of different systems and system configurations right on your laptop. As you'll learn
the further you get into programming there are a lot of different operating systems, libaries and other pieces of software
your program may need to run, so it can save you a lot of time and headache to be able to separate the runtime environment from the hardware.
This means you can have different environments easily on the same machine as well as deploy the same programs on different hardware.

Anyways follow the instructions in [this link](https://www.docker.com/get-started) to install Docker Desktop

## IDEs

IDE stands for [Integrated Development Environment](https://en.wikipedia.org/wiki/Integrated_development_environment)

There are many to choose from. The important thing to know is that they can help you write and test your code.

Personally I write most of these projects using IDEs from [Jetbrains](https://www.jetbrains.com/). I like the Community
Edition version of [PyCharm](https://www.jetbrains.com/pycharm/) which is free and sufficient for teaching yourself how to code.

Here are some other options you can consider:

* [Vim](https://www.vim.org/): a configurable text editor that has remained popular for software development for decades. 
It may seem barebones but it has a lot of capabilities and can be easily used to edit code on remote machines.
  
* [Emacs](https://www.gnu.org/software/emacs/): an open source text editor. I started programming with Emacs myself.
Simple tools like Emacs and Vim can be helpful for beginners because there aren't many bells and whitsles to distract you
  from the code

* [XCode](https://developer.apple.com/xcode/): Apple's IDE for Macs only I believe

* [Visual Studio](https://visualstudio.microsoft.com/): Microsoft's multi-language IDE with versions for Windows, Linux and Mac