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
