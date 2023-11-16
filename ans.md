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

***

# p4

***

# p5

***

# p6

***
