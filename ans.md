**我先打lol等等寫第二組**

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
P3
```py
def f3(s):
    cnt={}
    for c in s.lower():
        if c.isalpha():
            if c in cnt:
                cnt[c]+=1
            else:
                cnt[c]=1
    return dict(sorted(cnt.items()))

def test():  
    s=input()  
    print(f3(s))  

if __name__=="__main__":
    test()
```
P4
```py
s=input()
def f(s):
    if len(s) != 7 or not s.islower():
        return "error"
    ans=""
    for i in range(1,7):
        tmp=abs(ord(s[i])-ord(s[i-1]))
        if tmp>=10:
            tmp=tmp%10
        ans+=str(tmp)
    return ans
print(f(s))

```
P5
```py
def sn_check(sn):
    st=sn.split("-")
    arr=[7, 11, 13, 17, 23]
    for i in range(len(st)):
        if len(st[i])!= 5 or i>=len(arr):
            return st[i]
        sum=0
        for char in st[i]:
            sum+=ord(char)
        if sum%arr[i] != 0:
            return st[i]
    return "valid"


def test():
    while True:
        sn=input()
        if sn=="":
            break
        print(sn_check(sn))

if __name__ == '__main__':
    test()
```
