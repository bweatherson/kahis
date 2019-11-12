## Motivating Risk-Dominant Equilibria {#globalgame}

At an almost maximal level of abstraction, a two player, two option each game looks like this.

  ----- -------------------- --------------------
                $a$                  $b$
    $A$  $r_{11}$, $c_{11}$   $r_{12}$, $c_{12}$
    $B$  $r_{21}$, $c_{21}$   $r_{22}$, $c_{22}$
  ----- -------------------- --------------------

We're going to focus on games that have the following eight properties:

-   $r_{11} > r_{21}$
-   $r_{22} > r_{12}$
-   $c_{11} > c_{12}$
-   $c_{22} > c_{21}$
-   $r_{11} > r_{22}$
-   $c_{11} \geq c_{22}$
-   $\frac{r_{21}+r_{22}}{2} > \frac{r_{11}+r_{12}}{2}$
-   $\frac{c_{12}+c_{22}}{2} \geq \frac{c_{11}+c_{21}}{2}$

The first four clauses say that the game has two (strict) Nash equilibria: $Aa$ and $Bb$. The fifth and sixth clauses say that the $Aa$ equilibria is **Pareto-optimal**: no one prefers the other equilibria to it. In fact it says something a bit stronger: one of the players strictly prefers the $Aa$ equilibria, and the other player does not prefer $Bb$. The seventh and eighth clauses say that the $Bb$ equilibria is **risk-optimal**.

I'm going to offer an argument from Hans Carlsson and Eric van Damme [-@CarlssonVanDamme1993] for the idea that in these games, rational players will end up at $Bb$. The game that Human and The Radical Interpreter are playing fits these eight conditions, and The Radical Interpreter is perfectly rational, so this will imply that in that game, The Radical Interpreter will say that $p \notin E$, which is what we aimed to show.

Games satisfying these eight inequalities are sometimes called *Stag Hunt* games. There is some flexibility, and some vagueness, in which of the eight inequalities need to be strict, but that level of detail isn't important here. The name comes from a thought experiment in Rousseau's *Discourse on Inequality*.

> They were perfect strangers to foresight, and were so far from troubling themselves about the distant future, that they hardly thought of the morrow. If a deer was to be taken, every one saw that, in order to succeed, he must abide faithfully by his post: but if a hare happened to come within the reach of any one of them, it is not to be doubted that he pursued it without scruple, and, having seized his prey, cared very little, if by so doing he caused his companions to miss theirs.  [@Rousseau1913 209--10]

It is rather interesting to think through which real-life situations are best modeled as Stag Hunts, especially in situations where people have thought that the right model was a version of Prisoners' Dilemma. This kind of thought is one way in to appreciating the virtues of Rousseau's political outlook, and especially the idea that social coordination might not require anything like the heavy regulatory presence that, say, Hobbes thought was needed. But that's a story for another day. What I'm going to focus on is why Rousseau was right to think that a 'stranger to foresight', who is just focussing on this game, should take the rabbit.

To make matters a little easier, we'll focus on a very particular instance of Stag Hunt, as shown here. (From here I'm following Carlsson and van Damme very closely; this is their example, with just the labelling slightly altered.)

  ----- ------ ------
         $a$    $b$
    $A$  4, 4   0, 3
    $B$  3, 0   3, 3
  ----- ------ ------

At first glance it might seem like $Aa$ is the right choice; it produces the best outcome. This isn't like Prisoners Dilemma, where the best collective outcome is dominated. In fact $Aa$ is the best outcome for each individual. But it is risky, and Carlsson and van Damme show how to turn that risk into an argument for choosing $Bb$.

Embed this game in what they call a *global game*. We'll start the game with each player knowing just that they will play a game with the following payout table, with $x$ to be selected at random from a flat distribution over $[-1, 5]$.

  ----- -------- ----------
         $a$      $b$
    $A$    4, 4   0, $x$
    $B$  $x$, 0   $x$, $x$
  ----- -------- ----------

Before they play the game, each player will get a noisy signal about the value of $x$. There will be signals $s_R$ and $s_C$ chosen (independently) from a flat distribution over $[x - 0.25, x + 0.25]$, and shown to Row and Column respectively. So each player will know the value of $x$ to within $\frac{1}{4}$, and know that the other player knows it to within $\frac{1}{4}$ as well. But this is a margin of error model, and in those models there is very little that is common knowledge. That, they argue, makes a huge difference.

