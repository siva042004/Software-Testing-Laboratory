# Ex.No: 13  Pytest program for Sum of Digits 

### DATE: 29-10-2024                                                                          
### REGISTER NUMBER : 212221040155
### AIM: 
To write a python program for sum of digits and validate the code using Pytest. 
### Algorithm:

1. Write the python program for sum of digits of a number. 
2. Make sure that function name should be “def test_*():” and the line to be tested 
should have assert keyword at the beginning. 
3. Write some test cases for to be tested and save it as “test_sumofdig.py”. 
4. Open command prompt and change the directory to where pytest is installed
5. Executethe program as “pytest test_sumofdig.py”. 
6. Stop the program.

### Program:
```
def sum_of_digits(number: int) -> int:
    if number < 0:
        raise ValueError("Input should be a non-negative integer")
    return sum(int(digit) for digit in str(number))

def test_sum_of_digits_positive():
    assert sum_of_digits(123) == 6
    assert sum_of_digits(456) == 15
    assert sum_of_digits(98765) == 35

def test_sum_of_digits_zero():
    assert sum_of_digits(0) == 0

def test_sum_of_digits_large_number():
    assert sum_of_digits(1234567890) == 45

def test_sum_of_digits_negative():
    with pytest.raises(ValueError):
        sum_of_digits(-123)
```










### Output:
![image](https://github.com/user-attachments/assets/0d28fe04-b47d-4e13-b71a-12f81f9d622b)




### Result:
Thus, the python program for sum of digits is tested using pytest and executed and output is verified successfully.

