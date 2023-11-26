# University-Assignments
#Exercise 1:
#Write a program using a for loop to print the numbers from 1 to 10.
for i in range(1, 11):
    print(i)
#Exercise 2:
#Create a program that uses a for loop to print the multiplication table of a user-inputted number.
num = int(input("Enter a number: "))

for i in range(1, 11):
    print(num, 'x', i, '=', num*i)
#Exercise 3:
#Write a program using a while loop to find the sum of natural numbers up to a given number entered by the user.
num = int(input("Enter a number: "))
sum = 0
i = 1

while i <= num:
    sum += i
    i += 1

print("The sum of natural numbers up to", num, "is", sum)
#Exercise 4:
#Create a program that uses a for loop to iterate through a list of names and prints each name.
names = ['Alice', 'Bob', 'Charlie', 'David']

for name in names:
    print(name)
#Exercise 5:
#Write a program using a while loop to find the factorial of a user-inputted number.
num = int(input("Enter a number: "))
factorial = 1
i = 1

while i <= num:
    factorial *= i
    i += 1

print("The factorial of", num, "is", factorial)
#Exercise 6:
#Create a program using a for loop to print the Fibonacci series up to a specified number of terms entered by the user.
n = int(input("Enter the number of terms: "))

# initialize the first two terms
a, b = 0, 1

# print the first two terms
print(a, b, end=" ")

# loop from 2 to n
for i in range(2, n):
    # calculate the next term
    c = a + b
    # print the next term
    print(c, end=" ")
    # update the values of a and b
    a, b = b, c
#Exercise 7:
#Write a program using a while loop to reverse a number entered by the user.
num = int(input("Enter a number: "))
reversed_num = 0

while num > 0:
    digit = num % 10
    reversed_num = reversed_num * 10 + digit
    num //= 10

print("The reversed number is:", reversed_num)
#Exercise 8:
#Create a program that uses a for loop to iterate through a string and count the number of vowels.
string = input("Enter a string: ")
vowels = "aeiouAEIOU"
count = 0

for char in string:
    if char in vowels:
        count += 1

print("The number of vowels in the string is:", count)
#Exercise 9:
#Write a program using a while loop to check if a user-inputted number is a palindrome.
num = int(input("Enter a number: "))
temp = num
reverse_num = 0

while temp > 0:
    digit = temp % 10
    reverse_num = reverse_num * 10 + digit
    temp //= 10

if num == reverse_num:
    print(num, "is a palindrome number")
else:
    print(num, "is not a palindrome number")
#Exercise 10:
#Create a program using a for loop to calculate and print the sum of the squares of the numbers from 1 to 5.
sum_of_squares = 0

for i in range(1, 6):
    sum_of_squares += i ** 2

print("The sum of the squares of the numbers from 1 to 5 is:", sum_of_squares)
