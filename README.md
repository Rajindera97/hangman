# Hangman
Hangman is a classic game in which a player thinks of a word and the other player tries to guess that word within a certain amount of attempts.

This is an implementation of the Hangman game, where the computer thinks of a word and the user tries to guess it. 
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
