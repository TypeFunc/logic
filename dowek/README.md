Notes from the book "Proofs and algorithms" by Gilles Dowek.


## 2017.02.02 -- Section 1.1


## BibTeX entry

    @book {MR3012378,
        AUTHOR = {Dowek, Gilles},
         TITLE = {Proofs and algorithms},
        SERIES = {Undergraduate Topics in Computer Science},
          NOTE = {An introduction to logic and computability,
                  Translated from the French by Maribel Fernandez},
     PUBLISHER = {Springer, London},
          YEAR = {2011},
         PAGES = {xii+155},
          ISBN = {978-0-85729-120-2; 978-0-85729-121-9},
       MRCLASS = {03-01 (68-01)},
      MRNUMBER = {3012378},
           DOI = {10.1007/978-0-85729-121-9},
           URL = {http://dx.doi.org/10.1007/978-0-85729-121-9},
    }

--------------------------------------------

# Part I: Proofs

# 1 Predicate Logic

## 1.1 Inductive Definitions
### 1.1.1 The Fixed Point Theorem

**Definition 1.2** (Weakly complete ordering) An ordering relation ≤ is said to be
weakly complete if each increasing sequence has a limit.

**Definition 1.3** (Increasing function) Let ≤ be an ordering relation over a set E and
f a function from E to E. The function f is increasing if x ≤ y ⇒ f x ≤ fy.

**Definition 1.4** (Continuous function) Let ≤ be a weakly complete ordering rela-
tion over the set E, and f an increasing function from E to E. The function f is
continuous if for any increasing sequence lim i (f u i ) = f (lim i u i ).

**Proposition 1.1** (First fixed point theorem) Let ≤ be a weakly complete ordering
relation over a set E that has a least element m. Let f be a function from E to E. If
f is continuous then p = lim i (f i m) is the least fixed point of f .


**Definition 1.5** (Strongly complete ordering) An ordering relation ≤ over a set E
is strongly complete if E has a least element 0 and every nonempty subset A of
E has a least upper bound, denoted by sup A. 

**Exercise 1.1** Show that any strongly complete ordering is also weakly complete.  
(done)

Is the ordering

    b       c
     \     /
      \   /
       \ /
        a
   
weakly complete? Is it strongly complete?  
(Ans: yes; no.)

**Proposition 1.2** If the ordering ≤ over the set E is strongly
complete, then any nonempty subset A of E has a greatest lower bound, inf A.

*Proof.* Let A be a nonempty subset of E. A has a least upper bound, sup
 A. Define B = { y in E | forall x in A, y ≤ x }. B is a subset of E,
 so it has a least upper bound, say l. Note
 1. forall y in B, y ≤ l
 2. (forall y in B, y ≤ l') implies l ≤ l'.

Then l is th greatest lower bound of A. Why?
 1. l is a lower bound of A since if x in A, x is an upper bound of B and
 l ≤ x.
 2. l is the greatest lower bound since if y is a lower bound of A, y
 is in B and y ≤ l.


**Proposition 1.3** (Second fixed point theorem) Let ≤ be a strongly
  complete ordering over a set E. Let f be a function from E to E. If
  f is increasing then p = inf {c | f c ≤ c} is the least fixed point
  of f.

*Proof.* Let C be the set {c | f c ≤ c} and c be an element of C. Then
 p ≤ c since p is inf C. Since f is increasing f p ≤ f c. Note f c ≤ c
 because c is an element of C. 



### 1.1.2 Inductive Definitions
### 1.1.3 Structural Induction
### 1.1.4 Derivations
### 1.1.5 The Reflexive-Transitive Closure of a Relation

----------------------------------------------

## 1.2 Languages

### 1.2.1 Languages Without Variables
### 1.2.2 Variables
### 1.2.3 Many-Sorted Languages
### 1.2.4 Substitution
### 1.2.5 Articulation

----------------------------------------------

## 1.3 The Languages of Predicate Logic

----------------------------------------------

## 1.4 Proofs

----------------------------------------------

## 1.5 Examples of Theories

----------------------------------------------

## 1.6 Variations on the Principle of the Excluded Middle
### 1.6.1 Double Negation
### 1.6.2 Multi-conclusion Sequents 
