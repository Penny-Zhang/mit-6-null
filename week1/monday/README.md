# 1、shell. 
(since i use mac OS system, so i only mark things that is useful for mac OS).   
## mac OS - bash. 
open terminal - a single line on the top (shell prompt). 

![Image of terminal page](https://github.com/Penny-Zhang/images/blob/main/terminal.png). 

**basic and convenient use:**
1) it can show date and specific time when you enter "date" on it. 
2) when write "echo + anything you want it to show you", it will just show the things you write after "echo".  
   ( e.g. type "echo 'Hello, world'" ; "echo Hello\ World"). 
3) environment variable:  
    a) echo $PATH: show the path of command on my comnputer. 
       *absolute path: path that fully determine the locatiuon of a file*. 
       *relative path: path that is relative to the place where you are*.
    b) pwd: show currently location. 
    c) cd + ...: change the currently working directory (shell prompt will show that). 
       (cd -: go back to last directory）. 
    d) ls (+ ...): show the files'list of current directory. 
       (ls -l: show more details of files'list). 
    e) mv: rename a file or replace it in another directory.     
       (mv XX.XX YY.XX : rename file XX.XX to file YY.XX or move XX.XX into another directory）.
    f) cp: copy.    
    g) rm: remove.     
4) man: manual pages. 
   (man LS = upgrade LS --help). 
5) Q: quit. 
6) ctrl + L: clearl terminal.   

**different input & output forms by terminal**. 
1) echo hello: it will show "hello" on the terminal. 
   echo hello > hello.txt: there will be nothing happenning on the terminal, since  "hello" was written in a txt.  
2) cat: print the context of the file on the terminal. 
   (e.g. cat < hello.txt: it will show "hello" on the terminal). 
   (e.g. cat < hello.txt > hello2.txt: write the consequence of command "cat < hello.txt" into hello2.txt). 
   (e.g. cat < hello.txt >> hello2.txt: it will show "hello" twice on the terminal). 
*content-length: show the length*. 
3) "|": chain programs- the former output is the input of the next file. 
   (e.g. curl --head --silent google.com | grep --ignore-case content-length | cut --delimiter=' ' -f2). 

**rooter user**
1) sudo. 

## exercise
1.pass. 
2.  
`cd coding <br>`
`mkdir missing <br>`
3.
`man touch <br>`
4.  
`cd missing <br>`
`touch semester.txt <br>`
5.  
`open semester.txt <br>
(then copy: <br>
#!/bin/sh <br>
curl --head --silent https://missing.csail.mit.edu) <br>`
6.    
`./semester.txt. -- permission denied <br>`
7.  
`sh semester.txt -- show up <br>`
(serached online: “sh” takes the following file as a parameter, and “./” takes the following file as an executable program）<br>
8.  
`···man chmod <br>`
9.  
`chmod +x semester.txt <br>`
`./semester.txt <br>`
(my shell knows that the file is supposed to be interpreted using sh, because the file begins with "#!/bin/sh")
10.  
`touch last-modified.txt`
`ls -l | grep semester > last-modified.txt`







   
       
    
    
