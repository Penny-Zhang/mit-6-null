touch {foo,bar}/{a..j} <br/>
chmod (u/g/o/a) (+/-/=) (r/w/x）<br/>
chmod u=rw, og=rx<br/>
mkdir: build a new directory<br/>
touch file.format: build a new document with a specific format<br/>
mvdir: move directory (e.g. mvdir dir_name)<br/>
file: show the format of the document(file file_name)<br/>
find: find document with specific format(find*.file_format)<br/>
cat:(cat file)<be/>
head: (head -xx file_name)<br/>
tail: (tail -xx file_name)<br/>
paste: horizontal stitching file (paste file1 file2)<br/>
diff: shwo differences between file1 and file2 (diff file1 file2)<br/>
wc: count words/rows(wc_file_name)<br/>
uniq: delete duplicate rows<br/>
grep<br/>

**exercise**<br/>
**1.** 
Read man ls and write an ls command that lists files in the following manner:<br/>
Includes all files, including hidden files<br/>
Sizes are listed in human readable format (e.g. 454M instead of 454279954)<br/>
Files are ordered by recency<br/>
Output is colorized<br/>

**answer:** 
ls -l -h -t -r -a; ls -lhtra<br/>
(-l: show details of each document in the list;<br/>
-h: display the size of document in the formel of B, M, G;<br/>
-t: rearrange order in time;<br/>
-r: reverse order)<br/>
-a：show the documents, which were hidden behind up<br/>

![image](https://github.com/Penny-Zhang/images/blob/main/截屏2020-11-26%20下午3.22.54.png)<br/>
-: normal file; d: directory<br/>
rw-r--r--: access permission(user; group; other user)<br/>
x: the number of documents<br/>
xx: user's name<br/>
xxx: group's name<br/>
xxxx: the size of the document<br/>
xxxxx: the motifiled date<br/>
xxxxxx: document's name <br/>

**2.**
Write bash functions marco and polo that do the following. Whenever you execute marco the current working directory should be saved in some manner, then when you execute polo, no matter what directory you are in, polo should cd you back to the directory where you executed marco. For ease of debugging you can write the code in a file marco.sh and (re)load the definitions to your shell by executing source marco.sh.<br/>

**answer:**





