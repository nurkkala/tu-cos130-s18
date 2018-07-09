# COS 130 Summer Course

Installation instructions that follow assume a Mac.

## Set up Visual Studio Code

We'll use Visual Studio Code (VS Code) as our editor.

### Install VS Code

1. Download the installer from https://code.visualstudio.com/.
1. Unzip the downloaded file by double clicking on it in Finder.
1. From the Finder, drag the resulting file (called `Visual Studio Code`) into your `Applications` folder.
1. Run VS Code by double clicking it in the `Applications` folder

### Add VS Code Extensions

1. Open the extensions window by clicking the __Extensions__ icon (looks like a box of boxes)
1. In the search box at the top, enter `C/C++` and hit __RETURN__
1. Find the "C/C++ IntelliSense ..." extension listed from Microsoft. Click __Install__.
1. VS Code should display a window showing information about the C/C++ extension.
It has been downloaded but in order to use it, you need to reload VS Code by clicking the __Reload__ button.

## Install Homebrew and the Gnu C Compiler

Homebrew is a package manager for the Mac that makes it easy to install a huge variety of open-source software, including the Gnu C Compiler.

### Install Homebrew

1. Open a Terminal window. You can find the **Terminal** program from **Launchpad**, or you can use **Spotlight Search** and type in `Terminal`. The Terminal program gives you access to a command shell, which allows you to enter commands directly to your computer.
1. Navigate to the Homebrew home page at https://brew.sh/. Right near the top, there's a section entitled **Install Homebrew**. Copy the command that starts `/usr/bin/ruby` immeidately below the title.
1. Switch back to your Terminal window and paste the command you just copied. This will run the Homebrew installation. 
1. You may see several prompts during installation; go ahead and accept the default values.

### Install the Gnu C Compiler

You can use Homebrew to install other software. All Homebrew commands start with the word `brew`.

1. In the Terminal window (you can use the same one that you used to install Homebrew), enter this command to install the Gnu C Compiler:
   ```
   brew install gcc
   ```
   This will generate quite a lot of output and may take a while depending on the speed of your Internet connection, etc. Homebrew is installing a bunch of tools and programs that will allow you to compile and execute C programs.

### Install Other Utilities

Use Homebrew to install the following additional programs.

1. Install the Make program
   ```
   brew install make
   ```
2. Install the Git program
   ```
   brew install git
   ```

## Clone this Repository

You will need a working copy of this repository on your local machine. The Git program that you just installed is how you will get a copy of it.

1. Decide where you would like to store your working files on your Mac. You might already have a folder tree for your course work, which would work fine. The easiest place to do this is within the Finder.
1. Let's assume that you have created a folder called `Courses` in your `Documents` folder. We want to navigate to that folder _inside the Terminal command prompt_. Use the built-in **cd** command for this:
   ```
   cd ~/Documents/Courses
   ```
   where the tilde (`~`) is intepreted as your home directory.
1. Now clone this repository using Git:
   ```
   git clone https://github.com/nurkkala/tu-cos130-s18.git
   ```
1. You should find a new directory (folder) called `tu-cos130-s18` in your `Documents/Courses` directory. Change to that directory in your Terminal window:
   ```
   cd tu-cos130-s18
   ```

## Compile the Sample Program

Within the `tu-cos130-s18` folder that you cloned, you should see a file called `main.c`, which contains a trivial "hello, world" program. Let's compile and run that program.

1. From the Teminal command prompt type
   ```
   make
   ```
   This should run the Gnu C compiler, converting the `main.c` source file into an executable program called `main`.
   You should be able to see that file in the same directory (folder).
1. Run the `main` program from the Terminal shell prompt:
   ```
   main
   ```
   The program should output a simple message: `hello, world`
   If the shell can't find your `main` program, try executing it this way instead:
   ```
   ./main
   ```
   The leading `./` tells the shell to "look right in this directory" for the program.


