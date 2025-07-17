# function-with-in-a-function
def outer():
    print("this is a outer function.....")
    def inner():
        print("this is a inner fuction.....")
 # inner()
outer()
    
#indirect recursion
def dsum(n):
    if n==0:
        return 0
    return n%10 + temp(n//10)
def temp(n):
    return dsum(n)
num=int(input("enter a 4 digit number:"))
print("sum of digit:",dsum(num))
    
