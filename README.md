# Python-Project1
 Number Guess Game
 import random
def start_game():
  print('Welcome to the number guessing game! \nGuess the number 1-10')
  number = 1
  x = random.randint(1, 10)
  y= None 
    
  while x !=y:
    try:
      y = float(input('guess the number   '))
      
    except ValueError:
      print('need a number 1-10')
    else:
      if y>10 or y<1:
        
        print('must be a number from 0 - 10')
        print('Needs to be within 1-10')
        number +=1
        continue
        
      elif y > x :
          print("It's Lower")
          number +=1
              
      elif y < x:
          print("It's Higher")
          number +=1
      
      elif y == x:
        break
        
  
  print('Got it')
  z= 'you took {} times to get the answer!'.format(number)
  print(z+ 'thanks for playing')

  
      
    
  

  
              
              
              
      



