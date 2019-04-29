# Development
The SCIs are made on a two weekly or monthly basis. If, however, you want to follow the development of 1.13 as close as possible or maybe even help, you can compile the executable of 1.13 yourself and combine this with the latest game data.

## 1 SVN
The 1.13 development takes place on a so called Subversion server which from here we will call SVN. This software gives developers to possibility to collaborate on the project at the same time without losing any valuable work.  
SVN needs a client to be able to make use of its features, for Windows this client is [TortoiseSVN](https://tortoisesvn.net/downloads.html).

After installing TortoiseSVN you can create a new folder in any place and right click it, the context menu should show you an option called `SVN Checkout...`, when you click this a window will open, read on for further directions.

### 1.1 the 1.13 source code
To checkout the 1.13 executable source code with SVN you will have to fill in the following URL of the SVN repository: `https://ja2svn.mooo.com/source/ja2/trunk/GameSource/ja2_v1.13/Build`  
Make sure the value for `Checkout directory` is the directory that you want to place the SVN copy in, leave other settings as they are and press OK.  
The source code repository is just above 1GB in size, depending on your internet speed it could take a while for the SVN data to download, once it's done you will see the message `Completed` at the bottom of the activity window.

### 1.2 the 1.13 game data
The game data files are also located in a SVN repository at the following URL: `https://ja2svn.mooo.com/source/ja2_v1.13_data/GameDir`  
Also make sure that the `Checkout directory` is correct and leave the other settings as they are and press OK.  
The game data repository is close to 2GB in size, depending on your internet speed it could take a while to download.

## 2 Compiling the game executable
TODO  
Jagged Alliance 2 is coded in a mixed style C/C++, the best development environment to use for this is Microsoft Visual Studio, a free version is available at https://visualstudio.microsoft.com/vs/express/
You can pick from many versions of Visual Studio Express like 2005, 2008, 2010, 2013 or 2017.
