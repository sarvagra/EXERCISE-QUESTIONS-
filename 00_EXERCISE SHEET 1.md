# EXERCISE-1
## Q1. Explain with an example each when to use a for loop and a while loop.

A1. For loop must be used when we already know the number of times the loop
     has to be executed whereas while loop is used when we do not know the
     number of executions, it terminates when a given condition turns false.
     For example:

     ->To print the multiplication table of 54 upto 10 times, for loop is used:
     
     for i in range(1,11):
         print(i,"* 56=",i*56)
    
     ->To find the number of digits in a number,while loop is used:

    number=int(input("ENTER A NUMBER"))    
    k=0
    while number !=0:
         number=number//10
         k=k+1
    
    print("Number of digits =",k)
           


## Q2. Write a python program to print the sum and product of the first 10 natural numbers using for and while loop.

A2. To find the sum and product of first 10 natural 
    numbers using for loop :
    
    sum0=0
    prod=1 

    for i in range(1,11):
        sum0+=i
        prod*=i
    
    print("SUM=",sum0)
    print("PRODUCT=",prod)

## Q3. Create a python program to compute the electricity bill for a household.<br>The per-unit charges in rupees are as follows: For the first 100 units, the user will be charged Rs. 4.5 perunit, for the next 100 units, the user will be charged Rs. 6 per unit, and for the next 100 units, the user willbe charged Rs. 10 per unit, After 300 units and above the user will be charged Rs. 20 per unit.<br>You are required to take the units of electricity consumed in a month from the user as input.<br>Your program must pass this test case: when the unit of electricity consumed by the user in a month is 310, the total electricity bill should be 2250.

A3. ELECTRICITY BILL CODE:

    units=float(input("ENTER THE NUMBER OF UNITS OF ELECTRICITY CONSUMED"))
    amt=0.0
    if units<=100:
       amt=4.5*units
    elif units>100 and units <=200:
       amt=450+(6*(units-100))
    elif units>200 and units<=300:
       amt=450+600+(10*(units-200))
    else:
       amt=450+600+1000+(20*(units-300))
    
    print("     ELECTRICITY BILL")
    print("NUMBER OF UNITS USED=",units)
    print("TOTAL AMOUNT PAYABLE=RS.",amt)

## Q4. Create a list of numbers from 1 to 100. Use for loop and while loop to calculate the cube of each number and if the cube of that number is divisible by 4 or 5 then append that number in a list and print that list.

A4. REQUIRED CODE:

    l1=[]
    lcube=[]
    lfinal=[]
    for i in range(1,101):
        l1.append(i)
        lcube.append(i*i*i)
    
    i=0
    while i<100:
        if lcube[i]%4 == 0 or lcube[i]%5== 0:
            lfinal.append(lcube[i])
    i+=1
    
    print(l1)   
    print(lcube) 
    print(lfinal) 


## Q5. Write a program to filter count vowels in the below-given string.<br>string = "I want to become a data scientist"

A5. PROGRAM TO FILTER COUNT VOWELS :
    
    string = "I want to become a data scientist"
    count=0
    l=len(string)
    for i in range(0,l-1):
        if string[i]=='a' or string[i]=='e' or string[i]='i' or string[i]='o' or string[i]='u':
            count+=1
        
    print(count)

