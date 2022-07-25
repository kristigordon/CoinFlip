# CoinFlip

I started importing libraries and using a broader array of functionality. 

Here is a project using the random library and producing a random integer, either 1 or 0.

From this a pulled this randomly generated number into an if statement and printed Heads if 1 and Tails if 0.

I included some ASCII art to make things a little more fun. 

Here is my code:
```
import random
print("Welcome to the Coin Flip")
print('''
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⢀⡀⠀⠀⠀⠠⠤⠤⠤⠶⠶⠤⣤⣄⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠠⢊⣡⣶⣿⡷⠀⠀⠀⣀⣠⣤⣤⣤⣄⢹⡇⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⢿⠿⠟⠋⠀⠀⠀⣾⠉⠀⠀⠀⣀⣤⠞⢴⣆⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠙⠛⠒⠚⠛⠉⠁⠀⠀⣿⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠸⠁⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣾⣷⣶⣶⡄⠀⢸⣿⣦⡀⠀⠀⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢀⣀⣉⠉⠉⠀⠀⠀⠻⣿⣿⣷⡄⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠘⠛⠿⠿⢿⠆⢶⣦⣄⣿⣿⣿⣿⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣼⣿⣶⣶⣦⠀⢸⣿⣿⣿⣿⣿⣿⠀⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⢠⣬⣉⣉⣛⠀⢸⣿⣿⣿⣿⣿⣿⣄⠀⠀⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⣿⣿⠿⠟⠁⢸⣿⣿⣿⣿⣿⣿⣿⣷⡄⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠈⠉⠛⠶⠾⠿⠿⢿⣿⣿⣿⣿⣿⣿⡇⠀
⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠀⠉⠉⠉⠉⠉⠉⠁⠀''')

guess = input("Type your guess: Heads or Tails\n")

flip = random.randint(0, 1)

if flip == 1:
    print('''You flipped Heads!
          
        _.-'~~`~~'-._
     .'`  B   E   R  `'.
    / I               T \
  /`       .-'~"-.       `\
 ; L      / `-    \      Y ;
;        />  `.  -.|        ;
|       /_     '-.__)       |
|        |-  _.' \ |        |
;        `~~;     \\        ;
 ;  INGODWE /      \\)     ;
  \  TRUST '.___.-'`"     /
   `\                   /`
     '._   1 9 9 2   _.'
        `'-..,,,..-'`

''')
else:
    print(''' You flipped Tails
    
             _.oood"""""""booo._
         _.o""      _____    * ""o._
       oP"  _.ooo""""   """"o|o*_* "Yo
     o8   oP                 | |"._* `8o
    d'  o8'_.--._            | |/  ,\* `b
   d'  d'.' __   ".          | |: (( `\
  8'  d'/,-"  `.   :         | |  ||\_/* `8
 8   8'|/      :   :    |)   _ |  || |`|   8
,8  8          :  :   /)| \ || |\_|| | |8  8.
8' ,8         /  :    " /_) |`:' | | | |8. `8
8  8'        /  /       _ _='  \ ' __   __  8
8  8        /  /        \|__ |  | |  | | 8| 8
8  8.      /  /         ||   |  | |-:' | 8| 8
8. `8    ,' ,'       __/ |__ |__| |  \ |__|,8
`8  8  ,' ,'      _ /     __ . . . . . .8LL8'
 8   8"   `------'/(    ,'  `.`. | | ,-|8  8
  8.(_________dd_/  \__/ '  0|`.`: |: (8 ,8
   Y.  Y.                    | :/| |,\|* .P
    Y.  "8.          .,o     | | |,|"*  ,P
     "8.  "Yo_               | |p|"* ,8"
       "Y_   `"ooo.__   __.oo|"* * _P"
         `'"oo_     """""    * _oo""'
              `"""boooooood"""'
              ''')

print(f"Your guess was {guess}")
```

![Screen Shot 2022-07-24 at 10 58 51 PM](https://user-images.githubusercontent.com/66803124/180688058-85675fce-b003-4a77-920a-d6b857efcd1b.png)
