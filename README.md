Download link :https://programming.engineering/product/homework-3-electronic/

# Homework-3-Electronic
Homework 3 Electronic
Nash Equilibria

Compute all (mixed and pure) Nash equilibria for each of the following normal-form games:

Sample Answer:

(T,L),(T,R),((1/3,2/3),(3/4,1/4))

Especially, if no mixed equilibria, write as:

(T,L),(T,R)

If one player is indi erent for any mixed strategy, write as:

((any),(P,1-P))

Strategies

Consider the following game in matrix form with two players. Payo s for the row player Izzy are indicated rst in each cell, and payo s for the column player Jack are second.

X

Y

Z

S

5,

2

10, 6

25,

10

T

10,

12

5, 6

0,

0

This game has two pure strategy Nash equilibria. What are they (justify your answer)? Of the two pure equilibria, which would Izzy prefer? Which would Jack prefer?

Sample Answer: (S,X),(S,Y) Izzy(S,X) Jack(S,Y)

VE 492 : Electronic #3 (Due June 10rd, 2020 at 11:59pm)

Suppose Izzy plays a strictly mixed strategy, where both S and T are chosen with positive probability. With what probability should Izzy choose S and T so that each of Jack’s three pure strategies is a best response to Izzy’s mixed strategy.

Sample Answer: (1/2,1/2)

Note that the former is the probability of S and the latter is the probability of T .

Suppose Jack wants to play a mixed strategy in which he selects X with probability 0.7. With what probability should Jack plays actions Y and Z so both of Izzy’s pure strategies is a best response to Jack’s mixed strategy?

Sample Answer: (1/4,3/4)

Note that the former is the probability of Y and the latter is the probability of Z.

Based on your responses above, describe a mixed strategy equilibrium for this game in which both Jack and Izzy play each of their actions (pure strategies) with positive probability (you can rely on the quantities computed in the prior parts of this question).

Sample Answer: ((1/4,3/4),(7/10,3/20,3/20))

Note that the rst tuple is the strategy of Izzy and the second one is the strategy of Jack.

If we swap two of Izzy’s payo s in this matrixin other words, if we replace one of his payo s r in the matrix with another of his payo s t from the matrix, and replace t with r, we can make one of his strategies dominant. What swap should we make, which strategy becomes dominant?

Sample Answer: (S,X),(S,Y),S

Note: The two tuples are strategies of which you want to exchange Izzy’s payo s. And please write in dictionary order, e.g. (S; Y ) before (T; X). The S is the dominant strategy after the payo exchange.

Solving MDPs

Consider the gridworld MDP for which Left and Right actions are 100% successful.

Speci cally, the available actions in each state are to move to the neighboring grid squares. From state a, there is also an exit action available, which results in going to the terminal state and collecting a reward of 10. Similarly, in state e, the reward for the exit action is 1. Exit actions are successful 100% of the time.


Let the discount factor = 1. Write the following quantities in one line.

V0(d); V1(d); V2(d); V3(d); V4(d); V5(d)

Sample Answer:

0,0,0,0,1,10

VE 492 : Electronic #3 (Due June 10rd, 2020 at 11:59pm)

Value Iteration Convergence Values

Consider the gridworld where Left and Right actions are successful 100% of the time.

Speci cally, the available actions in each state are to move to the neighboring grid squares. From state a, there is also an exit action available, which results in going to the terminal state and collecting a reward of 10. Similarly, in state e, the reward for the exit action is 1. Exit actions are successful 100% of the time.


Let the discount factor =0.2. Fill in the following quantities.

V (a) = V1(a) =

V (b) = V1(b) =

V (c) = V1(c) =

V (d) = V1(d) =

V (e) = V1(e) =

Write the following quantities in one line.

Sample Answer:

0,0,0,0,1

Value Iteration Properties

Which of the following are true about value iteration? We assume the MDP has a nite number of actions and states, and that the discount factor satis es 0 < < 1.

