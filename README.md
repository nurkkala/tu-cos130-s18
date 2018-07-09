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

    `brew install gcc`

   This will generate quite a lot of output and may take a while depending on the speed of your Internet connection, etc. Homebrew is installing a bunch of tools and programs that will allow you to compile and execute C programs.
