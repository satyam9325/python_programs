## Assignment Part-1
Q1. Why do we call Python as a general purpose and high-level programming language?

Ans: Python is a programming language designed to be used for building software in a wide variety of application domains, across a multitude of hardware configurations and operating systems.

It is the programming language that enables development of a program in a much more user-friendly programming context and is generally independent of the computer's hardware architecture


Q2. Why is Python called a dynamically typed language?

Ans: It doesn’t know about the type of the variable until the code is run. So declaration is of no use. What it does is, It stores that value at some memory location and then binds that variable name to that memory container. And makes the contents of the container accessible through that variable name. So the data type does not matter. As it will get to know the type of the value at run-time.

Q3. List some pros and cons of Python programming language?

Ans:

Pros:
Beginner-friendly	
Large Community	
Flexible and Extensible	
Extensive Libraries	Work Environment
Embeddable	
Highly Scalable	
Portable	


Cons:
Issues with design
Slower than compiled languages
Security
High memory consumption
Dynamically-typed language
Garbage collection leads to potential memory losses


Q4. In what all domains can we use Python?

Ans:

1. Programming applications
2. Data Visualizations and Analysis
3. IOT applications
4. SEO
5. AI & Machine learning
6. Game Development


Q5. What are variable and how can we declare them?

Ans: Variable is a reference  point to create object and storing the values.

x = 7
y = "ineuron"

Q6. How can we take an input from the user in Python?

Ans: 

username = input("Enter username:")
print("username is : " + username)


Q7. What is the default datatype of the value that has been taken as an input using input() function?

Ans: String

Q8. What is type casting?

Ans: Converting one datatype into another datatype is known as type casting.

Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?

Ans: yes, if developer wants a user to enter multiple values from the input we have to use either split() method or List comprehension 

x, y = input("Enter two values: ").split()
x, y = [int(x) for x in input("Enter two values: ").split()] 

Q10. What are keywords?

Ans:
Python keywords are special reserved words that have specific meanings and purposes and can't be used for anything but those specific purposes.


Q11. Can we use keywords as a variable? Support your answer with reason.

Ans: No, you cannot use keyword as a variable.
it'll create ambiguity whether to take it as a keyword or a variable


Q12. What is indentation? What's the use of indentaion in Python?

Ans: Python indentation refers to adding white space before a statement to a particular block of code. 


Q13. How can we throw some output in Python?

Ans: To throw (or raise) an exception, use the raise keyword.


Q14. What are operators in Python?

Ans: Operators are used to perform operations on variables and values.


Q15. What is difference between / and // operators?

Ans: '/' is the division operator. '//' is the floor division operator. 

Q16. Write a code that gives following as an output.
```
iNeuroniNeuroniNeuroniNeuron
```

Ans: p = "iNeuron"
print(p*4)

Q17. Write a code to take a number as an input from the user and check if the number is odd or even.

Ans: 

p = 2343
if p%2 == 0:
    print("even")
else:
    print("odd")
	

Q18. What are boolean operator?

Ans: The Python Boolean type is one of Python's built-in data types. It's used to represent the truth value of an expression.

Q19. What will the output of the following?
```
1 or 0

0 and 0

True and False and True

1 or 0 or 0
```

Q20. What are conditional statements in Python?

Ans: A conditional statement as the name suggests itself, is used to handle conditions in your program. These statements guide the program while making decisions based on the conditions encountered by the program.

Q21. What is use of 'if', 'elif' and 'else' keywords?

Ans: 

1. if keyword to implement decision control. Python's syntax for executing a block conditionally
2. else condition can be optionally used to define an alternate block of statements to be executed if the boolean expression in the if condition evaluates to False
3. elif condition is used to include multiple conditional expressions after the if condition or between the if and else conditions.


Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".

Ans: 

age = int(input("Enter the age of a person: "))
if age >= 18:
    print("I can vote")
else:
    print("I can't vote")

Q23. Write a code that displays the sum of all the even numbers from the given list.
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```

Ans: 

numbers = [12, 75, 150, 180, 145, 525, 50]
sum = 0
for i in range(len(numbers)):
    if numbers[i]%2 == 0:
        sum = sum + numbers[i]
    else: 
        continue
print(sum)


Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.

Ans: 

x, y,z = [int(i) for i in input("Enter three values: ").split()] 
greater_number = 0
if x>y and x>z:
    greatest = x
elif y>z:
    greatest = y
else: 
    greatest = z
	

Q25. Write a program to display only those numbers from a list that satisfy the following conditions

- The number must be divisible by five

- If the number is greater than 150, then skip it and move to the next number

- If the number is greater than 500, then stop the loop
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```

Ans:

numbers = [12, 75, 150, 180, 145, 525, 50]
output_list = []
for i in range(len(numbers)):
    if numbers[i]%5 == 0 and numbers[i] <= 150:
        output_list.append(numbers[i])
    elif numbers[i]%5 == 0 and numbers[i] > 150 and numbers[i] <= 500:
        i = i+1
    elif numbers[i] > 500:
        break
print(output_list)