In particular, they prove that iterated deletion of strictly dominated strategies (almost) removes all but one strategy pair. (I'll go over the proof of this in the next subsection.) Each player will play $A$/$a$ if the signal is greater than 2, and $B$/$b$ otherwise.^[Strictly speaking, we can't rule out various mixed strategies when the signal is precisely 2, but this makes little difference, since that occurs with probability 0.] Surprisingly, this shows that players should play the risk-optimal strategy even when they know the other strategy is Pareto-optimal. When a player gets a signal in $(2, 3.75)$, then they know that $x < 4$, so $Bb$ is the Pareto-optimal equilibrium. But the logic of the global game suggests the risk-dominant equilibrium is what to play.

Carlsson and van Damme go on to show that many of the details of this case don't matter. As long as (a) there is a margin of error in each side's estimation of the payoffs, and (b) every choice is a dominant option in some version of the global game, then iterated deletion of strongly dominant strategies will lead to each player making the risk-dominant choice.

I conclude from that that risk-dominant choices are rational in these games. There is a limit assumption involved here; what's true for games with arbitrarily small margins of error is true for games with no margin of error. (We'll come back to that assumption below.) And since The Radical Interpreter is rational, they will play the strategy that is not eliminated by deleting dominant strategies. That is, they will play the risk-dominant strategy.

In game with Human, the rational (i.e., risk-dominant) strategy for The Radical Interpreter is to say that $p \notin E$. And in the case of Parveen and Rahul, rational (i.e., risk-dominant) strategy for The Radical Interpreter is to say that it is not part of Parveen's evidence that Rahul is in the restaurant. And this is an interest-relative theory of evidence; had Parveen been playing a different game, The Radical Interpreter would have said that it is part of Parveen's evidence that Rahul was in the restaurant.

And from this point all the intuitions about the case fall into place. If it is part of Parveen's evidence that Rahul is in the restaurant, then she knows this. Conversely, if she knows it, then The Radical Interpreter would have said it is part of her evidence, so it is part of her evidence. Parveen will perform the action that maximises expected utility given her evidence. And she will lose knowledge when that disposition makes her do things that would be known to be sub-optimal if she didn't lose knowledge.

In short, this model keeps what was good about the pragmatic encroachment theory developed in the previous chapters, while also allowing that evidence can be interest-relative. It does require a slightly more complex theory of rationality than was previously used. Rather than just model rational agents as utility maximisers, they are modelled as playing playing risk-dominant strategies in coordination games. But it turns out that this is little more than assuming that they maximise evidential expected utility, and they expect others (at least perfectly rational abstract others) to do the same, and they expect those others to expect they will maximise expected utility, and so on.

The rest of this section goes into more technical detail about Carlsson and van Damme's example. Readers not interested in these details can skip ahead to the next section. In the first subsection I summarise their argument that we only need iterated deletion of strictly dominated strategies to get the result that rational players will play the risk-dominant strategies. In the second subsection I offer a small generalisation of their argument, showing that it still goes through when one of the players gets a precise signal, and the other gets a noisy signal. And I discuss why that is relevant. (In short, the Radical Interpreter doesn't have to deal with noise, and we want the argument to respect that fact.)

### The Dominance Argument for Risk-Dominant Equilibria {#cvdproof}

Two players, Row (or R) and Column (or C) will play a version of the following game.

  ----- -------- ----------
         $a$      $b$
    $A$  4, 4     0, $x$
    $B$  $x$, 0   $x$, $x$
  ----- -------- ----------

They won't be told what $x$ is, but they will get a noisy signal of $x$, drawn from an even distribution over $[x - 0.25, x + 0.25]$. Call these signals $s_R$ and $s_C$. Each player must then choose $A$, getting either 4 or 0 depending on the other player's choice, or choose $B$, getting $x$ for sure.

Before getting the signal, the players must choose a strategy. A strategy is a function from signals to choices. Since the higher the signal is, the better it is to play $B$, we can equate strategies with 'tipping points', where the player plays $B$ if the signal is above the tipping point, and $A$ below the tipping point. Strictly speaking, a tipping point will pick out not a strategy but an equivalence class of strategies, which differ in how they act if the signal is the tipping point. But since that happens with probability 0, the strategies in the equivalence class have the same expected return, and so I won't distinguish them.

