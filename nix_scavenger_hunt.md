# *nix Scavenger Hunt

Complete the following challenges using the command-line interface on your favorite
Unix or Linux operating system. You are welcome and encouraged to consult any
additional documentation online or in books.

Please add your answers/responses/text pastes to the document after each prompt.

Note: For some of the challenges you will need to reference files included with
this repository, so you will need to fork the repo into your own Github account
and then clone it to your development environment.

## The Challenges

### Navigating the Filesystem

* Get an idea of where you are in the operating system. Use the `pwd` command to find your "path to working directory"--your current location in the filesystem of your devbox. *Paste the output of the `pwd` command here: /home/cabox/workspace   

* Discover more about this filesystem. Use `ls` (the "list" command)to see what is in this directory. *What directories and files do you see when you run `ls`? LICENSE  README.md  challenge_files  nix_scavenger_hunt.md  nix_scavenger_hunt_stretch.md   

* You can use *options* to modify how a command runs. Try using `ls -alh` to see the contents of your current directory. *How are the results different when you use the `-alh` options?

The is extra information. Along with the list of file names you also have the size of each file and the date it was created in the repository.
total 36K                                                                                                                                                                                               
drwxrwxr-x 4 cabox cabox 4.0K Jan 11 23:51 .                                                                                                                                                            
drwxr-xr-x 7 cabox cabox 4.0K Jan 11 23:51 ..                                                                                                                                                           
drwxrwxr-x 8 cabox cabox 4.0K Jan 11 23:51 .git                                                                                                                                                         
-rw-rw-r-- 1 cabox cabox 1.1K Jan 11 23:51 LICENSE                                                                                                                                                      
-rw-rw-r-- 1 cabox cabox 2.7K Jan 11 23:51 README.md                                                                                                                                                    
drwxrwxr-x 7 cabox cabox 4.0K Jan 11 23:51 challenge_files                                                                                                                                              
-rw-rw-r-- 1 cabox cabox 5.5K Jan 11 23:51 nix_scavenger_hunt.md                                                                                                                                        
-rw-rw-r-- 1 cabox cabox  317 Jan 11 23:51 nix_scavenger_hunt_stretch.md  
 
