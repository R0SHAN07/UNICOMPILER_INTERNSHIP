# UNICOMPILER_INTERNSHIP
#TASK-1(NUMBER GUESSING)
#TASK-1 
import random
a=random.randrange(1,101)
score=100
print("\t Welcome to the GUESSING GAME \t")
print("Find the hidden number\n")
print("Your initial score is :",score)
print("\nRule : 5 points will be deducted from your initial  score for every incorrect guess")
print("Let's begin the game\n")
n=int(input("Enter a number between 1-100 : "))
while(n!=a):
  score-=5
  if(a>n):
      print("Oops !!! Your guess is incorrect...")
      print("Hint : Enter a larger number...\n")
      if(a%2==0):{
          print("Hint :The hidden number is divisible by 2\n")
      }
      elif(a%3==0):{
          print("Hint :The hidden number is divisible by 3\n")
      }
      elif(a%5==0):{
          print("Hint :The hidden number is divisible by 5\n")
      }
      n=int(input("Enter your next guess :\n "))
  elif(a<n):
      print("Oops !!! Your guess is incorrect...")
      print("Hint : Enter a smaller number...\n")
      if(a%2==0):{
          print("Hint :The hidden number is divisible by 2\n")
      }
      elif(a%3==0):{
          print("Hint :The hidden number is divisible by 3\n")
      }
      elif(a%5==0):{
          print("Hint :The hidden number is divisible by 5\n")
      }
      n=int(input("Enter your next guess :\n "))
if(a==n):
  print("CONGRATULATION!!! You Guessed correctly ...\n The number was :",n)
print("Your final score is :",score)
