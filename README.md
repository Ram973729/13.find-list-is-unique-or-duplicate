# 13.find-list-is-unique-or-duplicate
n=int(input('Enter how many numbers you want:'))
l=list(map(int,input().split()))
a=0
for i in range(n):
    for j in range (i+1,n):
        if l[i]==l[j]:
            a=a+1
if a!=0:
    print('Duplicate List')
else:
    print('Unique List')
