# Problem-Difficulties
You have prepared four problems. The difficulty levels of the problems are A1,A2,A3,A4 respectively. A problem set comprises at least two problems and no two problems in a problem set should have the same difficulty level. A problem can belong to at most one problem set. Output the maximum number of problem sets you can create using the four problems.


m=int(input())
for i in range (m):
    p=list(map(int,input().split()))
    a=set(p)
    if(len(a)==4):
        print(2)
    elif(len(a)==3):
        print(2)
    elif(len(a)==2):
        p.sort()
        b = p[0]
        if(p.count(b)==2):
            print(2)
        else:
            print(1)
    else:
        print(0)
