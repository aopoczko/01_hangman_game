import random

print("H A N G M A N")

while True:    
    print('Type "play" to play the game, "exit" to quit:', end="")
    choice = input()
    if choice == "exit":
        break
    elif choice != "play":
        continue
    else:
        pass

    word = str(random.choice(['python', 'java', 'kotlin', 'javascript']))   #random word to guess
    text = ("-" * len(word))    #changing string
    tries = 8                   #lives
    letters = set()

    while tries > 0:
        
            
        print()
        print(text)
        print('Input a letter: ', end="")
        
        guess = input()

        if len(guess) > 1 or len(guess) < 1:
            print("You should input a single letter")
            continue
        else:
            pass


        if guess.islower():
            pass
        else:
            print("Please enter a lowercase English letter")
            continue
    
        if len(guess) > 1 or len(guess) < 1:
            print("You should input a single letter")
            continue
        else:
            pass
        
        if guess in letters:
            print("You've already guessed this letter") 
            continue   
        else:
            letters.add(guess)
                
        
        if guess in text or guess not in word:
            tries -= 1
            if guess in text:
                print("No improvements")
            else:
                print("That letter doesn't appear in the word")
            if tries == 0:
                print("You lost!")    
            continue

        
        if guess in word:
            for j in range(len(word)):
                if guess == word[j]:
                    text = text[:j] + guess + text[j+1:]
            
            if text == word:
                print("You guessed the word!")
                print("You survived!")
                break
            else:
                continue
                
            
        
