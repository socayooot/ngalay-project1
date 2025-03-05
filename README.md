# ngalay-project1
Inside this repository lies the first Assembly Project.

a) Nathan Galay CS 2160 MW (12:15PM - 1:30PM). 

To run the program:
1: compile the code in https://comparch.edu.cvut.cz/qtrvsim/app/
2: press run until "Enter a message:" is shown
3: open the terminal and enter some word
4: hit run until your message is fully displayed
5: If you continue to hit run, you will hit an error code

In this assignment, you will find part 1 and part 2 of the project

The code will explain what each function aims to do inside the final submission code.

b) test cases and test programs will be provided in the final code submission folder

c) 

Sources:
https://stackoverflow.com/questions/78064202/how-can-i-implement-the-c-puts-function-in-risc-v-assembly (The open source code that I looked at did not work and I had to write my own code. The general basis of looking at other code was to see how people formatted and how people approached the problem. In the link given, they have a similar approach to the initial project1.s) 

https://chatgpt.com/ (explaining why certain code works and fixing bugs) (chatGPT also explained to me that I was writing my methods wrong, and handling memory incorrectly, specifically the buffer and the ra. 

Notes: Additionally, looking back at my notes, I noticed that when you are dealing with memory in general, you need to have the prolog, body, and epilog.

d) I had a rough time understanding how to write my methods and understanding why the code fits together. From ChatGPT, a string is essentially a memory address that needs to be stored and the ra also needs to be stored so that data is not inevitibaly lost. I first got confused about this concept which lead to my first initial commits to have no thought into how the memory worked and it caused lots of bugs and issues that I struggled to fix. In the beginning, my methods seemed like they worked but the data was getting lost because I had no forethought in storing and making sure that the memory is working correctly. To fix my problems, I used chatGPT to explain to me how the code works with itself and additionally what the code actually does until I understood.

Additionally, starting was probably the hardest part of the project. Knowing where to start and what to do took a lot longer than it should. The way that I approached starting was looking at other source code and looking at project part 2. I essentially used the second part of the project as a template to start and then start writing methods. One by one I would write my code and then test it.

I should note that if the initial code was not given in the beginning in part 2, I would be extremely lost and desperate. We did not really work with strings in class, so understanding how they work and how you interact with them in Assembly in this project was something that I spent a lot of time on. The functions that allow the computer to tell the kernel to write to STDOUT and take from STDIN is still something that I am trying to grasp but I understand it much better than I did. One of the things I can touch upon is the buffer, the buffer isn't something that I did not really understand in C, but I finally got to see how it works in Assembly and it is extremely helpful when working with characters for a temporary amount of time and manipulate.

In other words, the hardest part of the project was probably memory control, tracking where it goes, and interacting with strings Additionally, debugging in Assembly is probably one of the hardest things to do because of how long it takes and understanding what each instruction is doing.

I also spent some time researching but I had an issue with the directions call and jal. In the case of call, I learned that call will have a chance to sometimes mess with the address of something that you're trying to preserve/manipulate/etc. In the case of call v. jal, I learned that it is safer to use jal rather than call. With this idea in mind, I also changed my code to not have shortcut commands like call and j and rather changing them to jal and beq. Although, they are effectively the same thing, it is better to play it safe. The problem that I faced with this was when I used call v. jal in my puts function, the message prompt would get cut off and it would start to print empty characters rather than the actual characters whcih indicates that there is something going wrong with the memory.

Talking with other students, there was an issue with knowing where to place functions in the code. Some people placed the functions at the top and some people placed it below main. I opted to place my functions below main and I could not figure out if there were errors associated with the position of the functions. There were times when I thought that the placement of the methods caused some issues with the code during compilation.

e) easily 25+ hours. To complete this project, I allegated 1.5 - 2 weeks to work on the project in small portions so I don't feel too stressed. However, I spent a lot of time researching and learning and trying to understand how addresses and strings work together.

f)

Some of the bugs that I experienced were that the characters were not getting taken. In some of my first iterations, I struggled with figuring out how to get the character into memory addresses to manipulate. 

I had many cases where my code broke out into infinite loops. Within these infinite loops, when I looked at the registers, there would only be one register where the memory is repeating the same address over and over. There were times when I was trying to run the infinite loop and then the entire site would freeze and I would lose all my code because of this infinite loop. I am unsure what happened here.

One of the biggest issues I had fixing was when I had the code to kind of work. When I went to print the message, my code would display empty characters and I spent a lot of time here researching and trying to understand memory concepts and strings. 
