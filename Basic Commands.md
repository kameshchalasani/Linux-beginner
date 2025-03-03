Here’s a list of basic Linux commands you can use in Windows Subsystem for Linux (WSL):

---

### **File and Directory Management**
1. `ls`- Lists the contents of a directory.
   - `ls` : List files in the current directory.
   - `ls -l` : List with detailed information.
   - `ls -a` : Include hidden files.

2. **`cd`** - Changes directories.
   - `cd <directory>` : Move to a specific directory.
   - `cd ..` : Move up one directory.
   - `cd ~` : Go to the home directory.

3. **`pwd`** - Prints the current directory path.

4. **`mkdir`** - Creates a new directory.
   - `mkdir <directory-name>` : Create a single directory.

5. **`rm`** - Deletes files or directories.
   - `rm <file>` : Delete a file.
   - `rm -r <directory>` : Delete a directory recursively.

6. **`cp`** - Copies files or directories.
   - `cp <source> <destination>` : Copy files.
   - `cp -r <source> <destination>` : Copy directories.

7. **`mv`** - Moves or renames files.
   - `mv <source> <destination>` : Move files.
   - `mv <old-name> <new-name>` : Rename files.

---

### **File Viewing and Editing**
8. **`cat`** - Displays the contents of a file.
   - `cat <file>` : Show file contents.

9. **`nano`** or **`vim`** - Edits files.
   - `nano <file>` : Open file in Nano text editor.
   - `vim <file>` : Open file in Vim editor.

10. **`less`** - Views file contents one screen at a time.
    - `less <file>` : Open file in a scrollable view.

11. **`head`** - Displays the first few lines of a file.
    - `head <file>` : Show the first 10 lines.
    - `head -n 5 <file>` : Show the first 5 lines.

12. **`tail`** - Displays the last few lines of a file.
    - `tail <file>` : Show the last 10 lines.
    - `tail -f <file>` : Continuously show new content.

---

### **File Permissions and Ownership**
13. **`chmod`** - Changes file permissions.
    - `chmod 755 <file>` : Set permissions.

14. **`chown`** - Changes file ownership.
    - `chown <user>:<group> <file>` : Change owner and group.

---

### **Searching and Finding**
15. **`find`** - Finds files and directories.
    - `find <path> -name <filename>` : Search for a file by name.

16. **`grep`** - Searches within files.
    - `grep '<pattern>' <file>` : Search for a pattern in a file.

---

### **System Monitoring**
17. **`top`** - Displays running processes and resource usage.
18. **`htop`** - Interactive process viewer (requires installation).

19. **`df`** - Shows disk space usage.
    - `df -h` : Human-readable format.

20. **`du`** - Shows directory space usage.
    - `du -sh <directory>` : Summary of space used.

21. **`free`** - Displays memory usage.
    - `free -h` : Human-readable format.

---

### **Networking**
22. **`ping`** - Tests connectivity to a host.
    - `ping <hostname>` : Ping a host.

23. **`curl`** - Retrieves content from URLs.
    - `curl <url>` : Fetch a URL's content.

24. **`wget`** - Downloads files from the internet.
    - `wget <url>` : Download a file.

25. **`netstat`** or **`ss`** - Displays network connections.
    - `netstat -tuln` : Show listening ports.

---

### **Package Management (For Ubuntu/Debian-based WSL)**
26. **`sudo apt update`** - Updates the package list.
27. **`sudo apt upgrade`** - Installs available updates.
28. **`sudo apt install <package>`** - Installs a package.
29. **`sudo apt remove <package>`** - Removes a package.

---

### **Other Useful Commands**
30. **`echo`** - Prints text to the terminal.
    - `echo "Hello, World!"` : Display a message.

31. **`whoami`** - Shows the current user.

32. **`uname`** - Displays system information.
    - `uname -a` : Detailed system information.

33. **`clear`** - Clears the terminal screen.

34. **`exit`** - Closes the terminal session.

------------------------------------------------------
Vim is a powerful text editor used in Linux and Unix environments. Here are the basic steps to use Vim effectively:

---

### 1. **Open Vim**
   - Open a file with Vim:  
     ```bash
     vim filename
     ```
     If the file doesn’t exist, Vim will create a new one.

---

### 2. **Understand Vim Modes**
   Vim operates in several modes. The two most commonly used are:
   - **Normal mode**: Default mode for navigation and commands.
   - **Insert mode**: For typing and editing text.

   **Switch between modes:**
   - Press `i` to enter Insert mode.
   - Press `Esc` to return to Normal mode.

---

### 3. **Basic Commands in Normal Mode**
   - **Save and Exit**:
     - Save changes: `:w`
     - Exit: `:q`
     - Save and exit: `:wq` or `:x`
     - Exit without saving: `:q!`

   - **Navigation**:
     - Arrow keys or `h`, `j`, `k`, `l` for left, down, up, right.
     - `gg` to go to the beginning of the file.
     - `G` to go to the end of the file.
     - `/text` to search for `text`.

   - **Editing**:
     - Delete a line: `dd`
     - Delete a word: `dw`
     - Undo: `u`
     - Redo: `Ctrl` + `r`
     - Copy (yank): `yy` (line) or `y{motion}`.
     - Paste: `p`

---

### 4. **Insert Text**
   - Press `i` to start inserting text at the cursor.
   - Press `o` to insert a new line below.
   - Press `O` to insert a new line above.
   - Press `a` to insert text after the cursor.

