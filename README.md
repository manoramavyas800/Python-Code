# Python-Code
//print Greatest Common division

n1=int( input("Enter Your Num"))
n2=int(input("Enter your num"))
gcd=1
for i in range(2,n1):
    if(n1%i==0 and n2%i==0):
        gcd=i
print(gcd)
