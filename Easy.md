## Q1
You are given a string .
Your task is to find out if the string  contains: alphanumeric characters, alphabetical characters, digits, lowercase and uppercase characters.

if __name__ == '__main__':
    s = input()
    print(any(i.isalnum() for i in s))
    print(any(i.isalpha() for i in s))
    print(any(i.isdigit() for i in s))
    print(any(i.islower() for i in s))
    print(any(i.isupper() for i in s))
 
note: inside any is an object of class generator



## Q2

You are given a string S and width W.
Your task is to wrap the string into a paragraph of width W.

def wrap(string, max_width):
    lst1 = []
    for i in range(0,len(string),max_width):
        lst1.append(string[i:i+max_width])
        
    return'\n'.join(lst1)

if __name__ == '__main__':
    string, max_width = input(), int(input())
    result = wrap(string, max_width)
    print(result)

Note: if join is not used, 'None' is added at the end

## Q1



## Q1



## Q1



## Q1



## Q1



## Q1



## Q1
