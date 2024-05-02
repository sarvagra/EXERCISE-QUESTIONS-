# EXERCISE-3

## Q1. Create a python program to sort the given list of tuples based on integer value using a lambda function. List : <br>[('Sachin Tendulkar', 34357), ('Ricky Ponting', 27483), ('Jack Kallis', 25534), ('Virat Kohli', 24936)]

A1. Program for sorting the above list :
    
     l=[('Sachin Tendulkar', 34357), ('Ricky Ponting', 27483), ('Jack Kallis', 25534), ('Virat Kohli', 24936)]
     l2=[]
     l3=[]
     for i in l:
         l2.append(i[1])
     l2.sort()
     for j in l:
         for i in range(0,len(l)):
             if j[1]==l2[i]:
                 l3.append(j)
     print("SORTED LIST :",l3)

## Q2. Write a Python Program to find the squares of all the numbers in the given list of integers using lambda and map functions.

A2. REQUIRED CODE :
     
    l=[11,12,13,14,3,9]
    list(map(lambda x : x**2 , l))

## Q3. Write a python program to convert the given list of integers into a tuple of strings. Use map an lambda functions.

A3. REQUIRED CODE :
    
     l=[121, 144, 169, 196, 9, 81]
     tuple(map(lambda x : str(x),l))   
     

## Q4. Write a python program using reduce function to compute the product of a list containing numbers from 1 to 25.

A4. Program to compute product of a list containing numbers from 1 to 25:

     l=[]
     for i in range(1,26):
          l.append(i)
     from functools import reduce
     x= reduce(lambda x,y : x*y , l)
     print(x)

## Q5. Write a python program to filter the numbers in a given list below that are divisible by 2 and 3 using the filter function.<br>[2, 3, 6, 9, 27, 60, 90, 120, 55, 46]

A5. Required code:
     
     k=[2, 3, 6, 9, 27, 60, 90, 120, 55, 46]
     l= list(filter(lambda x : x%2==0 or x%3==0,k))
     print("Numbers divisible by 2 and 3 : ",l)

## Q6. Write a python program to find palindromes in the given list of strings using lambda and filter function. ['python', 'php', 'aba', 'radar', 'level']

A6. Program to find palindromes in the given list:

     string=['python', 'php', 'aba', 'radar', 'level']
     x=list(filter(lambda x: x==x[::-1],string))
     print("Palindromes in the list are :",x)


     
    

    