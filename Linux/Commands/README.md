### Navigation Commands

<details>
<summary>ls(list)</summary>
Use to list out the directory.
<pre>
eg: ls 
    ls -l (long)
    ls -a (all file)
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
<summary>whoami</summary>
Use to display the current user
<pre>
eg: whoami
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
<summary>find file</summary>
To print out the extension of the file.
<pre>
eg: file filename
</pre>
</details>

<details>
<summary>PushD</summary>
Used to push a new layer of directory over the current directory.
Useful with the popd command.
<pre>
eg: pushd /folder1/folder2/folder3
    popd 
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
<summary>IP address</summary>
Use to check the ip, including address.
<pre>
eg: ip a
</pre>
</details>

<details>
<summary>Wget</summary>
Use to download web content,
eg: images and files.
<pre>
eg: wget url
    cat RepoList | while read $url; do wget "$url"; done
    -> download everything from RepoList
    wget url1 & wget url2
    -> download url1 and url2 parallelly.
</pre>
</details>

<br/><br/>

### Help Commands

<details>
<summary>whatis</summary>
used to print a small description about the command.
<pre>
eg: whatis ls
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
<summary>sudo updatedb</summary>
used to update the data-base of locate command.
<pre>
eg: sudo updatedb
</pre>
</details>

<details>
<summary>History</summary>
Use to display the command history
<pre>
eg: history
</pre>
</details>

<details>
<summary>grep filter</summary>
Use to filter-out, and search the command result.
Useful with piping
<pre>
eg: history | grep cd
    grep "string"
    grep -v -e"a" -e"b" -e"c"
    -v -> Invert selection
    -i -> Ignore case
    -e -> Multiple string/chars
    -c -> Matching count
    
</pre>
</details>

<details>
<summary>apropos</summary>
used to list and display all the commands related to the given tag.
<pre>
eg: apropos date
    apropos file
</pre>
</details>

<details>
<summary>aainfo</summary>
used to list the basic details about the screen and etc..
<pre>
eg: aainfo
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
<summary>Find files/folders</summary>
Use to find and display the file or folder.
<pre>
eg: find filename
    find . -iname A.txt
</pre>
</details>

<details>
<summary>locate</summary>
Used to locate the exe file of the given command/file/program etc...
<pre>
eg: locate fileName
</pre>
</details>
<details>
<summary>IP address</summary>
Used to display network address.
<pre>
eg: ip addr
</pre>
</details>
<br/>

### File System Commands

<details>   
<summary>cut</summary>
Use to cut strings.
<pre>
eg: echo "hello" | cut -c1
    h
    echo "hello" | cut -c1,5
    ho
    echo "hello" | cut -c2-
    ello
    echo "hello" | cut -c2-4
    ell
    echo "$line" | cut -f1-4
        A field is a string started from the begining 
        or a white-space to the next white-space or end
    -d
        A delimiter is a way of marking the string
        -d"*" in the "*" has been marked
        cut -d"*" -f2 -> cut after *
        cut -d"*" -f1 -> cut before *
        echo "$line" | cut -d"*" -f1,2,3 cut 3 strings
        sperated by *
</pre>
</details>

<details>   
<summary>head/tail</summary>
head display the lines from the head
tail display the lines from the tail
<pre>
eg: head hisFile newFile
    display 10 hisFile and newFile lines
    head hisFile
    display first 10 hisFile lines
    tail history 
    display last 10 hisFile lines
    -n -> number of lines
    -c -> number of chars
    -f -> live update
    tail -f dmesg
    head -n22 | tail -n +12 fileName
    12 to 22 lines
    
</pre>
</details>

<details>   
<summary>Translate</summary>
Trim the text or translate a char sequence 
<pre>
eg: 
    echo "hello world" | tr -d "l"
    heo word
    echo "hello world" | tr -s "l" "x"
    hexxo worxd
    echo "hello world" | tr -s "le" "el"
    hleo wored
    echo "Hello world" | tr -d [:lower:]
    H
</pre>
</details>

<details>   
<summary>Sed</summary>
quick parsing and transformation of text. 
<pre>
eg: 
    echo "I like brains, I like apples" | sed -e s/like/love/
    I love brains, I like apples
    echo "I like brains, I like apples" | sed -e s/like/love/g
    I love brains, I love apples
    echo "I like brains, I like apples" | sed -e s/like/love/2
    I like brains, I love apples
    echo "I like brains, I like apples" | sed -e s/^././
    . like brains, I llike apples
    -e -> add the script to the commands to be executed
    -s -> consider files as separate rather than as a single, continuous long stream.
    /s -> Match pattern
</pre>
</details>

<details>   
<summary>Sort</summary>
Sort the char sequence 
<pre>
eg: 
    sort fileName
    sort fileName -r 
    -r -> reverse the result
    -g -> general numeric-sort
    -b -> ignore leading white-space
    -f -> ignore lower-upper case
    -t -> field separator `sort -t$'\t' -k3`
    -k -> compare the following column or field `-k3 3rd field`
    -n -> compare according to string numerical value
</pre>
</details>

