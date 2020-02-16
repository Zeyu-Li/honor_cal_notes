# Honors Math

## About

This is a summery of **Honors Calculus** (117 + 118) (or as some people call it: "**Abstract Calculus**")
This course will focus on set theory and number theory (and logic)

\* note this won't display properly on GitHub, I use a program called [Typora](https://typora.io/) with inline math enabled

## Index

1. Sets
2. Logic
3. What is a number? (It's not what you think it is)
4. Induction
5. Absolute values
6. Intervals and bounds
7. Real numbers
8. Sequences and limits
9. Functions (and notation)
10. Continuity
11. 1-sided limits
12. min/max and sup/inf
13. Rolle's theorem
14. Intermediate value theorem
15. Mean value theorem (Meme value theorem)
16. Differentiation
17. First and second derivative test
18. L'Hopital's Rule (Le hospital)
19. Taylor's Theorem
20. Convex and concave
21. Inverse functions
22. Implicit differentiation
23. Exponentials and logs
24. Logarithmic differentiation



## Notes

#### 0. Shorthand

Ex. $\to$ example

Thm $\to$ Theorem (will be in block quotes)

s.t. $\to$ such that

##### Formal Logic

$\in \to$ element of

$\sub\ or\subseteq\ \to$ subset of

$\cup \to$ union

$\cap \to$ intercept



$\and \to$ and

$\or \to$ or

$\to\ \to$ then

$\iff \to$ if and only if (this is the same as \'\=\')

$=: \to$ is defined to be



$\forall \to$ for all

$\exist \to$ there exists

$\exist! \to$ there exists unique



$Q.E.D. \to$ and it is proved

$\therefore\ \to$ therefore 

$\because\ \to$ because



##### Fields

$\N \to$ natural numbers (i.e. 1,2,3,4...) [\* note 0 might be included in natural numbers depending on what text book is in use]

$W \to$ whole numbers ($\{0\} \cup \N$) 

$\Z \to$ integers (i.e. ..-2,-1,0,1,2...)

$\Q \to$ rational numbers (anything that can be expressed as $\frac{p}{q}, where\ p\in\Z\ and \ q\in\N$)

$\R \to$ will be discussed later

#### 1. Sets

a set is defined as a number (can be 0 but then that would be the trivial or stupid set) of elements belonging to the same group

> Ex. 
>
> * {1,2,3} = {2,1,3}
> * {a,b}
> * {even, odd}
> * $\N$ = {1,2,3,4,5...}
> * {} (trivial set)

If an element 'x' is part of a set 'A', it is described as $x\in A$

If $A \cup B = A,\ B\sub A$. If for all elements of B are in A, then B is considered a subset of A

If elements of A are present in B, then those elements 'C' are said to be $A\cap B$ or $A\cap B=C$ 

![venn diagram](pics/figure1venn.png)

From Bowmen notes

#### 2. Logic

##### Truth Values

There are 2 truth values, true (T or topology) and false (F or contradiction)

In math, there are established rules (which were set arbitrarily but is important for consistence around the world) for operations on truth values

Most of the time, a truth table will be used to illustrate how operators effect the truth value of a statement

Some common ones are:

$A\and B$ ; (A and B)

|      |      | A    | A    |
| ---- | ---- | ---- | ---- |
|      |      | T    | F    |
| B    | T    | T    | F    |
| B    | F    | F    | F    |

$A\or B$  ; (A or B)

|      |      | A    | A    |
| ---- | ---- | ---- | ---- |
|      |      | T    | F    |
| B    | T    | T    | T    |
| B    | F    | T    | F    |

$A\to B$  ; (If A then B)

|      |      | A    | A    |
| ---- | ---- | ---- | ---- |
|      |      | T    | F    |
| B    | T    | T    | T    |
| B    | F    | F    | T    |

$A\iff B$  ; (A if and only if B or A = B)

\* note this is a different way for displaying the truth table (important for chain multiple operators with more than 2 variables)

| A    | B    | $A\iff\ B$ | $A\to B\ and\ B\to A$ |
| ---- | ---- | ---------- | --------------------- |
| T    | T    | T          | T                     |
| T    | F    | F          | F                     |
| F    | T    | F          | F                     |
| F    | F    | T          | T                     |

To chain multiple operators together, you can use an extended truth table that considers all the variables (like the one above, but you must consider all variables and all the cases possible use a )

As seen from the table above, an iff is logically equivalent to a if b and b if a, therefore for proving an iff, the easiest way is to prove it using the A premise to get to B and then using the B premise to derive A



##### Contraction

The easiest way to prove something is to use *proof by contradiction*. Assume the opposite of the theorem or a fact that is true and find a contraction in reasoning

> Ex. 
>
> $\sqrt{2}\ is\ not\ rational$
>
> Start of proof by contraction:
>
> ​	Suppose for contradiction, $\sqrt{2}\ is\ rational$, i.e. it can be expressed as $\frac{p}{q}, where\ p\in\Z\ and \ q\in\N$. 
> $$
> \sqrt{2} = \frac{p}{q}\\
> \to \sqrt{2}^2 = \frac{p^2}{q^2}\\
> 2q^2=p^2
> $$
> \* note even number are expressed as 2n and odd number can be expressed as 2n+1 for $n\in\Z$
>
> Therefore p must be even because only an even squared is even $((2n)^2=4n^2\ and\ (2n+1)^2 = 4n^2+2n+1\therefore odd)$

#### 3. What is a number? (Algebraic Properties)

For real numbers, the following must be true

\* assume $a,b,c \in \R$ 

1. Must be associative

> $a+(b+c)=(a+b)+c$

2. Must have an additive identity

> $a+0=0+a=a$

3. Must have an *additive inverse* -a s.t. 

> $a+-a=-a+a=0$

4. Follows additive commutativity

> $a+b=b+a$

5. Are associate

> $a(bc)=(ab)c$

6. There exists are multiplicative identity where it is not 0

> $a\times 1= a$

7. It can distribute

> $a\times (b+c)=a\times b+a\times c$

8. Has an inverse that is not 0, i.e. $a^{-1}\ne 0$

> $a\times a^{-1}=1$

9. Follows multiplicative commutativity

> $a\times b=b\times a$

10. Trichotomy Law

> must be one and only one of the following relations:
>
> $a<b,\ a=b,\ a>b$

11. Closed under addition

> $a>0\ and \ b>0\to a+b>0$

12. Closed under multiplication

> $a>0\ and \ b>0\to a\times b>0$

More rules to come

Also note the first lemma (lemma is like a theorem but arbitrary defined to be a small theorem)

\* lemmas or thm can be assumed

![figure2midway](pics/figure2midway.png)

#### 4. Induction



## Resources

* school notes
* [Bowmen notes](http://www.math.ualberta.ca/~bowman/m117/m117.pdf)

### Note about this course and my experience

----

My school had an extraordinary honors calculus year. The main prof left by second semester and a German prof can in to sub, but, because of his Germanicness (he literally goes off of a German textbook), it was difficult to follow his sometimes rigorous and sometimes not rigorous (he called them trivial) proofs. 

Also, at my university, compute 272 is trivially similar to 117. 

## Licence

The rules for copy and distributing this project licence are 
outlined in the licence.txt file.

This project is under an MIT licence 


## Contributions

Contribute if and only if you know what you are doing (and optionally, it would help if you where Germanic or fluent in Germanics)

\* If someone wants to convert this to Latex, go ahead and pull request (must have a index or contents page with links)

