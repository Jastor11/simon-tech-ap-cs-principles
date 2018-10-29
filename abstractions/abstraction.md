# Abstractions: Reusing Code   

## The basics of Computer Science Part I

### Reusing Code  

The first part of this course covered the basic building blocks of
programming: loops, logic and variables. You can, in theory, write every
possible computer program using only these. But, because you have to define
everything you want the program to do, even apparently simple tasks can
require a lot of code.

We need a way of dealing with code to make it easier to manage. A
common technique is to reuse blocks of code, so that you don’t have
to keep writing the same code over and over again.

Here is an example of a re-usable block of code:

```
DEFINE SayHello age
   PRINT "Hello, you are " + age + " years old"
END
```

The first line of the code says we are defining a re-useable block of code that does a particular task. This task has a name: SayHello and a variable called age — we’ll see how that is used in a moment.

Next comes the code that performs the task — in this simple example the code displays the text “Hello, you are AGE years old”, where the word “AGE” is replaced with whatever the variable age contains. The last line tells us that this is the end of the code block.

Now you can write programs that use this code block:

```
IF age=10 THEN
   SayHello age
ELSE
   PRINT "You are not 10"
END
```

If the variable age contains 10, the code within SayHello will be run and the program will display the text “Hello, you are 10 years old”. If age is anything else, it will display the text “You are not 10”.

When we defined SayHello, we added a new instruction to our programming language. As well as using the loops, logic and variables that are built into the language, we now have another instruction we can use in programs: SayHello.

Defining SayHello has accomplished two things. First we can use it as many times as we like in our program without having to repeat the code it contains. SayHello only has one line of code in it, so that’s not a big of an advantage; but more complex code blocks could be hundreds of lines long. That would save you a lot of time and avoid potential errors — are you going to write exactly the same lines every time without a typo?

The second reason to use code blocks is to hide away complexity. Imagine you had code that performed a complex mortgage calculation, or could play Beethoven’s fifth symphony. It is much easier to think about a program that just says PlayBeethovenFifth or CalculateMortgage than to have to deal with the details of how to perform those tasks. One of the biggest challenges of being a programmer is remembering all the details of what your program does, as you are writing it. Replacing hundreds of lines of code with an easy to recall name helps a lot.

Once you have written the code that performs a task, you can forget about the detail of how the task is done and focus on using that task in your program.

All this neatly introduces the underlying computer science topic of **abstraction**.

### Abstraction

Abstraction is one of the key ideas in computer science. Abstraction is hiding away the details of how something works, leaving you to deal only with what it does. In the SayHello example, we have abstracted away the code that performs the task, leaving just the name of the task and one variable to deal with.

Once you have an abstraction, you can write programs that use the abstraction and ignore the details of how it works. Since an abstraction can also be built out of other abstractions, you can create software that does a sequence of very complex tasks, without having to understand how all the tasks are done.

Abstractions are what makes modern software possible. CPUs understand assembly language — primitive programming languages that are efficient for the CPU to run but very hard for most people to understand. Here is some code written in the “ARM” assembly language — which is the language of the CPUs used by iPhones and many other smartphones:

```
start
 MUL r0, r1, r1;
 LDR r2, =4;
 MUL r0, r2, r0;

 LDR r2, =3;
 MUL r2, r1, r2;

 ADD r0, r0, r2;

stop B stop
```

High level programming languages like Python, JavaScript, or Ruby are abstractions that hide away the details of assembly language, so thankfully you don’t need to understand any assembly language to use them.

Your web browser is another example of an abstraction: it understands how to take the URL you type in, talk over the Internet to the machines that run the website you want, get data back and convert that into the words, pictures and videos to display. But you don’t need to know how the TCP/IP protocol works, or how to render HTML or any of the other complex operations it performs. Just type in a web address and enjoy the pages that come back. All the details are abstracted away.

Abstraction let’s programmers stand on the shoulders of giants and focus on the structure of their program without having to understand all the details of how the abstracted code works.

But abstraction applies not just to programming, it is one of the major processes by which all computer software operates.