Also, strictly speaking, there are strategies that are not tipping points, because they map signals onto probabilities of playing $A$, where the probability decreases as $A$ rises. I won't discuss these directly, but it isn't too hard to see how these are shown to be suboptimal using the argument that is about to come. It eases exposition to focus on the pure strategies, and to equate these with tipping points. And since my primary aim here is to explain why the result holds, not to simply repeat an already existing proof, I'll mostly ignore these mixed strategies.

Call the tipping points for Row and Column respectively $T_R$ and $T_C$. Since the game is symmetric, we'll just have to show that in conditions of common knowledge of rationality, $T_R = 2$. It follows by symmetry that $T_C = 2$ as well. And the only rule that will be used is iterated deletion of strictly dominated strategies. That is, neither player will play a strategy where another strategy does better no matter what the opponent chooses, and they won't play strategies where another strategy does better provided the other player does not play a dominated strategy, and they won't play strategies where another strategy does better provided the other player does not play a strategy ruled out by these first two conditions, and so on.

The return to a strategy is uncertain, even given the other player's strategy. But given the strategies of each player, each players' expected return can be computed. And that will be treated as the return to the strategy pair. 

Note first that $T_R = 4.25$ strictly dominates any strategy where $T_R  = y > 4.25$. If $s_R \in (4.25, y)$, then $T_R$ is guaranteed to return above 4, and the alternative strategy is guaranteed to return 4. In all other cases, the strategies have the same return. And there is some chance that $s_R \in (4.25, y)$. So we can delete all strategies $T_R  = y > 4.25$, and similarly all strategies $T_C = y > 4.25$. By similar reasoning, we can rule out $T_R < -0.25$ and $T_C < -0.25$.

If $s_R \in [-0.75, 4.75]$, then it is equally likely that $x$ is above $s_R$ as it is below it. Indeed, the posterior distribution of $x$ is flat over $[s_R - 0.25, s_R + 0.25]$. From this it follows that the expected return of playing $B$ after seeing signal $s_R$ is just $s_R$.

Now comes the important step. Assume that we know that $T_C \leq y > 2$. Now consider the expected return of playing $A$ given various values for $s_R > 2$. Given that the lower $T_C$ is, the higher the expected return is of playing $A$, we'll just work on the simple case where $T_C = y$, realizing that this is an upper bound on the expected return of $A$ given $T_C \leq y$. The expected return of $A$ is 4 times the probability that Column will play $a$, i.e., 4 times the probability that $s_C < T_C$. Given all the symmetries that have been built into the puzzle, we know that the probability that $s_C < s_R$ is 0.5. So the expected return of playing $A$ is at most 2 if $s_R \geq y$. But the expected return of playing $B$ is, as we showed in the last paragraph, $s_R$, which is greater than 2. So it is better to play $B$ than $A$ if $s_R \geq y$. And the difference is substantial, so even if $s_R$ is epsilon less than that $y$, it will still be better to play $B$. (This is rather hand-wavy, but I'll go over the more rigorous version presently.)

So if $T_C \leq y > 2$ we can prove that $T_R$ should be lower still, because given that assumption it is better to play $B$ even if the signal is just less than $y$. Repeating this reasoning over and over again pushes us to it being better to play $B$ than $A$ as long as $s_R > 2$. And the same kind of reasoning from the opposite end pushes us to it being better to play $A$ than $B$ as long as $s_R < 2$. So we get $s_R = 2$ as the uniquely rational solution to the game.

Let's make that a touch more rigorous. Assume that $T_C = y$, and $s_r$ is slightly less than $y$. In particular, we'll assume that $z = y - s_R$ is in $(0, 0.5)$. Then the probability that $s_C < y$ is $0.5 + 2z - 2z^2$. So the expected return of playing $A$ is $2 + 8z - 8z^2$. And the expected return of playing $B$ is, again, $s_R$. These will be equal when the following is true. (The working out is a tedious but trivial application of the quadratic formula, plus some rearranging.)

$$s_R = y + \frac{\sqrt{145-32y} - 9}{16}$$ 

So if we know that $T_C \geq y$, we know that $T_R \geq y + \frac{\sqrt{145-32y} - 9}{16}$, which will be less than $y$ if $y > 2$. And then by symmetry, we know that $T_C$ must be at most as large as that as well. And then we can use that fact to derive a further upper bound on $T_R$ and hence on $T_C$, and so on. And this will continue until we push both down to 2. It does require quite a number of steps of iterated deletion. Here is the upper bound on the threshold after $n$ rounds of deletion of dominated strategies. (These numbers are precise for the first two rounds, then just to three significant figures after that.)

   Round   Upper Bound on Threshold
  ------- --------------------------
     1              4.250
     2              3.875
     3              3.599
     4              3.378
     5              3.195
     6              3.041
     7              2.910
     8              2.798
     9              2.701
    10              2.617

