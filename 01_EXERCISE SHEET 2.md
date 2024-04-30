# EXERCISE 2
## Q1. Which keyword is used to create a function? Create a function to return a list of odd numbers in the range of 1 to 25.

A1. def keyword is used to create a function in python. A function to return a list of odd numbers in the range of 1 to 25:

    def even():
        l1=[]
        for i in range(1,26):
            if i%2==0:
                l1.append(i)
         print(l1)

## Q2. Why *args and **kwargs is used in some functions? Create a function each for *args and **kwargs to demonstrate their use.
A2. *args and **kwargs are used to implement dynamic arguments in a function. *args is unsed to store data in a tuple while **kwargs is used to store data in a dictionary.

    def fn(*args):
        return args


    def f1(**kwargs)
        return kwargs


## Q3. What is a generator function in python? Why yield keyword is used? Give an example of a generator function.

A3. A generator function returns a generator iterator which is used to iterate over a sequence.Following function is a generator function which eventually prints even number from the given inputs :

    def even(*num):
        l1=[]
        for i in num:
             if i%2==0:
                yield i
        for i in even(1,2,3,4,5,6,7,8,9,10):
            print(i)
     
## Q4. Create a generator function for prime numbers less than 1000. Use the next() method to print the first 20 prime numbers.

A4. THE REQUIRED FUNCTION IS BELOW:
    
    def prime():
    for i in range(1,1001):
        k=0
        n=i
        while n>0:
            if i%n==0:
                k+=1
            n-=1
        if k<3:
            yield i
    prm = prime()
    for i in range(20):
        print(next(prm))

## Q5. Write a python program to print the first 10 Fibonacci numbers using a while loop.

A5. PROGRAM TO PRINT FIRST 10 FIBONACCI SERIES NUMBERS:

     def fibo():
         a,b=0,1
         s=0
         n=10
         while n>0:
            print(a)
            s=a+b
            a=b
            b=s
            n-=1

