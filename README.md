# Chapter 13 — Probability, Permutations, and Combinations Notes

## 13-1 Permutations and Combinations

### Basic Counting Principle

Multiply the number of choices for each step.

Example:

* 3 shirts and 4 pants
* Total outfits = 3 × 4 = 12

---

## Permutations

A permutation is an arrangement where order matters.

Formula:

P(n,r)=\frac{n!}{(n-r)!}

Where:

* n = total objects
* r = objects chosen

Example:

* Arrange 8 students in 8 seats

P(8,8)=8!=40320

Example:

* Choose president and vice president from 8 students

P(8,2)=\frac{8!}{6!}=56

---

## Combinations

A combination is an arrangement where order does NOT matter.

Formula:

C(n,r)=\frac{n!}{(n-r)!r!}

Example:

* Choose 3 males from 9 and 4 females from 11

C(9,3)\cdot C(11,4)=27720

---

## Practice Concepts

### Telephone Numbers

If first digit cannot be 0 or 1:

* First digit: 8 choices
* Remaining 6 digits: 10 choices each

Total:

8\cdot10^6

---

### Committees

Choosing 5 students from 25:

C(25,5)

---

### Basketball Team Example

Choose:

* 1 center from 3
* 2 forwards from 5
* 2 guards from 3

Total:

C(3,1)\cdot C(5,2)\cdot C(3,2)

---

# 13-2 Permutations with Repetitions and Circular Permutations

## Permutations with Repetition

Formula:

\frac{n!}{p!q!r!}

Where repeated letters are divided out.

Example:
Word: basketball

Repeated letters:

* 2 a’s
* 2 b’s
* 2 l’s

Calculation:

\frac{10!}{2!2!2!}=453600

---

## Circular Permutations

For arrangements around a circle:

(n-1)!

Example:
6 people at a round table:

(6-1)!=120

---

## Practice Concepts

### Books Together

3 hardcovers together and 5 paperbacks together:

Treat groups as blocks.

Arrangement:

* 2 groups can switch: 2!
* Hardcovers arrange internally: 3!
* Paperbacks arrange internally: 5!

Total:

2!\cdot3!\cdot5!

---

### Watch Symbols

12 symbols around a watch face:

(12-1)!

---

# 13-3 Probability and Odds

## Probability Formula

Formula:

P(E)=\frac{\text{favorable outcomes}}{\text{total outcomes}}

---

## Example — Marbles

Bag:

* 3 black
* 5 green
* 4 yellow

Total = 12

### Probability of Green

P(green)=\frac{5}{12}

---

### Probability of Not Yellow

Not yellow:

* 3 black + 5 green = 8

P(not\ yellow)=\frac{8}{12}=\frac{2}{3}

---

### Probability of 2 Black Marbles

Use combinations:

\frac{C(3,2)}{C(12,2)}=\frac{1}{22}

---

## Odds

Odds in favor:

\text{Odds in favor}=\text{successes}:\text{failures}

Example:
70% chance of sunny weather

* Success = 70
* Failure = 30

Odds:
7:3

---

# 13-4 Probabilities of Compound Events

## Independent Events

Events do not affect each other.

Formula:

P(A\ and\ B)=P(A)\cdot P(B)

Example:
Drawing a king, replacing it, then drawing another king:

\frac{1}{13}\cdot\frac{1}{13}=\frac{1}{169}

---

## Mutually Exclusive Events

Cannot happen at the same time.

Formula:

P(A\ or\ B)=P(A)+P(B)

Example:
Yellow or blue marble:

\frac{3}{10}+\frac{2}{10}=\frac{1}{2}

---

## Mutually Inclusive Events

Can happen together.

Formula:

P(A\ or\ B)=P(A)+P(B)-P(A\ and\ B)

Example:
Face card or black card:

\frac{12}{52}+\frac{26}{52}-\frac{6}{52}=\frac{8}{13}

---

## Dependent Events

One event affects another.

Example:
Two aces drawn without replacement.

Use combinations:

\frac{C(4,2)}{C(52,2)}=\frac{1}{221}

---

# 13-5 Conditional Probability

Conditional probability means probability given that another event already happened.

Formula:

genui{"math_block_widget_always_prefetch_v2":{"content":"P(A\mid B)=\frac{P(A\cap B)}{P(B)}"}}

Where:

* A ∩ B means “A and B”

---

## Example

Box contains:

* 3 red pencils
* 4 yellow pencils

Three pencils selected.

Find probability exactly two are red GIVEN second pencil is red.

Given:

* Event B = second pencil is red
* Event A = exactly two reds

Formula:

genui{"math_block_widget_always_prefetch_v2":{"content":"P(A\mid B)=\frac{P(A\cap B)}{P(B)}"}}

Result:

\frac{1}{2}

---

# 13-6 Binomial Theorem and Probability

A binomial experiment:

* Fixed number of trials
* Only two outcomes
* Independent events
* Same probability each trial

---

## Binomial Probability Formula

P(x)=C(n,x)p^x(1-p)^{n-x}

Where:

* n = trials
* x = successes
* p = probability of success

---

## Example — Word Game

Probability of winning:

p=\frac{3}{4}

5 games played.

Find probability of exactly 3 wins.

Calculation:

C(5,3)\left(\frac{3}{4}\right)^3\left(\frac{1}{4}\right)^2

Result:

\frac{135}{512}\approx0.264

---

## Example — Salesperson

Probability of sale:

p=\frac{1}{2}

12 customers approached.

Find probability of exactly 8 sales.

Calculation:

C(12,8)\left(\frac{1}{2}\right)^8\left(\frac{1}{2}\right)^4

Result:

\frac{495}{4096}\approx0.121