* The `man` ("manual") command tells you more about how any given command works. (*WARNING:* CodeAnywhere does not support the man command. You can click the following link to complete this task: http://linux.die.net/man/). Run `man` to see instructions about how to use `man`. Then use `man` to learn what the `a`, `l`, and `h` options mean when used with the `ls` command.  
-a - find all matching entries
-l - list contents of directory
-h - print this help message
-
* Commands can also take *arguments*, which are usually the names of files or locations that you want the command to work with. Try running `ls /` to see what files are in the *root* directory of the filesystem. 
LICENSE  README.md  challenge_files  nix_scavenger_hunt.md  nix_scavenger_hunt_stretch.md 

* A Unix filesystem has a few special shortcuts to refer to specific locations. `/` indicates the *root* of the filesystem, meaning the top-most directory in the filesystem hierarchy. Use the `cd` ("change directory") command to move to the root directory. (Hint: Use `man` to look up the `cd` command if you have any issues) *Then run `pwd` and paste the output here:*
* Another special shortcut in Unix is the `~` location. This indicates the *user root* directory, meaning the top-most directory in the hierarchy that comes below your user account. Use `cd` to move to `~`. *Run `pwd` and paste the response here:*cabox@box-codeanywhere:~$ pwd                                                                                                                                                                          
/home/cabox  

* Change directory into the `challenge_files` directory. Use `ls` to find only the files with a `.demo` pattern. *How many files do you find?* - 3
* Use the `cd` command to move "up" one directory. /home/cabox/workspace  
* Press the up arrow on your keyboard. cd
* Press the up arrow a few more times. Each command I enter in the command line one at a time
* Run the `history` command. *What do you see?* The last 55 commands I entered
    1  ls                                                                                                                                                                                              
    2  ls                                                                                                                                                                                              
    3  /                                                                                                                                                                                               
    4  cd                                                                                                                                                                                              
    5  pwd                                                                                                                                                                                             
    6  cd challenge_files                                                                                                                                                                              
    7  ls                                                                                                                                                                                              
    8  pwd                                                                                                                                                                                             
    9  cs                                                                                                                                                                                              
   10  cd                                                                                                                                                                                              
   11  cd -ls                                                                                                                                                                                          
   12  cd challenge_files                                                                                                                                                                              
   13  cd \challenge_files                                                                                                                                                                             
   14  pwd                                                                                                                                                                                             
   15  cd /challenge_files                                                                                                                                                                             
   16  pwd                                                                                                                                                                                             
   17  cd wow                                                                                                                                                                                          
   18  ls                                                                                                                                                                                              
   19  cd workspace                                                                                                                                                                                    
   20  cd challenge_files                                                                                                                                                                              
   21  ls                                                                                                                                                                                              
   22  ls '.demo'                                                                                                                                                                                      
   23  cd                                                                                                                                                                                              
   24  cd workspace                                                                                                                                                                                    
   25  cd challenge_files                                                                                                                                                                              
   26  cd up                                                                                                                                                                                           
   27  cd                                                                                                                                                                                              
   28  pwd                                                                                                                                                                                             
   29  cd workspace/challenge_files                                                                                                                                                                    
   30  cd /                                                                                                                                                                                            
   31  pwd                                                                                                                                                                                             
   32  ls                                                                                                                                                                                              
   33  cd workspace                                                                                                                                                                                    
   34  pwd                                                                                                                                                                                             
   35  cd challeng_files                                                                                                                                                                               
   36  cd challenge_files                                                                                                                                                                              
   37  pwd                                                                                                                                                                                             
   38  cd -/                                                                                                                                                                                           
   39  cd -dir                                                                                                                                                                                         
   40  cd -ls workspace                                                                                                                                                                                
   41  cd /workspace                                                                                                                                                                                   
   42  cd                                                                                                                                                                                              
   43  pwd                                                                                                                                                                                             
   44  cd workspace/challange_files                                                                                                                                                                    
   45  cd workspace                                                                                                                                                                                    
   46  cd challenge_files          
   47  cd                                                                                                                                                                                              
   48  mv workspace/challange_files                                                                                                                                                                    
   49  cd wordspace                                                                                                                                                                                    
   50  cd workspace                                                                                                                                                                                    
   51  cd challenge_files                                                                                                                                                                              
   52  pwd                                                                                                                                                                                             
   53  cd ..                                                                                                                                                                                             
   54  pwd                                                                                                                                                                                             
   55  history   

### Observing the System

* Discover what account you are logged into using the `whoami` command. *What username are you currently using?* - cabox   - No
If so, list them here:* - N/A
* How long has your system been running? Use `uptime` to see, and *paste the result here:* - 12:12:18 up  1:03,  1 user,  load average: 0.00, 0.00, 0.00

* Run `ps aux` and review the results. (Hint: Use `man` to learn more about the `ps` command and options.) *How do you interpret what you see here?*
* Run `top` and review the results. (Hint: You may need to use `ctrl-c` to get out of this app.) *How do you interpret what you see here?*
USER       PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND                                                                                                                               
root         1  0.0  0.5  33328  2708 ?        Ss   11:09   0:00 init                                                                                                                                  
root         2  0.0  0.0      0     0 ?        S    11:09   0:00 [kthreadd/911073]                                                                                                                     
root         3  0.0  0.0      0     0 ?        S    11:09   0:00 [khelper/911073]                                                                                                                      
root       144  0.0  0.1  19428   832 ?        S    11:09   0:00 upstart-udev-bridge --daemon                                                                                                          
root       178  0.0  0.2  49216  1416 ?        Ss   11:09   0:00 /lib/systemd/systemd-udevd --daemon                                                                                                   
root       303  0.0  0.1  15496   964 ?        S    11:09   0:00 upstart-socket-bridge --daemon                                                                                                        
root       304  0.0  0.1  15356   760 ?        S    11:09   0:00 upstart-file-bridge --daemon                                                                                                          
syslog     310  0.0  0.2 184188  1436 ?        Ssl  11:09   0:00 rsyslogd                                                                                                                              
root       384  0.0  0.5  61316  3052 ?        Ss   11:09   0:00 /usr/sbin/sshd -D                                                                                                                     
root       419  0.0  0.1  12740   848 tty1     Ss+  11:09   0:00 /sbin/getty 38400 console                                                                                                             
root       424  0.0  0.1  12740   844 tty2     Ss+  11:09   0:00 /sbin/getty 38400 tty2                                                                                                                
root       434  0.0  0.6  63876  3304 ?        Ss   11:09   0:00 sshd: cabox [priv]                                                                                                                    
cabox      436  0.0  0.2  64168  1556 ?        S    11:09   0:00 sshd: cabox@notty                                                                                                                     
cabox      437  0.0  0.1  12896  1032 ?        Ss   11:09   0:00 /usr/lib/openssh/sftp-server                                                                                                          
root       461  0.0  0.6  63876  3456 ?        Ss   11:55   0:00 sshd: cabox [priv]                                                                                                                    
cabox      463  0.0  0.2  63876  1468 ?        R    11:55   0:00 sshd: cabox@pts/0                                                                                                                     
cabox      464  0.0  0.3  18132  2032 pts/0    Ss   11:55   0:00 -bash                                                                                                                                 
cabox      480  0.0  0.2  15520  1144 pts/0    R+   12:12   0:00 ps aux 

### Finding and Viewing Files

* Make sure you are in the `challenge_files` directory. Use the `*` wildcard to find all the files that have the word "credit" in the filename. *How many files did you find?* 2

* Use the `more` command to view one of the `credit_cards` files you just discovered. (Hint: Type `q` to quit viewing the file. Press the `spacebar` to page down. Use your keyboard arrows to move up/down.) *What is the date in the file you have viewed?*  01-15-2015  
* Use the `find` command to search for files more effectively. Search the sub-directories under `challenge_files` to find the location of the file named `modi_laboriosam.txt`. *Where is that file located?*  /home/cabox/workspace/challenge_files/tmp 
* Use the `grep` command to search for text within a file. Use `grep` on all the `.user` files in `challenge_files` to find which files contain "WA" (the abbreviation for Washington state). *How many files did you find?* 2
* Use the `-r` option of `grep` to *recursively* find the text "Waldo" hidden in a file somewhere under the `challenge_files` directory. *Paste the result showing the file and line where the word "Waldo" shows up.*
serial-numbers/eaque_molestiae.txt:4:Ut est maiores quia autem. Nisi modi Waldo sed corporis sit explicabo ut est. Et est placeat ea sunt sunt consectetur sunt incidunt. Explicabo vel esse blanditiis
 dolorem culpa non quia.  

### Pipes and Connecting Commands

* Sometimes it's useful to output the results of a command to a text file for further analysis, reference, or processing. Try running `ls > files.txt`. Notice that the file `files.txt` was created. View that file using `more`. *What do you see in the `files.txt` file?* A listing of all of the files in the /challenge_files/ folder.  It ran the ls command and wrote the results to files.txt.
* Notice that if you run `ls -alh` in the `challenge_files` directory, the files scroll by very quickly. Sometimes it would be better to get the results in a paginated format. Try running `ls -alh | more`. *Describe what you see when you run `ls -alh | more`.* Running ls -alh in paginated format splits the output.  It only displays part of full result so you can review it. You can hit the spacebar to complete the command or the enter key to load one additional line.
* Earlier, when you viewed the list of active processes on your devbox using `ps aux`, the list was probably really long. You can make this list more manageable by using the pipe (`|`) to filter the results of `ps` using `grep`. Run `ps aux | grep <your_username>` to see what processes are running for your specific user. *Paste the list of processes that reference your username here:*
cabox      766  0.0  0.1   8816   752 pts/3    S+   14:58   0:00 grep --color=auto victa727      
