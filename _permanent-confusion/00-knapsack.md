---
title: The knapsack problem
subtitle: "How to write a book / P and NP / leaving home"
layout: one
image: >
    <plasher data-size="constant" data-size-params="100" data-map="constant" data-params="20000"></plasher>
    <plasher data-size="constant" data-size-params="50" data-map="constant" data-params="20000"></plasher>
    <plasher data-size="constant" data-size-params="20" data-map="constant" data-params="1000"></plasher>
    <plasher data-size="constant" data-size-params="10" data-map="constant" data-params="5"></plasher>
    <plasher data-size="constant" data-size-params="5" data-map="constant" data-params="5"></plasher>
    <plasher data-size="constant" data-size-params="2" data-map="constant" data-params="5"></plasher>
    <plasher data-size="constant" data-size-params="1" data-map="constant" data-params="5"></plasher>
---

> The way you can go
> isn’t the real way.
> The name you can say
> isn’t the real name. 


The Knapsack problem can be described in the following way (and yes, I do realize that this is not the best way to start a book, but bear with me (or don't, it's your choice, obviously), as the problem is very interesting, plus there will be a sex scene at the end and this part is, like, suuuper relevant for understanding its context): you have a backpack ("knapsack" is another word for backpack), with a given volume, say 10 liters (or we can say "10 gallons", if you are American (although, "yuck")), and a bunch of objects that you want to put there, each object with a different volume, say 1 liter, 2 liters, 3 liters and 5 liters and you want to fill it up, leaving no empty space. And you want to devise a general way to determine which objects you want to take, which works in all cases i.e. an algorithm.

You can, for example, start putting objects from lightest to heaviest - in this case you would put 1 liter and then 2 liters and then 3, but then you wouldn't be able to take the big 5 liter object. You can start from heaviest to lightest, then you would take 5, 3 and 2 and you would fill the 10 liter backpack to its full capacity, so this is a solution, but for this case, but not for others, e.g. if you have a 6 liter object instead of the 1 liter one (so 2, 3, 5, and 6) - in this case, the lightest-first *would* work. Of course, there are more complex solutions that would work in both cases, however, no solution that works in *all* cases have been found so far (except just trying all possible combinations of objects).

Checking if a given set of objects constitutes a solution to the knapsack problem is easy - you just have to sum a few numbers. But actually "finding" a solution for it, is a lengthy process (for just 5 objects you have 5 * 4 * 3 * 2 * 1 = 120 combinations that you have to try out). That puts the Knapsack problem in a very special class of algorithmic problems called "NP". What's even more interesting is that most problems in "NP" are "NP-complete" - this means that if you find a solution for one of such problems, then you'd have found a solution for all other problems of that class, so it's like all of them are different formulation of one and the same problem. 

Most people think that there is no such solution (that P is not equal to NP), and that is indeed the logical conclusion of the fact that no one managed to prove otherwise for more than 50 years. But on the other hand, it seems that there must be, right? Because else what is this weird problem doing in the middle of the computation complexity ladder, neither here nor there? It must be there for a reason. Because of this, I still think that it's worth trying to solve the Knapsack problem, and I sometimes do that after school or during it. This is a like a hobby for me. I started doing it before I knew most of this stuff, actually. But even after understanding it and knowing that it is probably impossible, I am still a believer - one thing that I know is that, in math, nothing is coincidental, so if it looks like there is a way, then there must be one.

A real-life scenario where I thought that I'd test this problem was when I left my family home for the first time and I had to fit all my possessions that I wanted to take with me in a backpack. I decided that I would take all the objects that I wanted to take and to try many different combinations until I find the most efficient one, however, I abandoned this plan even before I started packing, as a thought came to me which was quite depressing - even if I knew how to solve the knapsack problem, I wouldn't help me much with packing my belongings and deciding what to take. As hugely important this problem was, it suddenly seemed minuscule, even compared to my little dilemmas, the attachments that I had to some of my stuff, and my *lack of information* as to the place where I was going. 