---

### 5. **Search and Replace**
   - Search: `/pattern`  
     - Navigate matches with `n` (next) and `N` (previous).
   - Replace:  
     ```
     :%s/old/new/g
     ```
     This replaces all occurrences of `old` with `new`.

---

### 6. **Exit Vim**
   - Save changes and exit: `:wq` or `:x`
   - Exit without saving: `:q!`

---

### 7. **Advanced Tips**
   - **Open multiple files**:
     ```bash
     vim file1 file2
     ```
     Switch between them: `:n` (next) or `:prev`.
   - **Split window**:
     - Horizontal split: `:split filename`
     - Vertical split: `:vsplit filename`
     - Switch windows: `Ctrl` + `w` twice.

   - **Indentation**:
     - Indent: `>>`
     - Unindent: `<<`

   - **Line Numbers**:
     - Enable: `:set number`
     - Disable: `:set nonumber`

-------------------------------------------------------------------------------------

"Hacks" in the context of Linux commands often refers to clever or efficient ways to use them. Below are some Linux command "hacks" or tips to help you get the most out of your Linux experience:

---

### **File Management**
1. **Find files modified in the last 7 days:**
   ```bash
   find /path/to/directory -type f -mtime -7
   ```

2. **Delete files older than 30 days:**
   ```bash
   find /path/to/directory -type f -mtime +30 -exec rm {} \;
   ```

3. **Extract compressed files with a single command (any format):**
   ```bash
   tar -xvf file.tar.gz  # Or .tar.bz2, .tar.xz, etc.
   ```

---

### **Disk and System Monitoring**
4. **Display disk usage of current directory in a human-readable format:**
   ```bash
   du -sh *
   ```

5. **Monitor real-time system resource usage:**
   ```bash
   top  # Or use `htop` for an enhanced view
   ```

6. **Show the largest files/directories in a folder:**
   ```bash
   du -ah /path/to/directory | sort -rh | head -n 10
   ```

---

### **Networking**
7. **Check open ports:**
   ```bash
   sudo netstat -tuln
   ```

8. **Download a file from the internet:**
   ```bash
   wget http://example.com/file
   ```

9. **Test internet speed:**
   ```bash
   curl -s https://raw.githubusercontent.com/sivel/speedtest-cli/master/speedtest.py | python -
   ```

---

### **Process Management**
10. **Kill a process by name:**
    ```bash
    pkill process_name
    ```

11. **List processes by memory usage:**
    ```bash
    ps aux --sort=-%mem | head
    ```

---

### **SSH and Remote Management**
12. **Copy a file to a remote server:**
    ```bash
    scp file.txt user@remote_host:/path/to/destination
    ```

13. **Mount a remote directory via SSH:**
    ```bash
    sshfs user@remote_host:/remote/dir /local/mount/point
    ```

---

### **Productivity Hacks**
14. **Repeat a command every 2 seconds:**
    ```bash
    watch -n 2 'command_here'
    ```

15. **Quickly navigate directories:**
    Use `pushd` and `popd` to switch between directories.
    ```bash
    pushd /path/to/directory
    popd
    ```

---

### **Editing and Text Processing**
16. **Find and replace text in multiple files:**
    ```bash
    sed -i 's/old_text/new_text/g' *.txt
    ```

17. **Sort and remove duplicate lines in a file:**
    ```bash
    sort file.txt | uniq
    ```

---

### **Fun and Miscellaneous**
18. **Turn your terminal into a matrix screensaver:**
    ```bash
    cmatrix
    ```

19. **Get system uptime in a readable format:**
    ```bash
    uptime -p
    ```

20. **Display a calendar with holidays:**
    ```bash
    ncal -h
    ```

---

_____________________________________________________________________________
- $ pwd --> Display path of current working directory
- $ cd <directory> -->Change directory to <directory>
- $ cd .. --> Navigate to parent directory
- $ ls -->List directory contents
- $ ls -la --> List detailed directory contents, including hidden files
- $ mkdir <directory> --> Create new directory named <directory>
- $ cat <file> --> Output the contents of <file>
- $ less <file> --> Output the contents of <file> using the less command (which supports  pagination etc.)
- $ head <file> -->Output the first 10 lines of <file>
- $ <cmd> > <file> --> Direct the output of <cmd> into <file>
- $ <cmd> >> <file> -->Append the output of <cmd> to <file>
- $ <cmd1> | <cmd2> --> Direct the output of <cmd1> to <cmd2>
- $ clear --> Clear the command line window
- $ rm <file> Delete <file>
- $ rm -r <directory> Delete <directory>
- $ rm -f <file> Force-delete <file> (add -r to forcedelete a directory)
- $ mv <file-old> <file-new> Rename <file-old> to <file-new>
- $ mv <file> <directory> Move <file> to <directory> (possibly overwriting an existing file) $ cp <file> <directory>
Copy <file> to <directory> (possibly  overwriting an existing file)
- $ cp -r <directory1>  <directory2> Copy <directory1> and its contents to  <directory2> (possibly overwriting files in an existing directory)
- $ touch <file> Update file access & modification time (and create <file> if it doesn’t exist)

- $ chmod 755 <file> Change permissions of <file> to 755
- $ chmod -R 600 <directory> Change permissions of <directory> (and its contents) to 600
- $ chown <user>:<group> <file> Change ownership of <file> to <user> and <group> (add -R to include a directory’s contents


