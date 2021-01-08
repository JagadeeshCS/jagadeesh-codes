# jagadeesh-codes
def gcd(x,y):
    small = min(x,y)
    for i in range(1,small):
        if x%i == 0 and y%i == 0:
            gcd = i
    return gcd

def euclid(x,y):
    while y:
        x, y = y, x%y

    return x

def expo(x,y):
    if y == 0:
        return 1
    else:
        return x * expo(x,y-1)

def exp():
    x = int(input("enter base value:"))
    y = int(input("enter exponent value:"))
    p = 0
    p = x**y
    print(x,"power",y,"=",p)

