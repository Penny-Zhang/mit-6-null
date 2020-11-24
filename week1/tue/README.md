learn more and deeper in overview class<br/>

**control flow expressions**<br/> 
create command pipelines & saving results into files & reading from standard input<br/>

**use bash**<br/>
bash-zsh：chsh -s /bin/zsh; then restart terminal<br/>
zsh-bash：chsh -s /bin/bash; then restart terminal<br/>

assign variables: foo=XX (e.g. foo=bar)<br/>
access varibales: echo $foo or echo "$foo" (echo '$foo': $foo)<br/>
create a directory and cd to it: <br/> 
`mcd ()` {<br/>
    `mkdir -p "$1"`<br/>
    `cd "$1"`<br/>
}<br/>
mcd test: set up a file named "test" and cd to it <br/>
($1 to $9 are arguments to the script; $1 is the first argument)<br/>
($_ - Last argument from the last command)<br/>
($? - Return code of the previous command)<br/>

6:25/48:55


                                         

