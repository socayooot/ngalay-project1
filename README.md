# ngalay-project1
Inside this repository lies the first Assembly Project.

a) Nathan Galay CS 2160 MW (12:15PM - 1:30PM). 

To run the program:
1: compile the code in https://comparch.edu.cvut.cz/qtrvsim/app/
2: press run until "Enter a message:" is shown
3: open the terminal and enter some word
4: hit run until your message is fully displayed

In this assignment, you will find part 1 and part 2 of the project

The code will explain what each function aims to do

b) test cases and test programs will be provided in the final code

c) 

Sources:
https://stackoverflow.com/questions/78064202/how-can-i-implement-the-c-puts-function-in-risc-v-assembly (checking what other people did and comparing to my initial code)
https://chatgpt.com/ (explaining why certain code works and fixing bugs) (chatGPT also explained to me that I was writing my methods wrong, and handling memory incorrectly, specifically the buffer and the ra. 
Notes: Additionally, looking back at my notes, I noticed that when you are dealing with memory in general, you need to have the prolog, body, and epilog.

d) I had a rough time understanding how to write my methods and understanding why the code fits together. A string is essentially a memory address that needs to be stored and the ra also needs to be stored so that data is not inevitibaly lost. I first got confused about this concept which lead to my first initial commits to have no thought into how the memory worked and it caused lots of bugs and issues that I struggled to fix. To fix my problems, I used chatGPT to explain to me how the code works with itself and additionally what the code actually does until I understood.

Additionally, starting was probably the hardest part of the project. Knowing where to start and what to do took a lot longer than it should. 

In other words, the hardest part of the project was probably memory control and tracking where it goes. When I looked at the registers, it still was confusing to understand and most of the time, I used my own imagination to think about what is happening with the registers and memory.

e) easily 25+ hours. To complete this project, I allegated 1.5 - 2 weeks to work on the project in small portions so I don't feel too stressed.

f) Unlike the first project, when there is nothing inputted into the terminal, I will not get an error, I will get an infinite loop that runs and infinite ecall and I am not sure what is going on there.
