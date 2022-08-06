def Selection(x):
    for i in range (len(x)-1):
        min = i
        for j in range (i+1,len(x)):
            if x[j] < x[min]:
                min = j

        if min != 1:
            x[min],x[i] = x[i],x[min]




x=list(map(int,input().split()))
Selection(x)
print(x)
