**python Recursive algorithm** <br/>
Hanoi：<br/>
A(64 big-small), B，C<br/>
A-C-B(63)<br/>
A-B-C(1)<br/>
B(63 big-small), A, C(1)<br/>
...<br/>

'''def printMove (x, y):<br/>
    print('move from ' + str(x) +  ' to '  + str(y))<br/>

def Towers(n, one, two, three):<br/>
    if n==1:<br/>
        printMove(one, three)<br/>
    else:<br/>
       Towers(n-1, one, three, two)<br/>
       printMove(one, three)<br/>
       Towers(n-1, two, one, three)<br/>

print(Towers(3, 'A', 'B', 'C'))<br/>
'''

**Write a function to find roots**<br/>
'
def findRoot(x, power, epsilon):<br/>
    '''x and epsilon int or float, power an int<br/>
    epsilon >0 & power>=1<br/>
    return a float y s.t. y**power is within epsilon of x.<br/>
    if such a float does not exist, it returns None'''<br/>
    if x < 0 and power%2 == 0:<br/>
        return None<br/>
    low = min(-1.0, x)<br/>
    high = max(1.0, x)<br/>
    ans = (high+low)/2.0<br/>
    while abs(ans**power -x) > epsilon:<br/>
       if ans**power < x:<br/>
           low = ans<br/>
       else:<br/>
           high = ans<br/>
       ans = (high+low)/2.0<br/>
    return(ans)<br/>
'
**Use of keywords**<br/>
‘
def shop(where='store',what='pasta', howmuch='10 pounds'):<br/>
    print('I want you to go to the', where)<br/>
    print('and buy', howmuch,'of',what+'.')<br/>

shop()<br/>
shop(what='towels')<br/>
’

**Lambda**<br/>
Lambda function is used to create an anonymous function, the function name is not bound to the identifier.<br/>
Use lambda functions to return some simple calculation results<br/>
‘
def func():<br/>
    x=1<br/>
    y=2<br/>
    m=3<br/>
    n=4<br/>
    sum = lambda x,y:x+y #将lambda和变量sum绑定，sum就是函数名<br/>
    print(sum)  #输出的是lambda函数的地址<br/>
    sub = lambda m,n:m-n<br/>
    print(sub)<br/>
    return sum(x,y)+sub(m,n)<br/>

print(func())<br/>
’
tip：<br/>
Use lambda to find absolute value<br/>
‘
print((lambda x:-x)(-2))
'