<details>   
<summary>Uniq</summary>
Omit the char sequence 
<pre>
eg: 
    uniq fileName
    uniq fileName -d
    -d -> only print duplicate lines, one for each group
    -D -> print all duplicate lines
    -i -> ignore differences in case when comparing
    -u -> only print unique lines
    
</pre>
</details>

<details>   
<summary>Paste</summary>
quick manipulation with files.
<pre>
eg: 
    paste file1 file2 
    
    -> Align the content on the file in a horizontal manner,
       Separated by tab space.
       
    paste -d: file1 file2   
       Separated by colon.
       
    < fileName paste - - -
    -> Align the text file fileName in 3 columns,
       " - " is represent a column.
       
    paste -d';' - - -
    -> Three line separated by ;
    
    -d -> reuse characters from LIST instead of TABs.
    -s -> serial,  paste one file at a time instead of in parallel.
    -z -> line delimiter is NUL, not newline.
    
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

<details>   
<summary>touch file_name</summary>
Use to create file.
<pre>
eg: touch file.txt
    touch file1 file2 fileN
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
<summary>Delete files</summary>
Use to delete files.
<pre>
eg: rm filename
    rm * (remove all files)
    rm *.png (remove all png files)
    rm firstName* (remove all files starts with the firstName)
    rm -r folder (remove folder)
</pre>
</details>

<details>
<summary>Delete empty folders</summary>
used to delete folders which don't have  any content in it.
<pre>
eg: rmdir folderName
</pre>
</details>

<details>
<summary>copy</summary>
used to copy a file.
<pre>
eg: cp file1Path file2Path
    cp fileName  newFileName
</pre>
</details>

<details>
<summary>Rename / Move</summary>
used to rename and move file and folders.
<pre>
eg: mv oldFile newFile (the oldFile will get rewrites by the newFile)
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
    cat >> filename (append content)
    cat > filename (rewrite the file)
    type the content
    // concatenate files
    cat fileone filetwo
    cat fileone.txt >> filetwo.txt (append content)
    cat fileone.txt > filetwo.txt (rewrite the file)
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
    nano fileName
</pre>
</details>

<details>
<summary>more</summary>
more is an predecessor of less.
<pre>
eg: more fileName
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
<summary>PDF to text</summary>
Use to convert pdf file to text file.
<pre>
eg: pdftotext fileName
</pre>
</details>

<details>
<summary>Word count</summary>
Return the word count with in the file given.
<pre>
eg: wc fileName
</pre>
</details>

<details>
<summary>Compare</summary>
Compare two files and return the result.
<pre>
eg: cmp file1 file2
</pre>
</details>

<details>
<summary>Split</summary>
Split is used to make a copy of the file at the instance.
<pre>
eg: split fileName
</pre>
</details>

<details>
<summary>diff</summary>
Return the differences two files.
<pre>
eg: diff file1 file2
</pre>
</details>

<br/>

### User/Group Commands

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
<br/>

### Hack Commands

<details>
<summary>Disk free(df)</summary>
Use to check the disk status,
<pre>
eg: df
    df -h
</pre>
</details>

<details>
<summary>Users</summary>
Use to display the users logged into the system.
<pre>
eg: users
</pre>
</details>

<details>
<summary>ID</summary>
Use to display the id numbers of the user.
<pre>
eg: id
    id -un
</pre>
</details>

<details>
<summary>Piping</summary>
Use one command on another command.
<pre>
eg: history | less
    ls -la /> file.txt
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
<summary>sudo blkid</summary>
Use to list all the drives on the system
with the UUID and TYPE
<pre>
eg: sudo blkid
</pre>
</details>

<details>
<summary>killall program_name</summary>
To kill the program
<pre>
eg: killall chrome
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
<summary>ping domain -c number</summary>
ping is used to check internet connection
<pre>
eg: ping www.google.com 
    ping www.google.com -c 3
</pre>
</details>

<details>
<summary>Parallel</summary>
Parallel is used to run process parallelly
eg: downloading internet content,
    video conversion, run audio and video at the same time
    etc...
<pre>
eg: cat RepoList | parallel -j 4 wget {}
    -> take the urls from RepoList and put it into {}
       four process is done parrallelly.
    -j -> number of parallel slots, -j numOfSlots
</pre>
</details>

<br/>

### Useless Commands

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
<summary>xeyes</summary>
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
<summary>Cowsay</summary>
Use to display a dialogs
<pre>
eg: cowsay happy
 _______
< happy >
 -------
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
                
   cowthink happy
    _______
   ( happy )
    -------
           o   ^__^
            o  (oo)\_______
               (__)\       )\/\
                   ||----w |
                   ||     ||
   cowsay -f ghostbusters who you gonna call
   cowsay -f dragon-and-cow "message"
  
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

<br/>

### Other Commands

<details>
<summary>Calendar </summary>
Used to display a simple calendar.
<pre>
eg: cal
</pre>
</details>

<details>
<summary>Sh</summary>
Used to open a temporary sh file
<pre>
eg: sh
</pre>
</details>

<details>
<summary>Curl</summary>
Used to display html of the given url.
C-url
<pre>
eg: curl https://google.com
    curl https://github.com/AbhilashTUofficial
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
<summary>echo</summary>
Use to display the text give in screen
<pre>
eg: echo hello world!!!
</pre>
</details>

<br/>
