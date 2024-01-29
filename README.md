# hw1pr4

# coding: utf-8
#
# hw1pr4.py
#

""" 
Title for your adventure:   Yeah.

Notes on how to "win" or "lose" this adventure:
  To win, Pick Mark and say "yes", "Bark" is not bad either
  To lose, Pick "Mark" and say "no", or pick "Park"

"""

import time

def adventure():
    """ this function runs one session of interactive fiction
        Well, it's "fiction," depending on the pill color chosen...
        arguments: no arguments (prompted text doesn't count as an argument)
        results: no results     (printing doesn't count as a result)
    """
    delay = 0.5          # change to 0.0 for testing or speed runs,
                         # ..larger for dramatic effect!

    username = input("What is your name? ").lower()
    if username == "david":
        print("Hi David!")
    

    print()
    print("You wake up on a cold bed, unsure of where you are or how you got here,")
    print("it is dark.")
    print("Only lit by an oil lamp on the table in front of you")
    print("the only other object in the room is a small rock.")
    print()

    step1 = input("what do you do[grab it/leave it] ").lower()
    if step1 == "grab it":
        print()
        print("Yup... thats a rock")
        print("it's smooth and it fits nicely in your palm")
        print()

    else:
        print("nothing happens")
        print()
    
    print("...some time passes and you hear a series of clicking sounds from the door that leads out of the room")
    print("sounds like the door is open")
    print()

    step2 = input("do you[stay] or [leave] ").lower()
    print()

    if step2 == "stay":
        print("you stay and rot here :( ")
        print()
    else:
        print("you leave the room")
        print()
        print('you approach the a table with some large signs that read "Mark", "Bark", and "Park"')

        step3 = input('you walk towards it when a man with a devious grin says "who do you choose?" ').lower()
        print()

        if step3 == "mark":
            print('"Mark! Excellent choice."')
            print('from under the table a tall man appears with a pin on his chest that reads "Mark"')
            print("Mark introduces himself and you do the same, he seems like a swell guy.")
            print()

            music = input('after a little bit he asks you, "Tell me, whats your favorite genre of music?"').lower()
            if music == "rock":
                print('"Rock on!"')
            elif music == "pop":
                print == '"Oh nice! I like pop too."'
            elif music == "country":
                print('"oh... sorry."')
                print()
                print('you disapointed Mark')
            else: 
                print('well, everyone has their own taste')
                print()

            print("Mark leads the pair of you until you are outside where he asks you one more question.")
            print()
                
            Step2Mark = input('"Do you love me?"[yes/no/what?] ').lower()
            if Step2Mark == ("yes"):
                    print()
                    print('"I KNEW IT!!!" and before you can even think he puts a ring on your finger...')
                    print()
                    print('you and Mark are now married')
                    print()

            elif Step2Mark == "no":
                    print('"HOW could you!!!"')
                    print("he storms off crying into his hands")
                    print()
                    print("you disapointed Mark")
                    print()
                
            else:
                print('He cuts you off before you can fully respond"I KNEW IT!!!"')
                print()
                print("he puts a ring on your finger.")
                print()
                print("you and Mark are now married")
                print()
        
        elif step3 == "bark":
            print('"Interesting choice."')
            print()
            print("the man pulls a dog from behind the counter")
            print('on its collar it reads "Bark" ')
            
            input("confused you ask him whats going on. What do you say ")
            print()

            print("...despite what you say")
            print("the man shrugs and points in the direction of the exit")
            print()
            print("you now have a dog... Nice!")
            print("you leave, your dog in your arms ready to face whatever comes next...")

        elif step3 == "park":
            print()
            print("He stares at you for a second...")
            print("after a bit he hands you a pot with a plant in it")
            print('sticking out of the pot is a label that reads "Park"')
            print()
            print('"you should probably go plant that."the man says as he points towards the exit')
            print()
            
            Step2Park = input("what do you do[stay/leave] ").lower()

            if Step2Park == "leave":
                print("you leave and enter the outdoors")
                print('in a nearby patch of dirt you plant "Park"')
                print("the end")
            else:
                print('the man frowns as you refuse to leave and takes "Park" from you')
                print("he leaves out the exit and locks the door behind him")
                print("there is no other way out")
                print("you stay and rot here") 
