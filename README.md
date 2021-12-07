# Cogs18finalproject
# Not much code, but it is the background of our investigation
print ("After the Wilson Abrams High School reunion for the class of 1996 you have volunteered along with 11 other people to clean up the venue, but suddenly the lights go out. With the lights off you hear a blood curdling scream, only for the lights to be turned back on revealing your ex-class president and social butterfly Eve with a multiple stab wounds in the middle of the venue. When you ask who did this to her, she takes her last breathe. With you being a detective and your childhood bestfriend, Hunter, being a deputy you secure the crime scene knowing that you have a new case on your hands.") 

print("The people who were present at the time of the incident were; Jace the Jock, Chelsey the Cheerleader, Jimmy the Nerd, Blair the Emo girl, Cody the Gamer boy, Jazzie the Theater kid, Thiago the Gangster, Hunter your childhood friend, and Katie the Quiet Kid.")
Suspects = ["Jace", "Chelsey","Jimmy","Blair","Cody", "Jazzie", "Thiago", "Hunter","Katie"]
print(Suspects)





#Introduce Yourself
#defining name, so it could be more personal for the player
name = input("What is your name, detective?\n")
print("Greetings, " + name + ". Lets solve this murder mystery!")
answer = input("Would you like to start the investigation?(yes/no?)")
#Beginning the Investigation
if answer.lower().strip() == "yes":
    answer= input("It is time to look for clues, would you like Hunter to help or do it yourself?(Yourself/Hunter)")

    if answer == "Hunter":
#What happens when you make certain selction. The if,else,elifs, give you the possible outcomes of your decsions
        answer = input("He says he found a note. And says it is in Jace's handwriting. Do you believe him?(yes/no?)")
#Here it is exanding the scenerios. Using an addition "if" statement to create more possible endings to the investigation

        if answer == "yes":
#The Game to have a possible ending. Some scenerios end, while others branch out to multiple scerios and outcomes
             print ("You arrested Jace, but he was innocent. Game over")
        else:
            answer= input("You interrogate Jace and find out he is not the killer, you eliminate a possible suspect.But Jace does say Jimmy and Eve once dated and that can be motive. Is he telling the Truth or Lieing?(Truth/Lieing)")
            
            if answer == "Truth":
                answer = input("Jimmy gives you an albi because he was hooking up with Jazzie in a closet. But he says he saw Chelsey have an argument with Eve. Interrogate chelsey or arrest her?(Interrogate/Arrest)")
#I use several Ifs, else, elif, statements in order to broaden the possibilities of different outcomes and make the game more interative
                if answer == "Arrest":
                    answer = input("She is innocent. You get sued and you loose your job. Game over and Cold Case Bro")   
                else:
                    answer = input("She suddenly dies due to poison in the interrogation room and you find another note saying, Sorry brother. do you think it is a murder/suicide or is the killer still at large?(Murder/Suicide/Killer at large)")
                    if answer == "Murder/Suicide":
                        answer = print("Murder is considered solved, but Chelsey was not the murderer. you failed as a detective. Game over")
                        
                    elif answer =="Killer at large":
                        answer=print("You realize Hunter says that to you as a joke. With a broken heart you make the arrest. Case Closed. Congrat brother hehe")        
                        
            elif answer == "Lieing":
                answer = print ("You don't belive Eve would like Jimmy. So you interrogate Thiago. Thiago confesses and you make an arrest. Later evidence shows he is not guilty. Cold Case ")
                
    
#Alternative option of the first decsion/ This essentially took you on a completely different path with completely different outcomes 
    elif answer == "Yourself":
            answer = input("You find the murder weapon with finger prints and a note. Should you run DNA or analyze writing?(DNA/Analyze)")
#How to type your decsions and options are avaialbe after each line e.g (good/bad), to help players properly play my game            
    
            if answer == "DNA":
                answer = input("The lab was able to narrow down to three suspects Thiago, Chelsey, Jimmy, but they were poised after you offered them a drink of water. You also discover Jace and Blair are killed after you noticed they disapeared. Question the remaining suspects or look at footage. (Question/ Footage/Give Up)")
                if answer == ("Question"):
#Input statements were made when the outcome of one decsion branches out to become another outcome      
                    answer == input("You've questioned all of them except Hunter, but you feel you don't need to because Katie seems to have probable cause.Should you look into Hunter or further investigate Katie? (Look into/Further Investigate)")
                    if answer==("Look into"):
                        answer = print("You discover that Hunter does not have allibi for his location during both murders. You arrest your best childhood bestfriend.")
                    else:
                        answer == input("You check Katie's phone, there you find an image she accidently took when Eve was killed. In the photo you see a hand with rings. Do you search for the rings or arrest Katie under suspicion.(Search/Arrest Her)")
                        if answer ==("Search"):
                            answer= print("You look through everybody's belongings.You find the rings covered in Eve's blood along with poison in Hunter's belongings you make the arrest. Case closed. ")
                        else:
                            answer = print("You put an innocent woman behind bars for the rest of her life. Case closed, but not solved")
#Print Statements were used to simply end the game and give final outcome           
                elif answer == ("Footage"):
                    answer = input ("You see Cody put the poison in the glasses of water before you give it to them.Do you want to arrest him now or later? (NOW/ Later)")
                    if answer == ("NOW"):
                        print("You jumped the gun and got the wrong guy.")
                    elif answer == ("Later"):
                        print("Cody confesses he did put the poison, because he is working for the real Killer, Hunter. ")

                else:
                    print("You find a message in the mirror saying You're next. And you were. RIP ")
#The language I used throughout my project is casual to make the game more understandable and more fun   
            else:
                print("You see the writing can match Blair, Katie, and Jace. But Thiago and Jazzie was killed after trying to look at the footage tapes. Do you take a break to mourn or continue the investigation?(Mourn/Continue)")
                if answer ==("Mourn"):
                    answer = print(" You showed weakness. You discovered that the killer is you bestfriend Hunter, but only after he make you the next victim")
                else:
                    answer = input("You continue investigating, but Blair, Katie, and Jace were all in the bathroom at the time of the murders.You are at a dead in with clues do you wait for the next murder or revistit the original crimescene?(Wait/Revisit)")
                    if answer == ("Revisit"):
                        print("You discover there is a fake nail stuck on the back of the murder weapon.This fake nail belonged to Chelsey. You found your murderer. ")
                    elif answer == ("Wait"):
                        print("You wait for the next murder, unknowingly it is you.")
 #Had to different endings like how you found the killer, who you wrongly accused, and if you, yourself was a victim to make this game more interesting
 #I hope you enjoyed my little game, I really liked playing detective and writer to make it!
    

else:
    print("You shouldn't be a detective!")
                     
                     
