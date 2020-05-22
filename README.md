# Day1
#Q1 Write a program which will find all such numbers which are divisible
#by 7 but are not a multiple of 5,
#between 2000 and 3200 (both included).
#The numbers obtained should be printed in a comma-separated
#sequence on a single line.

#Hints:
#Consider use range(#begin, #end) method
for i in range(2000,3201):

    if i%7 == 0 and i%5!=0:
    
        print(i,end=',')
	
print("\b")



#Q2 With a given integral number n, write a program to
#generate a dictionary that contains (i, i*i) such that is an
#integral number between 1 and n (both included). and
#then the program should print the dictionary.
#Suppose the following input is supplied to the program:
#8
#Then, the output should be:
#{1: 1, 2: 4, 3: 9, 4: 16, 5: 25, 6: 36, 7: 49, 8: 64}
#Hints:
#In case of input data being supplied to the question, it
#should be assumed to be a console input.
#Consider use dict()

n = int(input("Enter the value of n: "))

sqr = {i : i*i for i in range(1, n+1)}

print(sqr)

#Q3 Write a program that accepts sequence of lines as input and prints
#the lines after making all characters in the sentence capitalized.
#Suppose the following input is supplied to the program:
#Hello world
#Practice makes perfect
#Then, the output should be:
#HELLO WORLD
#PRACTICE MAKES PERFECT


from string import *

lines = []

print ("Enter sequence of lines: ")

while True:

	line = input(" ")
	
	if not line:
	
		break
		
	lines.append(line.upper())

print(lines)

#Q4 Write a program to check wheather number is even or odd using if
#Else statement…

number=int(input("Please Enter a Number : "));

x=int(number/2)*2;

if(x==number):

    print("This Number is Even")
    
else:

    print("This Number is Odd")
    
    
    
    
#Q5 program that grants access only to kids aged between 8-12
#using if else statement
#Hint::
#If aged between 8 to 12 then you are allowed… welcome!!
#Otherwise Sorry not allowed ..Bye!

age = int(input('Enter the age'))

if ((age>= 8) and (age<= 12)): 

	print("YOU ARE ALLOWED. WELCOME !") 
	
else: 
	print("SORRY ! YOU ARE NOT ALLOWED. BYE !") 



