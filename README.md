# VDCoding01
the first try to GITHUB codez
<br>
import random
<br>
'''
Rules of the game 
1 for Rock choose r
0 for Paper choose p
-1 for Scissor choose s
'''
<br>
computer= random.choice([-1,0,1])
<br>
youstr= input("Enter your move:")
<br>
youDict={"r":1,"p":0,"s":-1}
<br>
reverseDict={1:"Rock", 0:"Paper", -1:"Scissor"}
<br>
you=youDict[youstr]
<br>
#by now we have 2 number(Variables), that are You/User and Computer

print(f"You chose {reverseDict[you]}\nComputer chose {reverseDict[computer]}")
<br>
if(computer==you):
    print("The game ended at a Draw!")
else:
    if(computer==1 and you==0):
        print("Congratulations! You Won!")
    elif(computer==0 and you==-1):
        print("Congratulations! You Won!")
    elif(computer==-1 and you==1):
        print("Congratulations! You Won!")
    elif(computer==0 and you==1):
        print("BOO! You Lost!")
    elif(computer==-1 and you==0):
        print("BOO! You Lost!")
    elif(computer==1 and you==-1):
        print("BOO! You Lost!")
