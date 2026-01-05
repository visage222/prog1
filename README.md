Program 1: Print numbers from 1 to 10 using a for loop.

# Print numbers from 1 to 10 using a for loop
for i in range(1, 11):
    print(i)
    

Program 2: Find if a number is even or odd using if-else statement.

# Check if a number is even or odd
num = int(input("Enter a number: "))

# Use if-else statement to check even or odd
if num % 2 == 0:
    print(f"{num} is even.")
else:
    print(f"{num} is odd.")


Program 3: Print multiplication table of a number (using a loop).

# Print multiplication table of a number
num = int(input("Enter a number: "))

for i in range(1, 11):
    print(num, "x", i, "=", num * i)


Program 4: Count how many times a specific number appears in a list (using for loop and if).

# Count how many times a number appears in a list
numbers = [1, 2, 3, 4, 2, 5, 2, 6, 2]
target = int(input("Enter the number to count: "))

count = 0

for num in numbers:
    if num == target:
        count += 1

print(f"The number {target} appears {count} times in the list.")


Program 5: Sum all numbers in a list (using a for loop).

# Sum all numbers in a list
numbers = [10, 20, 30, 40, 50]

total = 0

for num in numbers:
    total += num

print("The sum of all numbers in the list is:", total)



Program 6: Create a program that checks if a number is prime.

num = int(input("Enter a number: "))

for i in range(2, num):
    if num % i == 0:
        print(num, "is not a prime number.")
        break
else:
    if num > 1:
        print(num, "is a prime number.")
    else:
        print(num, "is not a prime number.")


Program 7: Print Fibonacci series up to a certain limit.

limit = int(input("Enter the limit: "))

a, b = 0, 1

while a <= limit:
    print(a, end=" ")
    a, b = b, a + b


Program 8: Program to check if a number is divisible by both 3 and 5.

num = int(input("Enter a number: "))

if num % 3 == 0 and num % 5 == 0:
    print(num, "is divisible by both 3 and 5.")
else:
    print(num, "is not divisible by both 3 and 5.")


Program 9: Find the largest number in a list.

numbers = [10, 45, 23, 67, 12, 89, 34]

largest = numbers[0]  # Assume the first number is the largest

for num in numbers:
    if num > largest:
        largest = num

print("The largest number in the list is:", largest)


Program 10: Reverse a string using a for loop.

# Reverse a string using a for loop
text = input("Enter a string: ")
reversed_text = ""

for char in text:
    reversed_text = char + reversed_text  # Add current character at the beginning

print("Reversed string:", reversed_text)


Program 11: Sum numbers from 1 to n using a while loop.

total = 0
i = 1

while i <= 5:
    total += i
    i += 1

print("The sum of numbers from 1 to 5 is:", total)


Program 12: Check if a string is a palindrome.

# Check if a string is a palindrome
text = input("Enter a string: ")

# Remove spaces and make lowercase for accurate checking
text = text.replace(" ", "").lower()

if text == text[::-1]:
    print("The string is a palindrome.")
else:
    print("The string is not a palindrome.")


Program 13: Print all prime numbers between 1 and 100.

# Print all prime numbers between 1 and 100
for num in range(2, 101):  # Start from 2, since 1 is not prime
    is_prime = True
    for i in range(2, int(num**0.5) + 1):
        if num % i == 0:
            is_prime = False
            break
    if is_prime:
        print(num, end=" ")




Program 14: Program to check if a number is positive, negative, or zero using if-elif-else.# Check if a number is positive, negative, or zero
num = float(input("Enter a number: "))

if num > 0:
    print(num, "is positive.")
elif num < 0:
    print(num, "is negative.")
else:
    print("The number is zero.")


Program 15: Create a program that prints a triangle pattern using a loop.

# Print a triangle pattern
rows = int(input("Enter the number of rows: "))

for i in range(1, rows + 1):
    print("*" * i)
