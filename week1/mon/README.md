# 1、shell. 
(since i use mac OS system, so i only mark things that is useful for mac OS).   
## mac OS - bash. 
open terminal - a single line on the top (shell prompt). 

![Image of terminal page](https://github.com/Penny-Zhang/images/blob/main/terminal.png). 

**basic and convenient use:**
1) it can show date and specific time when you enter "date" on it<br/>
2) when write "echo + anything you want it to show you", it will just show the things you write after "echo"<br/>
    ( e.g. type "echo 'Hello, world'" ; "echo Hello\ World")<br/>
3) environment variable:<br/>
    a) echo $PATH: show the path of command on my comnputer <br/>
          *absolute path: path that fully determine the locatiuon of a file* <br/> 
          *relative path: path that is relative to the place where you are* <br/>
    b) pwd: show currently location <br/> 
    c) cd + ...: change the currently working directory (shell prompt will show that) <br/>
          (cd -: go back to last directory） <br/>
    d) ls (+ ...): show the files'list of current directory <br/>
          (ls -l: show more details of files'list)<br/>
    e) mv: rename a file or replace it in another directory<br/> 
         (mv XX.XX YY.XX : rename file XX.XX to file YY.XX or move XX.XX into another directory<br/>
    f) cp: copy<br/>
    g) rm: remove<br/>
4) man: manual pages. 
      (man LS = upgrade LS --help). 
5) Q: quit. 
6) ctrl + L: clearl terminal.   

**different input & output forms by terminal** <br/>
1) echo hello: it will show "hello" on the terminal<br/>
   echo hello > hello.txt: there will be nothing happenning on the terminal, since  "hello" was written in a txt <br/>
2) cat: print the context of the file on the terminal<br/>
   (e.g. cat < hello.txt: it will show "hello" on the terminal)<br/>
   (e.g. cat < hello.txt > hello2.txt: write the consequence of command "cat < hello.txt" into hello2.txt)<br/> 
   (e.g. cat < hello.txt >> hello2.txt: it will show "hello" twice on the terminal)<br/>
      *content-length: show the length*<br/>
3) "|": chain programs- the former output is the input of the next file<br/>
   (e.g. curl --head --silent google.com | grep --ignore-case content-length | cut --delimiter=' ' -f2)<br/>

**rooter user**
1) sudo. 

## exercise
1.pass<br/> 
2.<br/>
`cd coding`<br/> 
`mkdir missing`<br/> 
3.  
`man touch`<br/>
4.<br/>
`cd missing`<br/> 
`touch semester.txt`<br/> 
5.<br/>
`open semester.txt`<br/> 
(then copy:  <br/>
#!/bin/sh<br/>
curl --head --silent https://missing.csail.mit.edu)<br/> 
6.<br/>
`./semester.txt. -- permission denied`<br/> 
7.<br/>
`sh semester.txt -- show up`<br/> 
(serached online: “sh” takes the following file as a parameter, and “./” takes the following file as an executable program)<br/>
8. <br/>
`···man chmod`<br/> 
9.<br/>
`chmod +x semester.txt` <br/> 
`./semester.txt`<br/>
(my shell knows that the file is supposed to be interpreted using sh, because the file begins with "#!/bin/sh")<br/>
10. <br/>
`touch last-modified.txt`<br/>
`ls -l | grep semester > last-modified.txt`<br/>







   
       
    
    
