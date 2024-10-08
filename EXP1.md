# Ex.No: 1 Write programs in Python Language to demonstrate the working of followingconstructs with possible test cases: a) do…while b) while…do c) if …else d) switch e) for 

### DATE:01/10/2024                                                                         
### REGISTER NUMBER : 212221040155

### AIM:  
To write python programs for do…while, while, for, switch and if…else and test with possible test 
Cases 

### Algorithm:
1. Start the program.
2. Create separate files for each given program.
3. Write simple program for each construct.
4.  the program with possible test cases.
5. Stop the program.
### Program:
```
```

def display():
    start = input("Enter a positive value for START: ")
    end = input("Enter a positive value for END: ")
    
    if start.isnumeric() and end.isnumeric():
        start = int(start)
        end = int(end)
        
        if start < 0 or end < 0:
            print("Both values must be positive.")
            display()
            return

        while start <= end:
            print(start, end=' ')
            start += 1
        print()  # For a new line after printing the numbers
    else:
        print("Enter a valid positive number.")
        display()

display()
```
```
def display():
    start = input("Enter a positive value for START: ")
    end = input("Enter a positive value for END: ")
    
    if start.isnumeric() and end.isnumeric():
        start = int(start)
        end = int(end)
        
        while start < end:
            print(start)
            start += 1
    else:
        print("Enter a valid positive number.")
        display()

display()
```
```
def switch():
    switcher = {
        0: "even",
        1: "odd"
    }
    n = input('Enter a value for N: ')
    
    try:
        n = int(n)
        print(switcher[n % 2])
    except ValueError:
        print("Enter a valid number.")
        switch()

switch()

```

```
def compare():
    a = input("Enter a value for A: ")
    b = input("Enter a value for B: ")
    
    try:
        a = int(a)
        b = int(b)
        
        if a > b:
            print("A is greater than B")
        elif a < b:
            print("B is greater than A")
        else:
            print("A is equal to B")
    except ValueError:
        print("Enter a valid number.")

compare()
```
```
def iterate():
    string = input("Enter a string: ")
    for i in string:
        print(ord(i), end=" ")
    print() 

iterate()
```

### Output:

![stl if else-output](https://github.com/user-attachments/assets/450616be-a913-48d7-ae4a-5d4aadff485d)
![Screenshot 2024-10-04 105526](https://github.com/user-attachments/assets/5192358e-1f70-4b33-9427-5f97a4fc4816)

![switch stl-output](https://github.com/user-attachments/assets/dd14f836-5ebb-4507-a044-b90809a8e221)
![stl forloop1](https://github.com/user-attachments/assets/3144661a-d44b-4863-b27f-137cedce805d)
![stl whiledo](https://github.com/user-attachments/assets/484a7e8a-3ed0-424e-933c-77c51c78013f)










### Result:
Thus, the python program to demonstrate the working of given constructs is implemented and the output is verified successfully.


