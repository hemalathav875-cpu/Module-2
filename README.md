~~~
MODULE 2

Built-in Functions -Binary Conversion Using Built-in Functions in Python

##Aim:

To write a Python program to convert the number 16 into its binary representation using built-in Python functions.

##Algorithm:

Assign the value 16 to a variable a.
Use the built-in bin() function to convert the number to binary.
Print the result.

##Program

number = 16
binary_representation = bin(number)
print(binary_representation)


Output

<img width="1175" height="355" alt="image" src="https://github.com/user-attachments/assets/fff81fb6-b9f1-4072-8be7-19f7552b54bb" />


Result:

Thus program has been executed successfully



Functions in Python: Modulo Calculator

## Aim
To write a Python program that defines a function which accepts two values and returns their modulo using the % operator.

##Algorithm

Define a function called result that takes two arguments a and b.
Inside the function, compute the modulo using a % b.
Print the result of the modulo operation.
Get two integer inputs from the user.
Call the result function with the user-provided values.

##Program

def calculate_modulo(a, b):
    return a % b

result = calculate_modulo(10, 3)
print(result)


Output

<img width="1187" height="301" alt="image" src="https://github.com/user-attachments/assets/be78c256-ac37-46bf-b14f-254cb22a4245" />

Result
 Thus program has been executed successfully


Lambda Function in Python: Addition of Two Numbers

##Aim
To write a Python program that defines a lambda function which takes two arguments a and b, and returns their sum.

##Algorithm

Get two integer inputs from the user.
Use a lambda function to define a function f that returns a + b.
Call the function with the user inputs and print the result.


##Program

add_numbers = lambda a, b: a + b

print(add_numbers(5, 3))


Output

<img width="1177" height="380" alt="image" src="https://github.com/user-attachments/assets/d9487a75-df03-4ff8-8067-ae3abbbab2da" />

Result

Thus program has been executed successfully


Looping(Patterns)-Pascal's Triangle Generator in Python
This project demonstrates a simple Python program to generate Pascal’s Triangle, where the number of rows is provided by the user.

##Aim

To write a Python program that generates Pascal's Triangle using numbers. The number of rows is accepted from the user.

##Algorithm

Start the program.
Input the number of rows from the user.
Loop from 0 to the number of rows.
For each row:
Print appropriate spaces to shape the triangle.
Compute values using the formula:
[ C(n, k) = \frac{n!}{k!(n-k)!} ]
Print all rows of Pascal’s Triangle.
End the program.


##Program

rows = int(input("Enter the number of rows: "))

triangle = []

for i in range(rows):
    row = [1] * (i + 1)
    for j in range(1, i):
        row[j] = triangle[i - 1][j - 1] + triangle[i - 1][j]
    triangle.append(row)

for row in triangle:
    print(" ".join(map(str, row)))



Sample Output

<img width="1261" height="565" alt="image" src="https://github.com/user-attachments/assets/60ccf603-e9bc-41e5-8eab-c95527dd3fb6" />


Result
Thus program has been executed successfully


Loops in Python: Palindrome Number Checker


##Aim

To write a Python program that checks whether a given number is a palindrome using loops.

##Algorithm

Get input from the user and assign it to a variable num.
Assign the value of num to a temporary variable temp.
Initialize a variable rev to 0 (used to store the reversed number).
Use a while loop to reverse the digits:
While temp > 0:
rev = (10 * rev) + temp % 10
temp = temp // 10
After the loop, compare rev with num:
If equal, print that the number is a palindrome.
Else, print that it is not a palindrome.


##Program

number = int(input("Enter a number: "))

original_number = number
reversed_number = 0

while number > 0:
    remainder = number % 10
    reversed_number = (reversed_number * 10) + remainder
    number = number // 10

if original_number == reversed_number:
    print(f"{original_number} is a palindrome number.")
else:
    print(f"{original_number} is not a palindrome number.")


Output
<img width="1376" height="572" alt="image" src="https://github.com/user-attachments/assets/ab6daa8f-9492-4ddb-8ab1-6e9ee4f20cea" />


Result

Thus program has been executed successfully
~~~
