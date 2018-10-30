# Algorithms: What Lies Behind the program

## The Basics of Computer Science Part II

---

## Algorithms

If you’ve done any programming, or dabbled in computer science, you have likely heard the term algorithm. Wikipedia defines an algorithm as: a step-by-step procedure for calculations. That may sound familiar; in the first part of this series, we defined a program as: the precise, step-by-step description of what must happen.

But “algorithm” isn’t just a fancy word for “program” — they’re related, but they are not the same thing. Importantly, an algorithm is a specific type of abstraction.

An algorithm is an abstract description of the how to perform a task. A program is the specific description of how to perform the task, written in a particular programming language.

### Hansel and Gretel

Hansel and Gretel is a classic fairy tale that has a well-known plot: who doesn’t love a good gingerbread house?

The plot is independent of a particular telling of the tale. The story can be in German, English or Swahili. Many different versions have been told, though they remain recognisably Hansel and Gretel.

The plot is the “algorithm” for Hansel and Gretel: the essentials of the tale. The particular wordings used to tell a story are like the programs.

## How useful are algorithms?

How useful is it to think about an abstract algorithm, rather than just writing a program?

### Algorithms are ways of creating things

An algorithm can be a surprisingly compact way of defining how to accomplish a task. Here’s an example:

If I asked you to list all the numbers, how long would it take you? The answer is “forever, and then some” since numbers stretch out to infinity.

Consider this algorithm, which lists all the numbers:

```
Start at 1
Repeat:
   Add 1 to the last number
```

In three lines we have a complete description of how to generate all the numbers. In a sense, this is a very compact representation of all the numbers.

An algorithm is the detailed process you follow to create something, rather than the thing itself. In this example, the algorithm tells you how to generate all the numbers, rather than being the list of all the numbers.

For many tasks, it is easier to write the algorithm for generating the desired results, rather than creating the results themselves. In particular, many interesting problems have an impractically large (sometimes even infinite) range of possible outcomes, so writing the algorithm is a lot easier.

### Thinking in Algorithms

Creating an algorithm to solve a task is a useful mental discipline. You have to consider every aspect of the task, then think through the steps required to complete it.

The core skill is breaking down complex tasks into manageable, repeatable pieces.

Here’s an example of this: I need more cash. What do I do? One way to solve this problem is to:

```
Walk to the nearest ATM
Put your bank card in
Enter your PIN
Enter how much money you need
Retrieve your bank card
Take your money
Walk home
```

Each of these tasks can be further broken down, for example walk to the nearest ATM could become:


```
Turn right at your front gate
Walk to the end of the road
Turn left at the junction
Walk to the main road
Cross the main road and walk up to the bank
```

You can keep breaking these tasks down for as long as you want or need.

The level of precision and thoroughness required to write a good algorithm helps you be thoughtful and logical in your approach to problem solving. These are useful skills in an increasingly technological world.

## Measuring Algorithm Efficiency

When you create an algorithm you obviously want it to correctly solve the problem at hand; but you should also consider how efficient the algorithm is. For many problems, it’s easy to create an algorithm that either takes a very long time to complete or never finishes at all. Clearly a correct algorithm that takes a short time to complete is preferable to one that takes a long time, or forever.

There is a whole area of Computer Science dedicated to calculating the efficiency of algorithms. While the details of doing this are beyond the scope of this post, there are lots of resources to help if you want to find out more: a good place to start is to search for “Big O notation”.

Probably the most widely used algorithms are the ones that sort a list of things. On the surface, sorting seems easy, but it turns out there are a lots of sorting algorithms, and their efficiency varies wildly.

A great place to start with sorting algorithms is the CS Unplugged site. I particularly like their sorting networks video, which shows how you can make a sorting algorithm work with nothing more than a playground, some chalk and a group of enthusiastic school children — no computers required.
