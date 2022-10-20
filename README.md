# Hangman
Hangman is a classic game in which a player thinks of a word and the other player tries to guess that word within a certain amount of attempts.

This is an implementation of the Hangman game, where the computer thinks of a word and the user tries to guess it. 
Milestone 1:
import random
fruits = ("banana", "mango", "orange", "starwberry", "pineapple") 
word_list = fruits
word = random.choice(word_list)
#print(word) 

guess = input("Enter a fruit: ") 
if len(guess) > 1:
    print("Good guess!")
else: 
    print("Oops! That is not a valid input.") 
    print(guess) 

Milestone 2:
while True:
    guess = input("Guess a letter: ")
    if guess.isalpha():
        print(guess)
        break
    else:
        print("Invalid letter. Please, enter a single alphabetical character.")

Milestone 3:
def ask_for_input(word):
  word = input("Enter a fruit: ") 
  if len(word) > 1:
      print("Good choice!")
  else: 
      print("Oops! That is not a valid input.") 
      print(word) 

ask_for_input('fruit') 

def check_guess(guess):
  while True:
    if guess.isalpha():
        #print(guess)
        break
    else:
        print("Invalid letter. Please, enter a single alphabetical character.") 

  if guess in word:
    print("Good guess!", guess, "is in the word.")
  else:
    print("Sorry,", guess, "is not in the word. Try again.")

  return guess.lower()

check_guess('a')
