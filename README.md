# Assignment-01-may-18-2022
l=list(map(int,input().split()))
n=len(l)
d={}
k=int(input())
curr_sum=0
if n==0:
    print(0)
else:
    for i in range(n):
        curr_sum=curr_sum+l[i]
    if curr_sum==k:
        p=[]
        for j in range(i+1):
            p.append(l[j])
        print(p)
    if curr_sum-k in d:
        t=[]
        t.append(l[i])
    if curr_sum in d:
        d[curr_sum]=d[curr_sum]+1
    else:
        d[curr_sum]=1
        
