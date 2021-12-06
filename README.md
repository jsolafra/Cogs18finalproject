# Cogs18finalproject
print ("After the Wilson Abrams High School reunion for the class of 1996 you have volunteered along with 11 other people to clean up the venue, but suddenly the lights go out. With the lights off you hear a blood curdling scream, only for the lights to be turned back on revealing your ex-class president and social butterfly Eve with a multiple stab wounds in the middle of the venue. When you ask who did this to her, she takes her last breathe. With you being a detective and your childhood bestfriend, Hunter, being a deputy you secure the crime scene knowing that you have a new case on your hands.") 

print("The people who were present at the time of the incident were; Jace the Jock, Chelsey the Cheerleader, Jimmy the Nerd, Blair the Emo girl, Cody the Gamer boy, Jazzie the Theater kid, Thiago the Gangster, Hunter your childhood friend, and Katie the Quiet Kid.")
Suspect = ["Jace", "Chelsey","Jimmy","Blair","Cody", "Jazzie", "Thiago", "Hunter","Katie"]


answer = input("Would you like to start the investigation?(yes/no?)")
if answer.lower().strip() == "yes":
    answer = input("It is time to look for clues, would you like Hunter to help or do it yourself?")
    
    if answer == "Hunter":
        answer = input("He says he found a note. And says it is in Jace's handwriting. Do you believe him?(yes/no?)")
        
        if answer == "Yes":
             print ("You arrested Jace, but he was innocent. Game over")
        else:
            print ("You interrogate Jace and find out he is not the killer, you eliminate a possible suspect.But Jace does say Jimmy and Eve once dated and that can be motive. Do you believe him?(Y/N?)")
            if answer == "Y":
                print ("Jimmy gives you an albi because he was picking up Dj Equipment. But he says he saw chelsey have an argument with eve. Interrogate chelsey or arrest her?")
                if answer == "Arrest":
                    print("She is innocent. You get sued and you loose your job. Game over and Cold Case Bro")
                    
                else:
                    print ("She suddenly dies due to poison in the interrogation room and you find another note saying, Sorry brother. do you think it is a murder/suicide or is the killer still at large?")
                    if answer == "Murder/Suicide":
                        print("Murder is considered solved, but Chelsey was not the murderer. you failed as a detective. Game over")
                    elif answer == "Killer still at large":
                        print("You realize Hunter says that to you as a joke. With a broken heart you make the arrest. Case Closed. Congrat brother hehe")
                    
            else:
                print (" You don't belive Eve would like Jimmy. So you interrogate Thiago. Thiago confesses and you make an arrest. Later evidence shows he is not guilty. Cold Case ")
                
    
    
    elif answer == "Myself":
            answer = input("You find the murder weapon with finger prints and a note. Should you run DNA or analyze writing?")
            
            if answer == "DNA":
                print("The lab was able to narrow down to three suspects Thiago, Chelsey, Jimmy. You also discover Jace is killed after he never returned from the bathroom.")
            else:
                print("You see the writing can match Blair, Katie, and Jace. But Thiago was killed after trying to look at the footage tapes")
                      
    

else:
    print("You shouldn't be a detective!")
                     
     
