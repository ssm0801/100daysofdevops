# ♾️ DevOps and 🐧 Linux Commands: A Powerful Duo🔥

Basics commands, Files and Directories operations

## 👉 Quick Intro
- Linux is open source, which means it is free and you can make any changes in the source code and use your own Linux
- Linux has multi-user support
- Linux Torvalds used Unix OS to create his own OS, which is named Linux
- It's essential to understand the fundamental Linux commands and how to use them effectively. This comprehensive guide will take you through a detailed exploration of these commands.

## 👉 Command Line Interface 🧑‍💻

CLI is like talking to a computer using special words (commands), you type in commands, and the computer does what you say. It's a bit like magic 🪄 words to make your computer do things.

*What does CLI look like?*

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698041321938/ed2d5896-8068-4278-b68f-daa06b3183b9.png)

*let's see what is written in CLI*

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698041000123/2bbdd6f8-13c2-43f8-a553-2c29da309d7a.png)

- **user name** of logged-in user
- **computer name**
- **~** is the home directory of logged-in user, which in this case is /home/ec2-user
- **#** at the end represents the root user, like the admin user in Windows
- **$** at the end represents a normal user

*pwd is a present working directory*

## 👉 Types of files

- **Ordinary File / Normal File 📝**
    - start with '-' in the ls -l command
    - contains data like text, images, audio, video, etc.
- **Directory File [folder] 📂**
    - start with 'd' in the ls -l command
    - contains all kinds of files in it
- **Link File 🔗**
    - start with 'l' in the ls -l command
    - it is a link to another file

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698048160433/4b9c2592-9848-4800-93a8-c759513a6c70.png)

*look at the first character of each line*

## 👉 Let's start with Commands ⚙️

### 1️⃣ Basics commands ✔️

`pwd` - present working directory, the current location of a user in the file structure

`cd` - change directory

`whoami` - it will display the current logged-in username

`who` - shows logged-in users of the system

`date` - display current date with time

`cal` - display calendar

`history` - get all commands that are executed in the past

`history n` - get only 'n' recent commands that are executed in the past

`man <command>` - it will give documentation of the command

`unzip <zip-file>` - extract the zip file

`tar -xvzf <tar-file>` - extract the tar file

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698042618038/99c6fdbb-09b8-4ee5-b6f5-d9e60c76271b.png)

### 2️⃣ Create or delete files and directories 📝

`touch <file>` - create an empty file

`touch <file1> <file2> ...` - create multiple empty files

`cat > <file>` - create a file with data [ctrl+d to save and exit]

`cat >> <file>` - append file with data [ctrl+d to save and exit]

`cat <file>` - display data in the file

`rm <file>` - delete file

`mkdir <dir>` - create directory

`rmdir <dir>` - delete an empty directory

`rm -d <dir>` - delete an empty directory

`rm -r <dir>` - delete a non-empty directory

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698043625065/6cdd9a23-f4ce-49ac-a80c-9bee51d8a31a.png)

### 3️⃣ File operations ⚙️

`cat file1 > file2` - copy content of file1 to file2

`cat file1 file2 > file3` - copy content of file1 & file2 to file3

`cp file1 file2` - copy content of file1 to file2

`cp -r dir1 dir2` - copy all files from dir1 to dir 2

`mv file1 file2` - rename or move file or dir

`cmp file1 file2` - display only the first difference

`diff file1 file2` - display all differences

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698044796130/20ee12fb-53f5-49d9-90d2-960f4bbed5bf.png)

### 4️⃣ List files 📃

`ls` - used to list files and dir in current dir [alphabetical order]

`ls <dir>` - used to list files and dir in a given dir

Flags

`ls -l` - list files and dir with info

`ls -r` - ordering files reversely alphabetical order

`ls -t` - list files and dir by ordering them based on modified date and time

`ls -tr` - ordering files reversely based on modified date and time

`ls -ltr`

`ls -a` - list hidden files also

`ls -R` - shows files and dir with subdirectories content

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698045077986/b4235f87-ee4c-48d9-82e9-91fb39baf811.png)

### 5️⃣ Read file data and details ✔️

`wc <file>` - display no. of lines, words, and characters in file

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698045595082/5565b6c1-b24d-4f4e-b3d8-230bb7ae6e9f.png)

`cat <file>` - display the content of the file

`cat -n <file>` : display the content of a file with line number

`tac <file>` : display the content of the file line-wise from bottom to top

`rev <file>` : each line in reverse order from top to bottom

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698045652376/7937e86e-5615-4662-824c-0d96ff83eac6.png)

`head <file>` : display top lines of file [default is 10]

`head -n <number> <file>` : display top n lines

`tail <file>` : display bottom lines of file [default is 10]

`tail -n <number> <file>` : display bottom n lines

`tail -n +<number> <file>` : display lines from nth to last

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698045929056/3755c21e-ee21-4039-aaa3-80c69931f595.png)

`grep 'text' file` : display matched lines with the file name

`grep 'text' *` : search text in all files in the current dir

`grep -n 'text'` : display matched lines with line number

`grep -l 'text'` : display only file name

`grep -i 'text'` file : search text in file [case insensitive]

`grep -R 'text'` : search text in all sub dir file

![](https://cdn.hashnode.com/res/hashnode/image/upload/v1698047705704/ab63f577-d7ff-4fa3-b0bc-c44572aedd72.png)

---

These basic Linux commands provide you with a solid foundation for navigating and managing your Linux system. As you continue your journey with Linux, you'll discover additional commands and tools that will empower you to perform more advanced tasks and streamline your system administration and development activities. Linux's robust command-line interface offers endless possibilities for customization, automation, and control, making it a powerful and versatile platform for a wide range of use cases.

**_Happy Learning !!! 👋_**