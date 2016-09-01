GGG: Git, GitHub, and Geostats2016
==========================



What are Git and GitHub? 
------------------
Git is "a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency." This translates to a program that makes it easy to track your code (e.g. R) changes over time, save and switch to previous versions, and allows you to collaborate with others without causing conflict.

GitHub is the service that hosts all of the files that are tracked through Git. Think of it like Google Docs, but for code and data.

Installing GitHub
-----------------------
You can find downloads for both Windows and Mac at https://git-scm.com/

* **Windows:**
    * Click "Download for Windows" on the right side of the page.  
    * Install and follow the installer instructions
    * Git should now be installed
* **Mac:** 
    * First download and install Xcode (it is quite large ~ 3.8 GB) from http://itunes.apple.com/us/app/xcode/id497799835
    * Once you have Xcode installed, open the terminal app (click applications > utilities > terminal).
    * Type the following command:
    *     xcode-select --install
    * Click the install button to install the developer tools.
    * You may want to add the terminal app to your dock at this point. You can do this by right-clicking terminal and clicking options > add to dock.
    * At this point git should be installed. You can test it by typing: 
    *     git --version
    * **If** you are getting errors about admin privileges, type the following command and accept the license:
    *     sudo xcodebuild -license
Setup Class Folder and GitHub
-------------
First you need a place to store the files that you will be 'pulling', or downloading, from GitHub. This is called your 'local repository', which is a copy of the 'master repository' on GitHub. Create it somewhere easy to get to, and remember the filepath to it, for example:

    C:\Geostats2016\

'Clone' - Downloading Class Data for the 1st Time
-------------
Once you've created the folder, it's time to download the data from GitHub into it. This is called cloning, and is done once when copying a repository to any machine. You do this by using the Command Prompt (Windows) or Terminal (Mac). **The following only has to be done once; the very first time you download**:

**Windows (Command Prompt)**:  
* Click the Start button and type into the box (Quick Search on Win7, or Ask Me Anything on Win10):
*     cmd
* Once you have the Command Prompt open, type 'cd' followed by the full filepath of the folder you created for Geostats. This will put you in that folder.
*     cd C:\Geostats2016\
* Alternatively, you can type 'cd' and then drag the folder from Windows to the Command Prompt to copy the filepath into Command Prompt.  

**Mac (Terminal)**:
* Open Finder and go to Applications, then to Utilities, and open Terminal
* Once you have Terminal open, type "cd " (include the space after cd) and then drag the Geostats folder you created into Terminal, and press Enter. This will put you in that folder.
*     cd [Drag and Drop Folder]

**Cloning:**
* Now it's time to use Git to 'clone', or download the files for the first time, from Github:
*     git clone https://github.com/wu16/geostats2016 .
    DO NOT forget the space and period after the URL. That means it creates the files in the folder that you're currently. in.  

* Now you have a local copy of the folder from GitHub on your computer!  
It **will not** automatically update. You will need to do Git 'pulls' to get the most up-to-date copy of the repository (see below).


'Pull' - Updating the Class Data to Current Version
-------------
Open Command Prompt or Terminal like you previously did, and navigate to the folder again. This time, once you're in the folder, you have to go into the repository subfolder, do this by typing:  

    cd geostats2016
    
Once you're in the repository folder, type the following to update to the latest version:

    git pull
    
That's it! Now you have the latest version of the class data. You will need to do this regularly to keep the files up-to-date.

Additional Resources and Information
------------------------------------
* 15-Minute Interactive Intro to GitHub: https://try.github.io/levels/1/challenges/1

* Git has integration with RStudio and is incredibly useful in maintaining various versions of R code without having to constantly save and keep track of files. It even has a GUI interface so you don't have to use the Command Prompt or Terminal. This can be done by following this tutorial: https://support.rstudio.com/hc/en-us/articles/200532077-Version-Control-with-Git-and-SVN

* GitHub manual: https://git-scm.com/book/en/v2

 
*Adapted by Tyler Hardy from tutorials found on https://git-scm.com/book/en/v2/Git-Basics-Getting-a-Git-Repository  
Mac installation instructions by Jason Tilley*
