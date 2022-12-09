# Basic-python-questions



###  to use the operators

a=int(input("Enter the first number:"))
b=int(input("Enter the second number:"))
add=a+b
sub=a-b
multi=a*b
div=a/b
remain=a%b
power=a**b
print('addtion',add)
print('subtraction',sub)
print('multiplication',multi)
print('division',div)
print('reaminder',remain)
print('power',power)



### to find a perfect number

n = int(input("Enter any number: "))
sum1 = 0
for i in range(1, n):
    if(n % i == 0):
        sum1 = sum1 + i
if (sum1 == n):
    print("The number is a Perfect number!")
else:
    print("The number is not a Perfect number!")





### To check a amrmstrong number 

n=int(input("Enter any number to check : "))
x=(n-(n%100))/100
y=((n-(n%10))/10)-x*10
z=n%10
if n == x**3+y**3+z**3:
    print("this is a armstrong number")
else:
    print("this is not a armstrong number")

## write a program to find a factorial

num = int(input("Enter a number: "))    
factorial = 1    
if num < 0:    
   print(" Factorial does not exist for negative numbers")    
elif num == 0:    
   print("The factorial of 0 is 1")    
else:    
   for i in range(1,num + 1):    
       factorial = factorial*i    
   print("The factorial of",num,"is",factorial)





### to print fibonacci series

nterms = int(input("How many terms? "))


n1, n2 = 0, 1
count = 0

if nterms <= 0:
   print("Please enter a positive integer")
elif nterms == 1:
   print("Fibonacci sequence upto",nterms,":")
   print(n1)
else:
   print("Fibonacci sequence:")
   while count < nterms:
       print(n1)
       nth = n1 + n2
       n1 = n2
       n2 = nth
       count += 1
       
       
       
       

### to check a palindromic string

x= input("enter a string: ")
y=x[::-1]
if x==y:
    print("this is a palindrome")
else:
    print("not a palindraome")