Value iteration is guaranteed to converge.

Value iteration will converge to the same vector of values (V ) no matter what values we use to initialize V .

None of the above.

VE 492 : Electronic #3 (Due June 10rd, 2020 at 11:59pm)

Policy Iteration

Consider the gridworld where Left and Right actions are successful 100% of the time.

Speci cally, the available actions in each state are to move to the neighboring grid squares. From state a, there is also an exit action available, which results in going to the terminal state and collecting a reward of 10. Similarly, in state e, the reward for the exit action is 1. Exit actions are successful 100% of the time.

The discount factor ( ) is 1.


Consider the policy 1 shown below, and evaluate the following quantities for this policy. Write your answers in one line.


( 1)(a) = V ( 1)(b) = V ( 1)(c) =

( 1)(d) = V ( 1)(e) =

Sample Answer:

0,0,0,0,1

VE 492 : Electronic #3 (Due June 10rd, 2020 at 11:59pm)

Policy Iteration

Consider the gridworld where Left and Right actions are successful 100% of the time.

Speci cally, the available actions in each state are to move to the neighboring grid squares. From state a, there is also an exit action available, which results in going to the terminal state and collecting a reward of 10. Similarly, in state e, the reward for the exit action is 1. Exit actions are successful 100% of the time.

The discount factor ( ) is 0.9.


Policy Iteration

Consider the policy i shown below, and evaluate the following quantities for this policy. Write your answers in one line.


( i)(a) = V ( i)(b) = V ( i)(c) =

( i)(d) = V ( i)(e) =

Sample Answer:

0,0,0,0,1

VE 492 : Electronic #3 (Due June 10rd, 2020 at 11:59pm)

Policy Improvement

Perform a policy improvement step. The current policy’s values are the ones from Part 1 (so make sure you rst correctly answer Part 1 before moving on to Part 2). Write your answers in one line.

(i). (i+1)(a) =

Exit

Right

(ii). (i+1)(b) =

Left

Right

(iii). (i+1)(c) =

Left

Right

(iv). (i+1)(d) =

Left

Right

(v). (i+1)(e) =

Left

Exit

Sample Answer:

A,A,A,A,B

Wrong Discount Factor

Bob notices value iteration converges more quickly with smaller and rather than using the true discount factor , he decides to use a discount factor of with 0 < < 1 when running value iteration. Write the options that are guaranteed to be true:

A. While Bob will not nd the optimal value function, he could simply rescale the values he nds

by

1

to nd the optimal value function.

1

If the MDP’s transition model is deterministic and the MDP has zero rewards everywhere, except for a single transition at the goal with a positive reward, then Bob will still nd the optimal policy.

If the MDP’s transition model is deterministic, then Bob will still nd the optimal policy.

Bob’s policy will tend to more heavily favor short-term rewards over long-term rewards compared to the optimal policy.

None of the above.

VE 492 : Electronic #3 (Due June 10rd, 2020 at 11:59pm)

MDP Properties

Which of the following statements are true for an MDP?

If the only di erence between two MDPs is the value of the discount factor then they must have the same optimal policy.

For an in nite horizon MDP with a nite number of states and actions and with a discount factor that satis es 0 < < 1, value iteration is guaranteed to converge.

When running value iteration, if the policy (the greedy policy with respect to the values) has converged, the values must have converged as well.

None of the above.

Which of the following statements are true for an MDP?

If one is using value iteration and the values have converged, the policy must have converged as well.

Expectimax will generally run in the same amount of time as value iteration on a given MDP.

For an in nite horizon MDP with a nite number of states and actions and with a discount factor that satis es 0 < < 1, policy iteration is guaranteed to converge.

None of the above.

10 Policies

John, James, Alvin and Michael all get to act in an MDP (S; A; T; ; R; s0).

John runs value iteration until he nds V which satis es

X

8s 2 S : V (s) = max T (s; a; s0)[R(s; a; s0) + V (s0)]


