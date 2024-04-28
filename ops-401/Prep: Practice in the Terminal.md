**The Command Line - What is it, how does it work and how do I get to one.**
* A command line, or terminal, is a text based interface to the system. You are able to enter commands by typing them on the keyboard and feedback will be given to you similarly as text. The command line typically presents you with a prompt. As you type, it will be displayed after the prompt. Most of the time you will be issuing commands.
  
| OS      | Opening a Terminal |
| ------- | ---------------- |
| Mac     | Applications -> Utilities. Or key combination "command ( ⌘ ) + space", which will bring up Spotlight,then start typing Terminal.|
| Linux   |  Applications -> Systems or Applications -> Utilities. Alternatively you able to 'right-click' on the desktop and there may be an option 'Open in terminal.'|
| Windows | If on windows and intend to remotely log into another machine then you will need an SSH client.|

**Basic Navigation - An introduction to the Linux directory system and how to get around it.**

  | Commands | Description |
  | -------- | ----------- |
  | pwd      | Print Working Directory - ie. Where are we currently.|  
  | ls       | List the contents of a directory.|
  | cd       | Change Durectoreis - ie. move to another directory.|

**More About Files - Find out some interesting characteristics of files and directories in a Linux environment.**
* Everything is a file under Linux. Even directories.
* Linux is an extensionless system. Files can have any extension they like or none at all.
* Linux is case senstitive.

**Manual Pages - Learn how to make the most of the Linux commands you are learning.**
* Instead of trying to remember everything, remember you can easily look stuff in the man pages.
  
| Commands | Description |
| -------- | ----------- |
| man 'command'| Look up the manual page for a particular command |
| man -k 'search term'| Do a keyword search for all manual pages containing the given search term.|
| /'term'| Within a manual page, perform a search for 'term'|
| n | After performing a search within a manual page, select the next found item.|

**File Manipulation - How to make, remove, rename, copy and move files and directories.**
| Commands | Description |
| -------- | ----------- |
| /mkdir| Make Directory -ie. Create a directory.|
| /rmdir| Remove Directory -ie. Delete a directory.|
| /touch| Create a black file.|
| /cp| Copy - ie. Copy a file or directory.|
| /mv| Move - ie. Move a file or directory (can also be used to rename).|
| /rm| Remove - ie. Delete a file.|

**Cheat Sheet - A quick reference for the main points covered in this tutorial.**

<details><summary><h4>Basic Navigation</h4></summary>
  <dl> 
    <dt> pwd </dt>
     <dd>Where am I in the system.</dd> 
    <dt> ls [path] </dt>
      <dd>Perform a listing of the given path or your current directory.</dd> 
      <dd>Common options: -l, -h, -a</dd>
    <dt> cd [path] </dt>
      <dd>Change into the given path or into your home directory.</dd> 
    <dt> Path </dt>
      <dd>A description of where a file or directory is on the filesystem.</dd> 
    <dt> Absolute Path </dt>
      <dd>One beginning from the root of the file system (eg. /etc/sysconfig ).</dd> 
    <dt> Relative Path </dt>
      <dd>One relative to where you currently are in the system (eg. Documents/music ).</dd> 
    <dt> ~ (tilde) </dt>
      <dd>Used in paths as a reference to your home directory (eg. ~/Documents ).</dd> 
    <dt> . (dot) </dt>
      <dd>Used in paths as a reference to your current directory (eg. ./bin ).</dd> 
    <dt> .. (dot dot) </dt>
      <dd>Used in paths as a reference to your current directories parent directory (eg. ../bin ).</dd> 
    <dt> TAB completion </dt>
      <dd>Start typing and press TAB. The system will auto complete the path. Press TAB twice and it will show you your alternatives.</dd> 
</dl>
</details>

<details><summary><h4>More About Files</h4></summary>
  <dl>
    <dt> /file [path] </dt>
      <dd>Find out what type of item a file or directory is.</dd> 
    <dt> Spaces in names </dt>
      <dd>Put whole path in quotes ( " ) or a backslash ( \ ) in front of spaces.</dd> 
    <dt> Hidden files and directories </dt>
      <dd>A name beginning with a . (dot) is considered hidden.</dd> 
</dl>
</details>

<details><summary><h4>Manual Pages</h4></summary>
  <dl>
    <dt>man <command></dt>
    <dd>View the man page for a command.</dd>
    <dt>man -k (search term)</dt>
    <dd>Search for man pages containing the search term.</dd>
    <dt>Press q to exit man pages</dt>
  </dl>
</details>

<details><summary><h4>File Manipulation</h4></summary>
  <dl>
    <dt>mkdir (directory name)</dt>
    <dd>Create a directory</dd>
    <dt>rmdir (directory name)</dt>
    <dd>Remove a directory (only if empty).</dd>
    <dt>touch (file name)</dt>
    <dd>Create a blank file.</dd>
    <dt>cp <source> <destination></dt>
    <dd>Copy the source file to the destination.</dd>
    <dt>mv <source> <destination></dt>
    <dd>Move the source file to the destination.</dd>
    <dd>May also be used to rename files or directories.</dd>
    <dt>rm <path></dt>
    <dd>Remove a file or directory.</dd>
    <dd>Common options: -r -f</dd>
  </dl>
</details>

<details><summary><h4>Permissions</h4></summary>
  <dl>
    <dt>r (read) w (write) x (execute)</dt>
    <dt>Owner or User, Group and Others</dt>
    <dt>ls -l [path]</dt>
    <dd>View the permissions of a file or all items in a directory.</dd>
    <dt>chmod <permissions> <path></dt>
    <dd>Change permissions. Permissions can be either shorthand (eg. 754) or longhand (eg. g+x).</dd>
  </dl>
</details>

<details><summary><h4>Useful Commands</h4></summary>
  <dl>
    <dt>du -sh ./*</dt>
    <dd>Find the size of every directory in your current directory.</dd>
    <dt>df -h</dt>
    <dd>Display how much disk space is used and also free.</dd>
    <dt>basename -s .jpg -a *.jpg | xargs -n1 -i cp {}.jpg {}_original.jpg</dt>
    <dd>Make a copy of every jpg image file in the current directory and rename adding _original.</dd>
    <dt>find /home -mtime -1</dt>
    <dd>Find all files in the given directory (and subdirectories) which have been modified in the last 24 hours.</dd>
    <dt>shutdown -h now</dt>
    <dd>Shutdown the system. (Replace -h with -r for reboot.)</dd>
  </dl>
</details>

<details><summary><h4>Process Management</h4></summary>
  <dl>
    <dt>CTRL + C</dt>
    <dd>Cancel the currently running process.</dd>
    <dt>kill (process id)</dt>
    <dd>Cancel the given process.</dd>
    <dd>Include the option -9 to kill a stubborn process.</dd>
    <dt>ps</dt>
    <dd>Obtain a listing of processes and their id's.</dd>
    <dd>Including the option aux will show all processes.</dd>
    <dt>CTRL + Z</dt>
    <dd>Pause the currently running process and put it in the background.</dd>
    <dt>jobs</dt>
    <dd>See a list of current processes in the background.</dd>
    <dt>fg (job number)</dt>
    <dd>Move the given process from the background to the foreground.</dd>
  </dl>
</details>

