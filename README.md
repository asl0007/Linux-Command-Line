# Linux-Command-Line

## [My own Command line practice]

### 1. ln -s fileName pointerName : create symbolic link(pointer to file).
### 2. init 0 ,poweroff : shutdown
### 3. int 6 - restart
### 4. tail fileName : print last 10 lines of file.
### 5. head fileName : print first 10 lines if file.
### 6. tail -f fileName : it show realtime changes in file.
### 7. htop : taskManager
### 8. who, w : who is logged in from when, how long and what prgrms user running.
### 9. top : processManager shows prgrms at top, which use more CPU power.
### 10 netstat -tupln:
### 11 mkdir -p lemon/child/neseted/ : creating nested folders in one line.
### 12 ctrl + D : to close terminal.

### 13. Every cmnd/prgrm has three channel
    STDIN --> 0 (file_discripter)
    STDOUT --> 1
    STDERR --> 2
    
    ex lemon 2>> err.txt //output the error to err.txt

### 14. ps aux | less : show the snapshot of running process.
### 15. cat key-value(filename) | cut -d: -f2
        ex: key-value file: 
            name : coderOO7
            sex : male
            age : 22
            
        //  Now "d" specify delimilator i.e ":" . cut cmnd seperate the o/p in two fields f1 contaning portion before ":" and f2 containg 
            portion after ":".
### 16. apt search whatever : search packages similar to keyword you enter after "search".

### 17 sudo nano /etc/login.defs : it allow to change defalult file permissions.
        ex: aim.txt (-rwxr_xr_x--->by default file permissions)
        
        step1--now enter above command .
        step2-- search for keyword UMASK
        step3-- UMASK 024 (these get substract. 0-->rwx, 2-->rx, 4-->r)
        step4-- save
        
        touch lemon.txt
        ls -l
        aim.txt rwxr_xr__(default new permission)
        
 ### 18 sudo su -i : root mode 
 
 ### 19 tail /etc/passwd: list of all system-accounts and user-account
        https://www.cyberciti.biz/faq/understanding-etcpasswd-file-format/
        
 ### 20 tail /etc/shadow: store the passwd of user-account in hash.
        https://www.digitalocean.com/community/tutorials/how-to-use-passwd-and-adduser-to-manage-passwords-on-a-linux-vps
        
 
 ### 21 which package-name: to find the location of package.
 
 ### 22 adduser username : it run pre-defined perScript which automatically create additional attributes..
        //Other command is : 
        useradd -m -d /home/coderoo7 -s /bin/bash coderoo7
        -m ---> create home directory
        -d ---> user-directory path
        -s ---> path of your shell
        coderoo7 ---> userName
        
 ### 23 userdel username : delete the user
        even after deleting the user the home directory contain the username Folder...we have to delete it manually.
 
 ### 24 usermod -L username : it lock the passwd means user can't login(create '!' symbol in passwd place).
 ### 25 usermod -U username : it enable the password login. 
 
 ### 26 echo $SHELL :  to know  the shell you are using.
 ### 27 echo $TERM : to know terminal you are using.
 
 ### 28 
