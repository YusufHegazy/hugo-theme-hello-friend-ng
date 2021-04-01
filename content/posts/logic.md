---
title: "A Journey into Mathematical Logic"
date: 2021-04-01T20:19:31+02:00
draft: false
toc: false
images:
tags:
  - untagged
---

## Diophantus of Alexandria
Diophantus was a Greek mathematician that flourshied at around 250 AD, he is most famous for his book "Arithmetica" in which he had compiled 130 algebraic problems among thirteen books where most of their solutions were positive integers, and that's why mathematicians call such algebraic equations as "Diophantine Equations".

Diophantus had a brilliant way in solving problems involving multiple variables using only a single variable, he did it in such a way that he finds relations which represent the other variables in terms of the first variable.

For Example, In his first problem of the fourth book:

> "Divide a given number into two cubes such that the sum of their sides is a given number".

He then provides two numbers:
> - Given Number: 370
> - Sum of Sides: 10

### Normal Approach
We can visualize the problem Geomterically as follows:
{{< image src="/img/logic/cubes.png" width="50" alt="two cubes X and Y" position="center" style="border-radius: 8px;"  >}}
Let's solve it using second grade algebra!

The two sides ($x$ and $y$) add up to 10 and the sum of their cubes  is 370.\
$x + y = 10$\
$x^3 + y^3 = 370$

$x = 10 - y$\
$(10 - y)^3 + y^3 = 370$\
$(1000 + 30y^2 - 300y - y^3) + y^3 = 370$\
$30y^2 - 300y + 630 = 0$\
$y^2 - 10y + 21 = 0$\
$(y - 7)(y - 3) = 0$\
**y = 7, y = 3**

I didn't want to bother with detailed explaination of the steps above (I hope all of those who are reading this know some basic algebra), here is how Diophantus solved such problems.
### Diophantus's Approach
He would first express the two variables (x and y) as two relations in terms of one variable so his x will be (x+5) and his y will be (x-5).\
$(x + 5) + (x - 5) = 10$

These indeed satisfy the first equation and will yield 10 upon adding them together, and for the second equation he describes it as follows:\
$(5 + x)^3 + (5 - x)^3 = 370$

It will seem a bit odd and crazy at first, but once we start expanding these cubes, terms will start cancelling out like crazy until we are left with:\
$30x^2 + 250 = 370$

Which will yield:\
$x^2 = 4$

Finally we arrive at the same solution:\
$x = 2$\
$(x + 5) = {\bf 7}$\
$(x - 5) = {\bf 3}$

his problems may seem plain and simple at the first glance but they sometimes become very tough and hard to attack, "Every question requires a quite special method, which often will not serve even for the most closely allied problems. It is on that account difficult for a modern mathematician even after studying 100 Diophantine solutions to solve the 101th problem"