That is, $T_R = 4.25$ dominates any strategy with a tipping point above 4.25. And $T_R = 3.875$ dominates any strategy with a higher tipping point than that, assuming $T_C \leq 4.25$. And $T_R \approx 3.599$ dominates any strategy with a higher tipping point than that, assuming $T_C \leq 3.875$. And so on.

And similar reasoning shows that at each stage not only are all strategies with higher tipping points dominated, but so are strategies that assign positive probability (whether it is 1 or less than 1), to playing $A$ when the signal is above the 'tipping point'. So this kind of reasoning rules out all mixed strategies (except those that respond probabilistically to $s_R = 2$).

So it has been shown that iterated deletion of dominated strategies will rule out all strategies except the risk-optimal equilibrium. The possibility that $x$ is greater than the maximal return for $A$ is needed to get the iterated dominance going. And the signal to have an error bar to it, so that each round of iteration removes more strategies. But that's all that was needed; the particular values used  are irrelevant to the proof.

### Making One Signal Precise {#perfectri}

The aim of this sub-section is to prove something that Carllson and van Damme did not prove, namely that the analysis of the previous subsection goes through with very little change if one party gets a perfect signal, while the other gets a noisy signal. So I'm going to discuss the game that is just like the game of the previous subsection, but where it is common knowledge that the signal Column gets, $s_C$, equals $x$.

Since the game is no longer symmetric, I can't just appeal to the symmetry of the game as frequently as in the previous subsection. But this only slows the proof down, it doesn't stop it.

We can actually rule out slightly more at the first step in this game than in the previous game. Since Column could not be wrong about $x$, Column knows that if $s_C > 4$ then playing $b$ dominates playing $a$. So one round of deleting dominated strategies rules out $T_C > 4$, as well as ruling out $T_R > 4.25$.

At any stage, if we know $T_C \leq y > 2$, then $T_R = y$ dominates $T_R > y$. That's because if $s_R \geq y$, and $T_C \leq y$, then the probability that Column will play $a$ (given Row's signal) is less than 0.5. After all, the signal is just as likely to be above $x$ as below it (as long as the signal isn't too close to the extremes). So if $s_R$ is at or above $T_C$, then it is at least 0.5 likely that $s_C = x$ is at or above $T_C$. So the expected return of playing $A$ is at most 2. But the expected return of playing $B$ equals the signal, which is greater than 2. So if Row knows $T_C \leq y > 2$, Row also knows it is better to play $B$ if $s_R \geq y$. And that just means that $T_R \leq y$.

Assume now that it is common knowledge that $T_R \leq y$, for some $y > 2$. And assume that $x = s_C$ is just a little less than $y$. In particular, define $z = y -x$, and assume $z \in (0, 0.25)$. We want to work out the upper bound on the expected return to Column of playing $a$. (The return of playing $b$ is known, it is $x$.) The will be highest when $T_R$ is lowest, so assume $T_R \leq y$. Then the probability that Row plays $A$ is $(1 + 2z)/2$. So the expected return of playing $a$ is $2 + 4z$, i.e., $2 + 4(y - x)$. That will be greater than $x$ only when

$$x < \frac{2 + 4y}{5}$$ 

And so if it is common knowledge that $T_R \leq y$, then it is best for Column to play $b$ unless $x < \frac{2 + 4y}{5}$. That is, if it is common knowledge that $T_R \leq y$, then $T_C$ must be at most $\frac{2 + 4y}{5}$.

So now we proceed in a zig-zag fashion. At one stage, we show that $T_R$ must be as low as $T_C$. At the next, we show that if it has been proven that $T_R$ takes a particular value greater than 2, then $T_C$ must be lower still. And this process will eventually rule out all values for $T_R$ and $T_C$ greater than 2.

This case is crucial to the story of this chapter because The Radical Interpreter probably does not have an error bar in their estimation of the game they are playing. But it turns out the argument for risk-dominant equilibria being the unique solution to interpretation games is consistent with that. As long as one player has a margin of error, each player should play the risk-dominant equilibria.
