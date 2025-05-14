# Python-Code
//print Greatest Common division

n1=int( input("Enter Your Num"))
n2=int(input("Enter your num"))
gcd=1
for i in range(2,n1):
    if(n1%i==0 and n2%i==0):
        gcd=i
print(gcd)

//find Maximum nums in Array

nums=[2,4,5,6,7,8,9]
max=nums[0]
for i in range(1,7):
    if(nums[i]>max):
        max=nums[i]
print(max)


//print pattern in python

n=int(input("Enter your number"))
for i in range(1,n):
    for j in range(1,i):
        print(j,end=" ")
    print()

    //print Palindrome or not

    
num=int(input("Enter your number"))
reverse=0
temp=num
while(temp!=0):
    rem=temp%10
    reverse=reverse*10+rem
    temp=temp//10
if(num==reverse):
    print("Palindrome")
else:
    print("not Palindrome")

    //print Fectorail

    
def Fectorial(n):
    xFact=1
    for i in range(2,n+1):
        xFact*=i
    return xFact
print("Fectorial is",Fectorial(5))
//Sieve of Eratosthenes theorm to find prime number in range n

def sieve(n):
    isPrime=[True]*(n+1)
    isPrime[0]=isPrime[1]=False
    for i in range(2,int(n**0.5)+1):
        if isPrime[i]:
            for j in range(i*i,n+1,i):
                isPrime[j]=False
    for i in range(2,n+1):
        if(isPrime[i]):
            print(i,end =' ')
n=int(input("Enter your number"))
sieve(n)

//print combination 

def fectorial(n):
    xFact=1
    for i in range (1,n+1):
        xFact*=i
    return xFact
def combination(n,r):
    return fectorial(n)//(fectorial(r)*fectorial(n-r))
n=int(input("Enter your Number"))
r=int(input("Enter value of r"))
cpr = combination(n, r)
print(cpr)
