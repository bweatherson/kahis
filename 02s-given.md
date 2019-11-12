## Taking As Given {#given}

To start towards a positive theory of belief, it helps to think about the following example, featuring a guy I'll call Sully. (This example is going to resemble the examples involving Renzo in @RossSchroeder2014, and at least for a while, my conclusions are going to resemble theirs as well.) Sully is a fan of the Boston Red Sox, and one of the happiest days of his life was when the Red Sox broke their 86 year long curse, and won baseball's World Series in 2004. He knows, and hence believes, that the Red Sox won the World Series in 2004. He likes their chances to win again this year, because in Sully's heart, hope always springs eternal. 

It's now the start of a new baseball season, and Sully is offered, for free, a choice between the following two bets.

* Bet A wins $50 if the Red Sox win the World Series this year, and nothing otherwise.
* Bet B wins $60 if the same team wins the World Series this year as won in 2004, and nothing otherwise.

For Sully, this choice is a no-brainer. If the Red Sox win this year, he wins more money taking B than A. If the Red Sox don't win this year, he gets nothing either way. So it's better to take B than A, and that's what he does.

What Sully has done here is use dominance reasoning, in particular weak dominance reasoning. One option weakly dominates another if it might have a better return, and can't have a worse return. Weak dominance is used as an analytical tool in game theory. But it is also a form of inference that non-theorists, like Sully can use. (Though unless they've taken a game theory course they might not use this phrase to describe it.) 

Sully's case can be distinguished from that of his more anxious friend Mack. Mack is also a big Red Sox fan, and also looks back on that curse-busting World Series win with fondness. But if you offer Mack the choice between these two bets, he'll hesitate a bit. He'll wonder if he's really sure it was 2004 that the Red Sox won. Maybe it was 2005 he thinks. He'll eventually think that even if he's not completely sure that it was 2004, it was very likely 2004, and so it is very likely that bet B will do better, and that's what he will take.

Even if Sully and Mack end up at the same point, they have used very different forms of reasoning. Sully uses weak dominance reasoning, while Mack uses probabilistic reasoning. Sully takes the fact that the Red Sox won in 2004 as given, while Mack just takes it to be very likely. The big thing I want to rely on here is that these are very different psychological processes. Neither of these guys is doing something that approximates, or simplifies, the other; they both take bet B, but they get to that conclusion via very different routes.

There is a theoretical analog to this psychological point. Most game theorists think that weak dominance reasoning can be iterated more or less indefinitely. (Though there are some notable exceptions.) But few think that likelihood reasoning can be iterated indefinitely. This reflects the fact that they are very different kinds of reasoning. Dominance reasoning is pre-probabilistic.

Sully's reasoning isn't just dominance reasoning. It's dominance reasoning that relies on some very specific assumptions. When Sully reasons that A can't do better than B, he's not drawing any kind of logical or metaphysical point. It's logically and metaphysically possible that the Red Sox lost in 2004. For that matter, and this is a point @Ganson2019 stresses, it's logically and metaphysically possible that the payouts for A and B are other than what Sully thinks they are.

And thought he might not make it explicit, at some level Sully surely knows this. If pushed, he'd endorse the conditional "If I've misremembered when the curse-busting World Series win was, and the Red Sox didn't win in 2004, then bet A might do better than bet B". So while he is disposed to use dominance reasoning in deciding whether to take A or B, this disposition rests on taking some facts about the world for granted.

Recall the disjunctive way that Sully reasoned. Either the Red Sox will win this year or they won't. Either way, I won't do better taking bet A, but I might do better taking bet B. So I'll take bet B. This reasoning - not just the reasons Sully has but his reasoning - can be appropriately represented by the kind of decision table that is familiar from decision theory or game theory.

----------- ------------- -------------------
             Red Sox Win   Red Sox Don't Win
 Take Bet A      $50            $0
 Take Bet B      $60            $0
----------- ------------- -------------------

Focus for now on the columns in this table. Sully takes two possibilities seriously: that the Red Sox win this year, and that they don't. The 'possibilities' here are possibilities in the sense of @Humberstone1981. They have content - in one of them the Red Sox win, in the other they don't, but they don't settle all facts. In the right-hand column, there is no fact of the matter about which team wins the World Series. In neither column is there a fact of the matter about what Sully will have for lunch tomorrow. If you want to think of these in terms of worlds, they are both very large sets of worlds, and within those sets there is a lot of variability.^[Analysing these possibilities as sets of worlds is unhelpful when we want to use a model like this to represent modal or logical uncertainty. But it's a helpful heuristic in most cases. And there isn't anything wrong with using a model that breaks down when applied outside its appropriate zone.]

But there is more to the content of each column than what is explicity represented in the header row. In each column, for example, the Red Sox won in 2004. That's why Sully can put those monetary payoffs into the cells. And in each column, the terms of the bet are as Sully knows that they are. In sets of worlds terms, the sets that are represented by the columns are exclusive, but far from exhaustive.

Consider those propositions which are true according to all of the columns in this table. Say a proposition is *taken as given* in a decision problem when it the decider treats one option as dominating another, and does so in virtue of a table in which that proposition is true in every column. Then here is one principle about belief that seems to be very plausible.

Given
:    S believes that $p$ only if there is some possible decision problem such that S is disposed to take $p$ as given when faced with that problen.

**Given** is logically weak in one respect, and strong in another. It only requires that S be willing to take $p$ for granted in one possible choice. It doesn't have to be a likely, or even particularly realistic choice. Sully is unlikely to have strangers offer him these free money bets. But given how representationally sparse decision tables are, for something to be true in all columns of a decision table is a very strong claim. It doesn't suffice, for instance, for $p$ to be true in some columns and false in none. Each column has to take a stance on $p$, and endorse it.

But **Given** cannot be converted to a biconditional. Being disposed to sometimes take $p$ as given is not sufficient for belief. If Anisa had played the Red-Green game rationally, she would have lost any belief about when the Battle of Hastings was. To explain cases like that, we need to expand our theory of belief.
