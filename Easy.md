## Q1
You are given a string .
Your task is to find out if the string  contains: alphanumeric characters, alphabetical characters, digits, lowercase and uppercase characters.

```
if __name__ == '__main__':
    s = input()
    print(any(i.isalnum() for i in s))
    print(any(i.isalpha() for i in s))
    print(any(i.isdigit() for i in s))
    print(any(i.islower() for i in s))
    print(any(i.isupper() for i in s))
```
note: inside any is an object of class generator



## Q2

You are given a string S and width W.
Your task is to wrap the string into a paragraph of width W.
```
def wrap(string, max_width):
    lst1 = []
    for i in range(0,len(string),max_width):
        lst1.append(string[i:i+max_width])
        
    return '\n'.join(lst1)

if __name__ == '__main__':
    string, max_width = input(), int(input())
    result = wrap(string, max_width)
    print(result)
```
Note: if join is not used, 'None' is added at the end

## Q3

Let's learn about list comprehensions! You are given three integers x,y and z representing the dimensions of a cuboid along with an integer n. Print a list of all possible coordinates given by (i,j,k) on a 3D grid where the sum of i+j+k is not equal to n. Here,0<=i<=x,0<=j<=y,0<=k<=z . Please use list comprehensions rather than multiple loops, as a learning exercise.
```
if __name__ == '__main__':
    x = int(input())
    y = int(input())
    z = int(input())
    n = int(input())
    
    s = [[i,j,k] for i in range(x+1) for j in range(y+1) for k in range(z+1) if i+j+k!=n]
    print(s)
```
## Q4
Given the participants' score sheet for your University Sports Day, you are required to find the runner-up score. You are given  scores. Store them in a list and find the score of the runner-up.
```
if __name__ == '__main__':
    n = int(input())
    arr = map(int, input().split())
    arr = sorted(set(list(arr)))
    print(arr[-2])
```
Note: set function eliminates duplicated


## Q5

The provided code stub will read in a dictionary containing key/value pairs of name:[marks] for a list of students. 
Print the average of the marks array for the student name provided, showing 2 places after the decimal
```
if __name__ == '__main__':
    n = int(input())
    student_marks = {}
    for _ in range(n):
        name, *line = input().split()
        scores = list(map(float, line))
        student_marks[name] = scores
    query_name = input()
    for key in student_marks:
        if query_name == key:
            ls = student_marks[key]
            break;
    print(format(sum(ls)/len(ls),'.2f'))
```  
Note: format function varies the number of decimal places

## Q6
Converts all the elements in list to int
```
integer_list = map(int, input().split())
```
## Q7
You are given a string and your task is to swap cases. In other words, convert all lowercase letters to uppercase letters and vice versa.
```
def swap_case(s):
    t = ''
    for i in s:
        if i.isupper():
            t+=i.lower()
        elif i.islower():
            t+=i.upper()
        else:
            t+=i
    return t
```

## Q8
the user enters a string and a substring. You have to print the number of times that the substring occurs in the given string. String traversal will take place from left to right, not from right to left.

```
def count_substring(string, sub_string):
    l = len(string)
    sl = len(sub_string)
    count=0
    for i in range(0,l-sl+1):
        if string[i:i+sl]==sub_string:
            count+=1
    return count
```

## Q9



## Q10



## Q11



## Q12



## Q13
