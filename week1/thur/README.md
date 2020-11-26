touch {foo,bar}/{a..j} <br/>

**exercise**
1. 
Read man ls and write an ls command that lists files in the following manner:<br/>
Includes all files, including hidden files<br/>
Sizes are listed in human readable format (e.g. 454M instead of 454279954)<br/>
Files are ordered by recency<br/>
Output is colorized<br/>

**answer:** 
ls -l -h -t -r<br/>
(-l: show details of each document in the list;<br/>
-h: display the size of document in the formel of B, M, G;<br/>
-t: rearrange order in time;<br/>
-r: reverse order)<br/>

![image](https://github.com/Penny-Zhang/images/blob/main/截屏2020-11-26%20下午3.22.54.png)<br/>

2.
Write bash functions marco and polo that do the following. Whenever you execute marco the current working directory should be saved in some manner, then when you execute polo, no matter what directory you are in, polo should cd you back to the directory where you executed marco. For ease of debugging you can write the code in a file marco.sh and (re)load the definitions to your shell by executing source marco.sh.<br/>

**answer:**





