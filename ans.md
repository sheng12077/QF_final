P1
```py
n=int(input())
ans=0
for i in range(1,n+1):
    if i%3==0:
        ans+=i

print(ans)
```

P2
```py
isbn = input()
tmp=0
arr1=[]
ans=0
for i in isbn:
    if i == 'X':
        tmp+=10
        arr1.append(tmp)
    else:
        tmp+=int(i)
        arr1.append(tmp)

for i in range(len(arr1)):
    ans+=arr1[i]
print("YES") if ans%11==0 else print("NO")
```

```py
isbn = input()
tmp=0
arr1=[]
ans=0
for i in isbn:
    if i == 'X':
        tmp+=10
        arr1.append(tmp)
    else:
        tmp+=int(i)
        arr1.append(tmp)

for i in range(len(arr1)):
    ans+=arr1[i]
if ans%11==0: 
    print("YES")
else:
    print("NO")
```

