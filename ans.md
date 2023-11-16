# p1

我懶
***

# p2

ans可以改sum
一堆ans 
會被懷疑
```py
a=int(input())
b=int(input())
c=int(input())
ans=0
while a>=b:
    print("please input a and b again!")
    a=int(input())
    b=int(input())
while c<=0:
    print("please input c again!")
    c=int(input())
for i in range(a+1,b):
    if i%c==0:
        ans+=i
print(ans)
```


```py
a=int(input())
b=int(input())
c=int(input())
ans=0
while a>=b:
    a=int(input())
    b=int(input())
    print("please input a and b again!")
while c<=0:
    c=int(input())
    print("please input c again!")
for i in range(a+1,b):
    if i%c==0:
        ans+=i
print(ans)
```

```py
a=int(input())
b=int(input())
c=int(input())
while a>=b:
    a=int(input())
    b=int(input())
    print("please input a and b again!")
while c<=0:
    c=int(input())
    print("please input c again!")
ans=0
for i in range(a+1,b,1):
    if i%c==0:
        ans=ans+i
print(ans)
```

***

# p3
我寫好了，測資有錯，等他改好==


有其他方法，等我


記得改變數名字，不然一堆lis


建議改data array ...
```py
lis=input().split(",")
step=int(input())
for i in range(len(lis)):
    lis[i]=int(lis[i])
for i in range(len(lis)-1):
    for j in range(len(lis)-i-1):
        if lis[j]<lis[j+1]:
            lis[j],lis[j+1]=lis[j+1],lis[j]
    if ((i+1)==step):
        print(f"step{step}:{lis}")

```
```py
lis=input().split(",")
step=int(input())
for i in range(len(lis)):
    lis[i]=int(lis[i])
for i in range(1,len(lis)):
    for j in range(len(lis)-i-1):
        if lis[j]<lis[j+1]:
            temp=lis[j+1]
            lis[j+1]=lis[j]
            lis[j]=temp
    if (i==step):
        print(f"step{i}:{lis}")
```

***

# p4

小複雜，等我寫比較簡單的，想走的可以先用沒關西
```py
data=input().split(",")
al=[]
di=[]
ot=[]

for i in data:
    if (i.startswith('-') and i[1:] or i).isdigit():
        di.append(i)
    elif i.isalpha():
        al.append(i)
    else:
        ot.append(i)
print(di)
print(al)
print(ot)
```

```py
s=input().split(',')
number=[]
alphabet=[]
other=[]
def isnumber(a):
    if a.isdigit():
        return True
    else:
        if a[0]=='-' and a[1:].isdigit():
            return True
    return False
for i in range(len(s)):
    if isnumber(s[i]):
        number.append(s[i])
    elif s[i].isalpha():
        alphabet.append(s[i])
    else:
        other.append(s[i])
print(number)
print(alphabet)
print(other)
```

```py
number=[]
alphabet=[]
other=[]
s=input().split(',')
def isnumber(a):
    if a.isdigit():
        return True
    else:
        if a[0]=='-' and a[1:].isdigit():
            return True
    return False

for i in range(len(s)):
    if isnumber(s[i]):
        number.append(s[i])
    elif s[i].isalpha():
        alphabet.append(s[i])
    else:
        other.append(s[i])
print(number)
print(alphabet)
print(other)
```

```py
number=[]
alphabet=[]
other=[]
s=input().split(',')
def isnumber(a):
    if a.isdigit():
        return True
    else:
        if a[0]=='-' and a[1:].isdigit():
            return True
    return False

for i in s:
    if isnumber(i):
        number.append(i)
    elif i.isalpha():
        alphabet.append(i)
    else:
        other.append(i)
print(number)
print(alphabet)
print(other)
```

***

# p5
等我==

```py
pw=input()
upp=False
low=False
di=False
other=False
leng=False
title=True
def isodd(a):
    s="~!@#$%^&*()_+-*/<>,.[]\/\'\"=><˙{ }"
    for i in s:
        if a==i:
            return True
    return False
for i in pw:
    if i.isupper():
        upp=True
    if i.islower():
        low=True
    if i.isdigit():
        di=True
    if isodd(i):
        other=True
if len(pw)>=6 and len(pw)<=12:
    leng=True
if pw[0].isdigit():
    title=False
if (upp and low and di and other and leng and title):
    print("Success")
else:
    print("Fail")
```
可讀性應該不錯，加油
這我沒丟到oj上
應該能過
```py
pw=input()
check_len=True
check_title=True
check_digit=False
check_upper=False
check_lower=False
check_odd=False
for i in range(len(pw)):
    if pw[i].isupper():
        check_upper=True
    if pw[i].islower():
        check_lower=True
    if pw[i].isdigit():
        check_digit=True
    if (pw[i].isdigit() and pw[i].isalpha)==False:
        check_odd=True
if pw[0].isdigit():
    check_title=False
if len(pw)>12 or len(pw)<6:
    check_len=False
if (check_len and check_digit and check_lower and check_upper and check_title and check_odd):
    print("Success")
else:
    print("Fail")
```

***

