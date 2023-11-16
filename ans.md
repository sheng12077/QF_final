# p1

畫圖
等等，但建議自己畫
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

***

# p5

***

# p6

***
