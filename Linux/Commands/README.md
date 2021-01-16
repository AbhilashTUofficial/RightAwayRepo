<details>
<summary>killall program_name</summary>
To kill the program
<pre>
eg: killall chrome
</pre>
</details>

<details>
<summary>clear</summary>
Use to clear the screen.
<pre>
eg: clear
</pre>
</details>

<details>
<summary>Print Working Directory(PWD)</summary>
Use to display the path of current directory.
<pre>
eg: pwd
</pre>
</details>

<details>
<summary>cd(change directory)</summary>
Use to change the directory
<pre>
eg: cd education
</pre>
</details>

<details>
<summary>Rename</summary>
Use to rename files.
<pre>
eg: mv file1name file2name
</pre>
</details>

<details>
<summary>Delete files</summary>
Use to delete files.
<pre>
eg: rm filename
</pre>
</details>

<details>
<summary>Delete folders</summary>
Use to rename folders.
<pre>
eg: rmdir foldername
    // only work if the folder has nothing on it.
    rm -r foldername 
    // if the folder has something.
</pre>
</details>

<details>
<summary>Find files/folders</summary>
Use to find and display the file or folder.
<pre>
eg: find filename
    find . -iname A.txt
</pre>
</details>

<details>
<summary>touch file_name</summary>
Use to create file.
<pre>
eg: touch file.txt
</pre>
</details>

<details>
<summary>ls(list)</summary>
Use to list out the directory.
<pre>
eg: ls
</pre>
</details>

<details>
<summary>touch file1 file2</summary>
Use to create multiple files.
<pre>
eg: touch file1.txt file2.txt
</pre>
</details>

<details>
<summary>touch file0 (file0 is already existed)</summary>
Use to open and close the file, useful for change the last file open time.
<pre>
eg: touch file.txt
    touch *.txt
</pre>
</details>

<details>
<summary>sudo touch /forceCommand</summary>
Use to create a flag file (file which execute on boot).
useful for run scripts on startup.
<pre>
eg: sudo touch /forcefsck
</pre>
</details>

<details>
<summary>fsck</summary>
Use to check the files, similar to chkdsk in windows.
file system check
<pre>
eg: sudo fsck
</pre>
</details>

<details>
<summary>which package_name</summary>
which display the path to the package.
<pre>
eg: sudo which google-chrome
    which cat
</pre>
</details>

<details>
<summary>ping domain -c number</summary>
ping is used to check internet connection
<pre>
eg: ping www.google.com 
    ping www.google.com -c 3
</pre>
</details>

<details>
<summary>cat</summary>
Cat read, write, and display the content into the terminal
(text files)
<pre>
eg: // read file
    cat /etc/fstab
    cat file_path
    // write file
    cat >> filename
    type the content
    // concatenate files
    cat fileone.txt >> filetwo.txt
</pre>
</details>

<details>
<summary>nano</summary>
nano is a text editor in linux.
(text files)
<pre>
eg: // read/write file
    nano /etc/fstab
    nano file_path
</pre>
</details>

<details>
<summary>less file</summary>
Use to display text content to the screen,
like cat but it is more easy to hover over long texts,
'Q' to exit.
<pre>
eg: less file.txt
</pre>
</details>

<details>
<summary>sudo blkid</summary>
Use to list all the drives on the system
with the UUID and TYPE
<pre>
eg: sudo blkid
</pre>
</details>

<details>
<summary>sudo -s</summary>
extend the sudo, and lock the terminal to the root.
type exit to exit begin a root user. 
<pre>
eg: sudo -s
    apt-get update
    apt-get upgrade
</pre>
</details>

<details>
<summary>Switch user</summary>
Use to switch between users
<pre>
eg: su user2
    cd ~
    exit
    su user1
    cd ~
    exit
</pre>
</details>

<details>
<summary>Add user</summary>
Use to add new user.
<pre>
eg: adduser name
</pre>
</details>

<details>
<summary>Delete user</summary>
Use to delete a user.
<pre>
eg: deluser name
</pre>
</details>

