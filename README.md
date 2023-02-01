# Q.1	Write a program to implement List Operations(Nested list, Length, Concatenation, Membership ,Iteration ,Indexing and Slicing), List Methods(Add, Append, Extend & Delete) 			[15 M] 
```
List1 = [34,'shubham',45,'python',657,'scala',9999] 
List2 = [788,5,499,45,499,67]

Sum = sum(List2)
print("Sum of all elements in List2 : ",Sum)

#nested list
Nested_List = ["Happy", [2,0,1,5],['s','k']]
print("Nested List is : ",Nested_List)

#length
Length = len(List1)
print("Length of List1 : ",Length)

#concatenation
List3=List1+List2
print("Concatenation of List1 & List2 is : ",List3)

#membership
ele='shubham'
if ele in List1:
   print(ele,"is member of List1")
else:
   print(ele,"is not a member of List1")

#list iteration
print("Iteration in List1 : ")
for i in List1: 
    print(i)
print()

#indexing
print("Index of 499 in List2 : ",List2.index(499))

#slicing
Slice_List1 = List1[2:5]
print("Slice_List1 is elements from 2 to 5 index of List1 : ",Slice_List1) 

#insertion in list
List1.insert(2,'kulkarni')      
print("List1 after Inserting 'kulkarni' at position 2 : ",List1)

#append to the list
List1.append(205) 
print("List1 after Appending 205 : ",List1)

#extend a list into another list
List1.extend(List2)         
print("After Adding List2 into List1 : ",List1)

#remove item at index
List2.pop(4)
print("List2 after delete element at 4 position : ",List2)

print("List2 after sorting : ",sorted(List2))


```
Output

Sum of all elements in List2 :  1903
Nested List is :  ['Happy', [2, 0, 1, 5], ['s', 'k']]
Length of List1 :  7
Concatenation of List1 & List2 is :  [34, 'shubham', 45, 'python', 657, 'scala', 9999, 788, 5, 499, 45, 499, 67]
shubham is member of List1
Iteration in List1 : 
34
shubham
45
python
657
scala
9999

Index of 499 in List2 :  2
Slice_List1 is elements from 2 to 5 index of List1 :  [45, 'python', 657]
List1 after Inserting 'kulkarni' at position 2 :  [34, 'shubham', 'kulkarni', 45, 'python', 657, 'scala', 9999]
List1 after Appending 205 :  [34, 'shubham', 'kulkarni', 45, 'python', 657, 'scala', 9999, 205]
After Adding List2 into List1 :  [34, 'shubham', 'kulkarni', 45, 'python', 657, 'scala', 9999, 205, 788, 5, 499, 45, 499, 67]
List2 after delete element at 4 position :  [788, 5, 499, 45, 67]
List2 after sorting :  [5, 45, 67, 499, 788]



































# Q.2  Program to print multiplication table for given no. 		[10 M] 

```
num = int(input("Enter the number: "))

print("Multiplication Table of", num)
for i in range(1, 11):
   print(num,"X",i,"=",num * i)
   
```

Output
Enter the number: 12
Multiplication Table of 12
12 X 1 = 12
12 X 2 = 24
12 X 3 = 36
12 X 4 = 48
12 X 5 = 60
12 X 6 = 72
12 X 7 = 84
12 X 8 = 96
12 X 9 = 108
12 X 10 = 120















# Q.3	Write a program to Illustrate Different Set Operations. 	[15 M] 

```
A = {0, 2, 4, 6, 8}; 
B = {1, 2, 3, 4, 5}; 

print("Set A : ",A)
print("Set B : ",B)
#union 
print("Union :", A | B) 
  
#intersection 
print("Intersection :", A & B) 
  
#difference = elements in A not in B
print("Difference :", A - B) 
  
#symmetric difference = elements in A not in B & elements in B not in A
print("Symmetric difference :", A ^ B)

```
Output

Set A :  {0, 2, 4, 6, 8}
Set B :  {1, 2, 3, 4, 5}
Union : {0, 1, 2, 3, 4, 5, 6, 8}
Intersection : {2, 4}
Difference : {0, 8, 6}
Symmetric difference : {0, 1, 3, 5, 6, 8}











# Q.4  Program to check whether the given no is prime or not.  [10 M]

```
number = int(input("Enter any number: "))

if number > 1:
    for i in range(2, number):
        if (number % i) == 0:
            print(number, "is not a prime number")
            break
    else:
        print(number, "is a prime number")
else:
    print(number, "is not a prime number")
    
```

Output

Enter any number: 23
23 is a prime number




















# Q.5 Write a program to implement Simple Chatbot. 		[15 M] 

```
qna={
     "hii":"hey",
     "how are you" "":"I am fine",
     "what is your name":"my name is suhas",
     "how old are you":"i am 21 years old",
 }
 
while True:
   qs=input()
   if(qs=="quit"):
    break
   else:
      print(qna [qs])
      
```   

output

how are you
I am fine








# Q.6 Program to find factorial of the given no  * With Recursive Function [10 M]

```
def factorial(num):
    
    if num == 1:
        return num
    else:
        return num * factorial(num - 1)
	
num = int(input("Enter a Number: "))

if num < 0:
    print("Factorial cannot be found for negative numbers")
elif num == 0:
    print("Factorial of 0 is 1")
else:
    print("Factorial of", num, "is: ", factorial(num))
```

OR
```
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
   
```

Output
Enter a Number: 5
Factorial of 5 is:  120




# Q.7 Write a program to implement Breadth First Search Traversal. [15 M]              
```
graph = {'a':['b','c'],
        'b':['a','d','e'],
        'c':['a','f','g'],
        'd':['b'],
        'e':['b'],
        'f':['c'],
        'g':['c']}
        
def bfs(graph,initial):
      visited=[]
      queue=[initial]
      
      while queue:
        node=queue.pop(0)
        if node not in visited:
           visited.append(node)
           neighbours=graph[node]
    
           for neighbour in neighbours:
              queue.append(neighbour)
      return visited
print("breath first traversal string")
print(bfs(graph,'a'))

```   
   
output 

breath first traversal string
['a', 'b', 'c', 'd', 'e', 'f', 'g']  
     
     







# Q.8 Write a program to implement Depth First Search Traversal. [15M] 

```
graph = { 
'5':['3','7'], 
'3':['2','4'],
'7':['8'],
'2':[],
'4':['8'],
'8':[]
}

visited = set() # Set to keep track of visited nodes of graph.
def dfs(visited, graph, node): #function for dfs
  if node not in visited:
     print (node) 
  visited.add(node)
  for neighbour in graph[node]: 
      dfs(visited, graph, neighbour)
  #Driver Code
print("Following is the Depth-First Search") 
dfs(visited, graph, '5')

```
output


Following is the Depth-First Search
5
3
2
4
8
7







# Q.9 Write a program to implement Water Jug Problem.         [15 M] 

```
x = 0 
y = 0 
m = 4
n = 3
print("Initial state = (0,0)")
print("Capacities = (4,3)")
print("Goal state = (2,y)")
while x != 2:
  r = int(input("Enter rule:"))
  if(r == 1):
    x = m
  elif(r == 2):
    y = n
  elif(r == 3):
    x = 0
  elif(r == 4):
    y = 0
  elif(r == 5):
    t = n - y
    y = n
    x -= t
  elif(r == 6):
    t = m - x
    x = m
    y -= t
  elif(r == 7):
    y += x
    x = 0
  elif(r == 8):
    x += y
    y = 0
  print (x, y)
  
```  

output

Initial state = (0,0)
Capacities = (4,3)
Goal state = (2,y)
Enter rule:1
4 0

