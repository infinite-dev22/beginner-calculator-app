# beginner-calculator-app
# importing time module to cause CPU delay during execution
from time import *

# function to get user input
def calculator():
    #making varibles global 
   global num1, operator, num2
   print('loading, pleasewait...')
   #time delay by stopping CPU action for 1 second
   sleep(1)
   
   print('CALCULATOR')
   #getting user input, user pmust press enter to record his values 
   num1 = float((input('\nnum1: ')))
   operator = input('\nsign: ')
   num2 = float(input('\nnum2: '))

#function to determine operator used by user using if...elif statements   
def op_determine():
     if operator == '+':
         ans = num1 + num2
         print(ans)
     elif operator == '-':
         ans = num1 - num2
         print(ans)              
     elif operator == '*':
         ans = num1 * num2
         print(ans)             
     elif operator == '/':
         ans = num1 / num2
         print(ans) 
 
# calling the functions           
calculator()
op_determine()      
