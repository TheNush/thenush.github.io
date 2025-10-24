---
layout: post
title: "Geometric proof that Gaussian integers form a principal ring"
author: "Dhanush Giriyan"
categories: "proofs"
tags:   [ring-theory, geometry]
---

### Preliminary Definitions
We begin with preliminary definitions for completeness. 

**Definition 1.** A *ring* is a set $R$ equipped with two binary operations, denoted by $+$ and $\cdot$, such that

- $(R,+)$ is an abelian additive group with identity element $0$
- $R$ contains a unit element denoted by $1$, i.e., for every $x \in R$, $1\cdot x=x\cdot 1 = x$
- for all $a,b,c \in R$, multiplication satisfies associativity:

$$
\begin{align*}
a\cdot (b \cdot c) = (a\cdot b)\cdot c
\end{align*}
$$

- for all $a,b,c \in R$, multiplication distributes over addition in the usual sense:

$$
\begin{align*}
a\cdot (b+c) &= a\cdot b + a\cdot c \text{(left distributivity)}\\
(a+b)\cdot c &= a\cdot c + a\cdot c \text{(right distributivity)}
\end{align*}
$$

A ring is said to be *commutative* if for all $a,b \in R, a\cdot b = b\cdot a$.
We will restrict ourselves to the setting of commutative rings for the rest of this post. 

**Definition 2.** A subset $I$ of a ring $R$ is called an *ideal* of the ring if for all $r \in R$ and $a,b \in I$:

- $a+b \in I$
- $-a \in I$
- $r\cdot a, a\cdot r \in I$

In other words, $I$ is a subgroup of $(R,+)$ and is closed under multiplication by elements of $R$. 
An ideal is said to be *principal* if it can be expressed in the form of $xR=Rx$ for some $x \in R$. 

Finally, a ring wherein every ideal of the ring is principal is referred to as a *principal ring*. 

---WORK IN PROGRESS---