<details>
<summary>Add group</summary>
Use to add new group
<pre>
eg: addgroup groupname
</pre>
</details>

<details>
<summary>Add user to the group</summary>
Use to add user to a specific group.
<pre>
eg: usermod -a -G groupname username
</pre>
</details>

<details>
<summary>Delete user from the group</summary>
Use to remove user form certain group.
<pre>
eg: gpasswd -d username groupname
</pre>
</details>

<details>
<summary>Delete a group</summary>
Use to delete a group
<pre>
eg: delgroup groupname
</pre>
</details>

<details>
<summary>Change password</summary>
Use to change the password
<pre>
eg: passwd username
    passwd
</pre>
</details>

<details>
<summary>Shut down</summary>
Use to Shut down
<pre>
eg: sudo shutdown -r 15
    //reboot the system in 15 minutes
    sudo shutdown -c
    //cancel the count down
    sudo shutdown -h now
    //shut down the system
    
</pre>
</details>

<details>
<summary>Reboot</summary>
Use to Reboot
<pre>
eg: sudo reboot
</pre>
</details>

<details>
<summary>man</summary>
Use to pull out the manual for the given command
<pre>
eg: man htop
    man nano
    man neofetch
    man man
</pre>
</details>

<details>
<summary>top</summary>
Use to display the background tasks
<pre>
eg: top
</pre>
</details>

<details>
<summary>htop</summary>
Use to display the background tasks running on the system
<pre>
eg: htop
</pre>
</details>

<details>
<summary>neofetch</summary>
Use to display basic info about the system
<pre>
eg: neofetch
</pre>
</details>

<details>
<summary>Matrix</summary>
Use to display the matrix effects
<pre>
eg: cmatrix
    cmatrix -a
    cmatrix -b
    cmatrix -B
    cmatrix -r
    etc..
</pre>
</details>

<details>
<summary>figlet</summary>
Use to display the text give in screen
<pre>
eg: figlet this is cool
</pre>
</details>

<details>
<summary>banner</summary>
Use to display the text give in screen
<pre>
eg: banner this is cool
</pre>
</details>

<details>
<summary>toilet</summary>
Use to display the text give in screen
<pre>
eg: toilet this is cool
    toilet -f mono12
    toilet -F metal
    toilet -f mono12
    A
        ▄▄
       ████
       ████
      ██  ██
      ██████
     ▄██  ██▄
     ▀▀    ▀▀

    etc...
</pre>
</details>

<details>
<summary>Terminal train</summary>
Use to display a moving train
<pre>
eg: sl
    sl -a
    sl -s
    etc...
</pre>
</details>

<details>
<summary>xeys</summary>
Use to display two eyes on the monitor
<pre>
eg: xeyes
</pre>
</details>

<details>
<summary>oneko the cat</summary>
Use to display a cat chasing the cursor.
<pre>
eg: oneko
</pre>
</details>

<details>
<summary>espeak</summary>
Use to speak the following text
<pre>
eg: espeak hello
</pre>
</details>

<details>
<summary>have you mooed today?</summary>
Use to display a cow
<pre>
eg: apt-get moo
                 (__)
                 (oo)
           /------\/
          / |    ||
         *  /\---/\
            ~~   ~~
            
..."Have you mooed today?"...
</pre>
</details>

<details>
<summary>Terminal fire</summary>
Use to display a fire
<pre>
eg: aafire
</pre>
</details>

<details>
<summary>BB the movie</summary>
Use to display the text give in screen
<pre>
eg: bb
</pre>
</details>
<details>
<summary>chmod</summary>
Use to change the permissions to file
chmod [-R][who][+,-,=][permission]filename
<pre>
-R: recursive, allow to effect everything under that folder
who: u -> user, g ->group, o ->others a ->all
+ -> add permission
- -> remove permission
== -> assign permission
permission : w -> write, r -> read, x -> execute
eg: chmod a+w file.txt (all users can write to the file.txt)
    chmod -R g+x folder (all groups can execute all the files in the folder)
    chmod g+w, o-rw, a+x file.txt (dealing with multiple permissions)
</pre>
</details>
