---
title: "Bayesian Networks"
published: true
morea_id: experience-04-bayesian-network
morea_type: experience
morea_summary: "Bayesian networks"
morea_sort_order: 31
morea_start_date: "2025-02-10T23:00"
morea_labels: "4 extra credits"
---

# Bayesian Networks

A Bayesian network is a probabilistic graphical model and has many applications. Here we study a simple Bayesian network.

A student has a class in the early morning. It is easy to be late to this class due to oversleeping or late bus. 

Suppose that the student may oversleep ($S$) with probability 0.5, and may encounter a late bus ($B$) with probability 0.5. The events $S$ and $B$ are *independent*.

- If the student overslept and the bus was late, the probability of being late to the class is $P(L \| S \cap B) = p_1$.
- If the student overslept and the bus was not late, the probability of being late to the class is $P(L \| S \cap B^c) = p_2$.
- If the student did not oversleep and the bus is late, the probability of being late to the class is $P(L \| S^c \cap B) = p_3$.
- If the student did not oversleep and the bus was not late, the probability of being late to the class is $P(L \| S^c \cap B^c) = p_4$.

Given that the student is late to the class, we can infer whether the student overslept or it was the late bus.

Questions:
- (1 point) Write down the expressions of the conditional probabilities $P(S \| L)$, $P(B \| L)$, and $P( S \cap B \| L)$.
- (1 point) Under what values of $p_1, p_2, p_3, p_4$ are the two events $S$ and $B$ conditionally independent given $L$?
- (1 point) In causal inference, we call it the "explaining away" effect if $P(S \| L) > P(S \| B \cap L)$. This means given that the student is late to the class, knowing that the bus was late reduces the likelihood that the student overslept. Under what values of $p_1, p_2, p_3, p_4$ we will have the "explaining away" effect?
- (1 point) On the contrary, the opposite of "explaining away" is "reinforcing", where $P(S \| L) < P(S \| B \cap L)$. Under what values of $p_1, p_2, p_3, p_4$ we will have the "reinforcing" effect?

Please send your solution to me via email. Good luck!
