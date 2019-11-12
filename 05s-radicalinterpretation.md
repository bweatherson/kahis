## The Radical Interpreter {#radicalinterpretation}

Many philosophical problems can be usefully thought of as games, and hence studied using game theoretic techniques. This is especially when the problems involve interactions of rational agents. Here, for example, is the game table for Newcomb's problem, with the human who is usually the focus of the problem as Row, and the demon as Column.[^GameExplain]

                    Predict 1 Box   Predict 2 Boxes
  ---------------- --------------- -----------------
      Choose 1 Box     1000, 1            0,0
    Choose 2 Boxes     1001, 0           1, 1

This game has a unique Nash equilbrium; the bottom right corner.[^NashDefn] And that's one way of motivating the view that (a) the game is possible, and (b) the rational move for the human is to choose two boxes.

Let's look at a more complicated game. I'll call it The Interpretation Game. The game has two players. Just like in Newcomb's problem, one of them is a human, the other is a philosophical invention. But in this case the invention is not a demon, but The Radical Interpreter. To know the payouts for the players, we need to know their value function. More colloquially, we need to know their goals.

-   The Radical Interpreter assigns mental states to Human in such a way as to predict Human's actions given Human rationality. We'll assume here that evidence is a mental state, so saying what evidence Human has is among Radical Interpreter's tasks. (Indeed, in the game play to come, it will be their primary task.)
-   Human acts so as to maximise the expected utility of their action, conditional on the evidence that they have. Human doesn't always know what evidence they have; it depends on what The Radical Interpreter says.

The result is that the game is a coordination game. The Radical Interpreter wants to assign evidence in a way that predicts rational Human action, and Human wants to do what's rational given that assignment of evidence. Coordination games typically have multiple equilibria, and this one is no exception.

Let's make all that (marginally) more concrete. Human is offered a bet on *p*. If the bet wins, it wins 1 util; if the bet loses, it loses 100 utils. Human's only choice is to Take or Decline the bet. The proposition *p*, the subject of the bet, is like the claim that Rahul is in the restaurant. It is something that is arguably part of Human's evidence. Unfortunately, it is also arguable that it is not part of Human's evidence. We will let $K$ be the rest of Human's evidence (apart from $p$, and things entailed by $K \cup p$), and stipulate that $\Pr(p | K) = 0.9$. Each party now faces a choice.

-   The Radical Interpreter has to choose whether *p* is part of Human's evidence or not.
-   Human has to decide whether to Take or Decline the bet.

The Radical Interpreter achieves their goal if human takes the bet iff *p* is part of their evidence. If *p* is part of the evidence, then The Radical Interpreter thinks that the bet has positive expected utility, so Human will take it. And if *p* is not part of the evidence, then The Radical Interpreter thinks that the bet has negative expected utility, so Human will decline it. Either way, The Radical Interpreter wants Human's action to coordinate with theirs. And Human wants to maximise expected utility. So we get the following table for the game.

                     $p \in E$   $p \notin E$
  ----------------- ----------- --------------
       Take the bet    1, 1        -9.1, 0
    Decline the bet    0, 0          0, 1

We have, in effect, already covered The Radical Interpreter's payouts. They win in the top-left and lower-right quadrants, and lose otherwise. Human's payouts are only a little trickier. In the bottom row, they are guaranteed 0, since the bet is declined. In the top-left, the bet is a sure winner; their evidence entails it wins. So they get a payout of 1. In the top-right, the bet wins with probability 0.9, so the expected return of taking it is $1 \times 0.9 - 100 \times 0.1 = -9.1$.

There are two Nash equilibria for the game - I've bolded them below.

                     $p \in E$   $p \notin E$
  ----------------- ----------- --------------
       Take the bet  **1, 1**      -9.1, 0
    Decline the bet    0, 0        **0, 1**

That there are two equilibria to this game should not come as a surprise. It's a formal parallel to the fact that the pragmatic encroachment theory I've developed so far doesn't make a firm prediction about this game. It is consistent with the theory developed so far that Human's evidence includes $p$, and they should take the bet, or that due to interest-sensitive features of the case, it does not include $p$, and they should not take the bet. The aim of this chapter is to supplement that theory with one that, at least most of the time, makes a firm pronouncement about what the evidence is.

But to do that, I need to delve into somewhat more contested areas of game theory. In particular, I need to introduce some work on equilibrium choice. And to do this, it helps to think about a game that is inspired by an example of Rousseau's.

[^GameExplain]: In these games, Row chooses a row, and Column chooses a column, and that determines the cell that is the outcome of the game. The cells include two numbers. The first is Row's payout, and the second is Column's. The games are non-competitive; the players are simply trying to maximise their own returns, not maximise the difference between their return and the other player's return.
    
    The idea of treating Newcomb's Problem, and similar decision-theoretic problems, as games traces back to @Harper1986.

[^NashDefn]: A Nash equilibrium is an outcome of the game where every player does as well as they can given the moves of the other players. Equivalently, it is an outcome where no player can improve their payout by unilaterally defecting from the equilibrium.
