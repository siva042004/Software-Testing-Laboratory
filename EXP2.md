# Ex.No: 2   Matrix Multiplication 

### DATE:01/10/2024                                                                            
### REGISTER NUMBER : 212221040155

### AIM: 
Write a python program for matrix multiplication and inspect for failures.
 
### Algorithm:

Algorithm:
1. Start the program.
2. Create empty list formatrix1, matrix2 and result.
3. Get the rows and columns count from the user.
4. Get the values of two matrix.
5. Perform matrix multiplication and store the answer in result.
6. Stop the program.
### Program:
```

r1, c1 = input("Enter row and column count in matrix 1: ").split()
r2, c2 = input("Enter row and column count in matrix 2: ").split()
matrix1 = []
matrix2 = []
result = []
if r1.isnumeric() and c1.isnumeric() and r2.isnumeric() and c2.isnumeric():
    r1 = int(r1)
    c1 = int(c1)
    r2 = int(r2)
    c2 = int(c2)
    if c1 != r2:
        print("Matrix multiplication not possible due to column of matrix 1 not equal to row of matrix 2.")
    elif max(r1, c1, r2, c2) > 20 or min(r1, c1, r2, c2) == 0:
        print("Matrix multiplication not possible due to size constraints (max size 20x20 or size 0).")
    else:
        
        print("Enter elements of matrix 1:")
        for i in range(r1):
            a = []
            for j in range(c1):
                a.append(int(input(f"Element [{i+1},{j+1}]: ")))
            matrix1.append(a)
        for i in range(r2):
            a = []
            for j in range(c2):
                a.append(int(input(f"Element [{i+1},{j+1}]: ")))
            matrix2.append(a)

        result = [[0 for _ in range(c2)] for _ in range(r1)]  # Initialize result matrix with zeros
        for i in range(r1):
            for j in range(c2):
                sum = 0
                for k in range(c1):  
                    sum += matrix1[i][k] * matrix2[k][j]
                result[i][j] = sum
        print("Resultant Matrix:")
        for i in range(r1):
            for j in range(c2):
                print(result[i][j], end=" ")
            print()

else:
    print("Enter valid numeric values for rows and columns.")

```

### Output:


![stl ex-2 output](https://github.com/user-attachments/assets/d040a000-20bc-41af-b3a1-f62f7e7775e5)











### Result:
Thus, the python program for matrix multiplication is implemented and the causes for its failure is introspected successfully.

