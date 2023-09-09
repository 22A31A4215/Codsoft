# Codsoft
#password generator
import random
lower_letters="abcdefghijklmnopqrstuvwxyz"
upper_letters="ABCDEFGHIJKLMNOPQRSTUVWXYZ"
numbers="0123456789"
symbols="@#$_&/:;*!?^"
combining=upper_letters+lower_letters+numbers+symbols
length=int(input())
password="".join(random.sample (combining,length))
print("your password is", password)|

#simple calculator
number1= int(input("enter number1"))
number2= int(input("enter number2"))
print("1. Addition")
print("2.Subtraction") 
print("3. Multiplication")
print("4.Division")
option= int(input("enter your option"))
if option==1:
  print(number1+number2)
elif option=-2:
  print(number1-number2)
elif option=-3:
  print (number 1*number2)
elif option==4:
  print (number1/number2)
else:
  print("default option once check again")

  #quiz game
def quiz_guess(guess,answer):
    global score
    guessing=True
    attempt=0
    while guessing and attempt<3:
        if guess.lower()==answer.lower():
            print("correct answer")
            score=score+1
            guessing=False
        elif attempt<2:
            guess=input("sry try again")
            attempt=attempt+1
        elif attempt==3:
            print(answer)
score=0
print("all the best")
guess1=input("what is full form of ai")
quiz_guess(guess1,"artificial intelligence ")
guess2=input("when did ai started")
quiz_guess(guess2,"1943")
guess3=input("who is inventor of ai")
quiz_guess(guess3,"johnMcCarthy")
print("your score ",str(score))
  
