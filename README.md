# alx-system_engineering-devops
**This repository is about bash basics and permission in Linux**
*I am going to list all the commands and their uses.*

**1.** **ls** : This command lists all the files and directory in Linux.

**2.** **cd ~** : This command takes you to the home direcrory.

**3** **ls -l** : This command list all the files and directory in linux The "-l" option stands for "long format," which provides additional information about each file or directory.

**4** **ls -la** : This command list all the files and directory in linux The "-la" option displays all the hidden files begining with a **(.)**

**5** **ls -lan** : This command gives you a detailed information about all files and directories, including hidden ones, and see the numeric IDs of the owners and groups associated with each file or directory.

**6** **mkdir -p  /tmp/my_first_directory/** : This command "mkdir -p /tmp/my_first_directory/", will create the directory "my_first_directory" inside the "/tmp" directory. If the "/tmp" directory doesn't exist, the command will create it as well. The "-p" option guarantees that the command will create all necessary parent directories in the path if they are missing (mkdir is used to create a directory.

**7** **rm /tmp/my_first_directory/betty** : This command "rm /tmp/my_first_directory/betty", will delete the file named "betty" within the "my_first_directory" directory. Please note that this action is irreversible, and the file will be permanently deleted from your system. Make sure to double-check the path and the file you intend to remove before executing this command, as it does not prompt for confirmation.

**8** **rm /tmp/my_first_directory/betty** : This command "rm /tmp/my_first_directory/betty", will delete the file named "betty" located within the "my_first_directory" directory, which itself is within the "/tmp" directory.

**9** **rm -r /tmp/my_first_directory** : This command "rm -r /tmp/my_first_directory", will delete the directory named "my_first_directory" located within the "/tmp" directory. The "-r" option ensures that the command removes not only the directory itself but also all files and subdirectories within it Be sure to use this command with caution because once exacuted the delete action is permanent.

**10** **cd -** : This command is used to change the current working directory to the previous directory you were in.

**11** **ls -la . .. /boot** : This command will give the detailed listing of the current directory, the parent directory, and the contents of the /boot directory. This will include file permissions, ownership, file size, and other information about each file and directory present in those locations.

**12** **file /tmp/iamafile  $file_size** : This command will obtain the file size of a file named "iamafile" located in the "/tmp" directory and display it.

**13** **ln -s /bin/ls __ls__** : This command creates a symbolic link "__ls__" and saves it in /bin/ls.

**14** **find . -maxdepth 1 -iname "*.html" -type f | xargs -I '{}' cp -u '{}' "$(dirname "$(pwd)")"** : This command, will find all files with the extension ".html" in the current directory and copy them to the parent directory. Please ensure you have the necessary permissions to perform the copy operation and double-check the command before executing it.

**"find"** : The command used to search for files and directories.

**"."** : Represents the current directory.

**"-maxdepth 1"** : Specifies the maximum depth of the search, limiting it to the current directory only.

**"-iname "*.html""** : The option to search for files with the extension ".html" (case-insensitive).

**"-type f"** : Filters the search results to include only regular files.

**"|"** : The pipe symbol, used to redirect the output of the "find" command to the next command.

**"xargs -I '{}' cp -u '{}' "$(dirname "$(pwd)")""** : The "xargs" command is used to pass the output of the "find" command as arguments to the "cp" command. "-I '{}'" defines a placeholder for each argument. "cp -u '{}' "$(dirname "$(pwd)")"" is the command that copies the found files to the parent directory ("-u" ensures that only newer files are copied).

**100** **mv [[:upper:]]* /tmp/u** : This command is instructing the system to move all files in the current directory whose names start with an uppercase letter to the "/tmp/u" directory

**101** **rm *~** :The command "rm *~" is used to remove or delete files ending with a tilde () character in the current directory.

**102** **mkdir -p welcome/to/school** : This command will create three directories: "welcome", "to", and "school", in a nested structure. If any of these directories don't exist, the command will create them along with any necessary parent directories.

**103** **ls -la -m -p** : This command will provide a detailed list of files and directories in the current directory. The entries will be separated by commas, and directories will be indicated by a trailing slash ("/").

