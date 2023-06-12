# Linux Bourne Again Shell. Bash.

## [The Command Line](https://ryanstutorials.net/linuxtutorial/commandline.php)

Linux bash, or the "Bourne Again Shell," is a command-line interpreter and scripting language used in Linux and Unix-based operating systems. It provides users with a textual interface to interact with the operating system and execute various commands.

The bash shell works by reading and executing user commands entered via the command line. When you enter a command, the shell interprets it and communicates with the operating system to carry out the requested action. It supports a wide range of commands, utilities, and programming constructs, allowing users to perform tasks such as file manipulation, process management, system configuration, and more.

To access a bash shell, you need to open a terminal emulator on your Linux system. Here's how you can do it:

 1. Graphical Interface: If you're using a Linux distribution with a graphical user interface (GUI), you can typically find a terminal application in the "System Tools," "Utilities," or similar category of your application launcher. Click on the terminal icon to launch it, and you'll have access to a bash shell.

 2. Keyboard Shortcut: Many Linux distributions provide a keyboard shortcut to quickly open a terminal. The default shortcut is often Ctrl + Alt + T, but it can vary depending on your specific distribution or customization.

 3. Menu Navigation: Some Linux distributions organize their applications into hierarchical menus. You can navigate through these menus to find the terminal application. Look for categories like "System," "Utilities," or "Accessories" to locate the terminal.

 4. Command Line Login: If you're using a Linux system without a graphical interface, such as a server or a minimal installation, you'll typically have a command-line login prompt. After logging in with your username and password, you'll directly enter a bash shell.

Once you've opened a terminal and accessed the bash shell, you can start entering commands and executing them by pressing the Enter key. The shell will interpret your commands and provide the corresponding output or perform the requested action. You can use various command-line tools, utilities, and options to accomplish specific tasks efficiently.

## [Basic Navigation](https://ryanstutorials.net/linuxtutorial/navigation.php)

This segment starts by introducing the concept of a file system hierarchy in Linux. It explains that the file system is organized in a tree-like structure, with the root directory ("/") at the top. All other directories and files are located within this structure.

It covers the following commands:

  1. `pwd`: This command stands for "print working directory" and displays the current directory you're in.

  2. `ls`: This command lists the files and directories in the current directory. It can be customized with various options to show additional information such as file permissions, timestamps, and sizes.

  3. `cd`: This command is used to change directories. You can use it to navigate to a specific directory by providing the directory's path as an argument.

  4. Relative and Absolute Paths: The tutorial explains the difference between relative and absolute paths. Relative paths are specified relative to the current directory, while absolute paths start from the root directory.

  5. `.` and `..`, These are special directory names. `.` refers to the current directory, while `..` refers to the parent directory.

  6. Tab Completion: The tutorial introduces tab completion, a handy feature that allows you to complete directory and file names by pressing the Tab key.

  7. Hidden Files: Linux hides files and directories whose names start with a dot (".") by default. The tutorial explains how to display hidden files using the `ls` command with the `-a` option.

It covers essential commands and concepts that will help you move around the file system efficiently and find your way to specific directories and files.

## [More About Files](https://ryanstutorials.net/linuxtutorial/aboutfiles.php)

Interesting concepts and characteristics of file and directories are explained here but here is what I liked...

  1. Everything is a file: In Linux, not only regular files but also directories, devices, and even hardware components are represented as files. This uniform representation simplifies the interaction with the system.

  2. File types: Linux recognizes various types of files, including regular files, directories, symbolic links, device files, named pipes, sockets, and more. Each file type has its purpose and behavior.

  3. File permissions: Linux implements a robust file permission system. Each file has permissions that define who can read, write, and execute it. These permissions can be set independently for the file owner, the group, and others.

  4. Ownership: Every file is associated with an owner and a group. The owner has specific permissions, and the group to which the file belongs also has certain permissions. These ownership attributes allow for fine-grained access control.

  5. File size: Files in Linux have varying sizes, ranging from empty files to several terabytes or more. The `ls` command displays the size of files in bytes, but you can use various options to present the size in a more readable format.

  6. File timestamps: Each file has three timestamps associated with it: the access time (atime), the modification time (mtime), and the change time (ctime). These timestamps record when the file was last accessed, modified, or had its metadata changed.

  7. File extensions: Unlike some other operating systems, Linux does not rely heavily on file extensions to determine file types. Instead, it utilizes file metadata and content to identify file types accurately.

  8. Directories: Directories are special files that contain entries for other files and directories. They provide the hierarchical structure for organizing files in the file system.

  9. Hidden files: Files and directories whose names start with a dot (".") are considered hidden in Linux. By default, they are not displayed when using the `ls` command, but you can use the `-a` option to show them.

## [Manual Pages](https://ryanstutorials.net/linuxtutorial/manual.php)

YO! Seriously as awful as reading a manual sounds, trust.

Read the Manual Pages: The manual pages (accessed using the `man` command) provide in-depth documentation for each command. Refer to the manual pages for detailed explanations, examples, and related information. Practice reading and understanding the manual pages to gain a deeper understanding of the commands... 

..Such as experimentations...

..experiment with Command Options: Linux commands often come with a wide range of options that modify their behavior. Explore these options and experiment with different combinations to understand their effects. The `man` command can provide detailed information about command options and usage.


## [File Manipulation](https://ryanstutorials.net/linuxtutorial/filemanipulation.php)

- Making Files and Directories:

  `touch`: Create an empty file or update the access and modification timestamps of an existing file.
  `mkdir`: Create a new directory.

- Removing Files and Directories:

  `rm`: Remove files and directories.
  `rm <file>`: Remove a file.
  `rm -r <directory>`: Remove a directory and its contents recursively.
  `rmdir`: Remove an empty directory.

- Renaming Files and Directories:

  `mv`: Move or rename files and directories.
  `mv <oldname> <newname>`: Rename a file or directory.
  `mv <file> <directory>`: Move a file to a different directory.
  `mv <directory> <newdirectory>`: Rename a directory.

- Copying Files and Directories:

  `cp`: Copy files and directories.
  `cp <file> <destination>`: Copy a file to a specified destination.
  `cp -r <directory> <destination>`: Copy a directory and its contents recursively to a specified destination.

- Moving Files and Directories:

  `mv`: Move files and directories (as mentioned above). The mv command can also be used to move files and directories to a different location.