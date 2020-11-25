##bash shell<br/>
**output**
$(CMD) (e.g. for file in $(ls), first call "ls") <br/>
<(CMD) (e.g diff <(ls foo) <(ls bar : show differences between files in dirs foo and bar)<br/>
 
**commond**
$0 - Name of the script<br/>
$1 to $9 - Arguments to the script. $1 is the first argument and so on.<br/>
$@ - All the arguments<br/>
$# - Number of arguments<br/>
$? - Return code of the previous command<br/>
$$ - Process identification number (PID) for the current script<br/>
!! - Entire last command, including arguments. A common pattern is to execute a command only for it to fail due to missing permissions; you can quickly re-execute the command with sudo by doing sudo !!<br/>
$_ - Last argument from the last command. If you are in an interactive shell, you can also quickly get this value by typing Esc followed by .<br/>
![image](https://github.com/Penny-Zhang/images/commit/eba1a34546ba8c01a9b1646f3c63f0b3efe279a0?short_path=405fd89)<br/>

**conditionally execute**<br/>
&& ; ||<br/>

**wildcards**<br/>
for files: foo, foo1, foo2, foo10 and bar<br/>
enter: "rm foo? " foo1 and foo2 will be deleted<br/>
enter: "rm foo*" all foo will be deleted except for bar<br/>






