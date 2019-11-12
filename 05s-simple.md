## A Simple, but Incomplete, Solution {#simplesolution}

Let's take a step back and look at the puzzle more abstractly. We have a person *S*, who has some option *O*, and it really matters whether or not the expected value of *O*, i.e., $V(O)$, is at least $x$. (I am assuming that Parveen is in the business of maximising expected utility here. In chapter \@(ties) I'll look cases where this is an unreasonable assumption. But it seems reasonable here, because it doesn't take much work to see that Red-True has very high utility.) It is uncontroversial that her evidence includes some background $K$, and controversial whether it includes some contested proposition $p$. It is also uncontroversial that $V(O | p) \geq x$, and we're assuming that for any proposition $q$ that is in her evidence, $V(O | q) = V(O)$. That is, we're assuming the relevant values are conditional on evidence. We can capture that last assumption with one big assumption that probably isn't true, but is a harmless idealisation for the purposes of this chapter. Say there is a prior value function $V^-$, with a similar metaphysical status to the mythical, mystical prior probability function. Then for any choice $C$, $V(C) = V^-(C | E)$, where $E$ is the evidence the agent has.

Now I can offer a simple, but incomplete, solution.  Let $p$ be the proposition that she might or might not know, and the question of whether $V(O) \geq x$ be the only salient one that $p$ is relevant to. Then she knows $p$ only if the following is true:

> $\frac{V^-(O | K) + V^-(O | K \wedge p)}{2} \geq x$

That is, we work out the value of $O$ with and without the evidence $p$, and if the average is greater than $x$, good enough!

That solves the problem of Parveen and Rahul. Parveen's evidence may or may not include that Rahul is in the restaurant. If it does, then Blue-True has a value of \$50. If it does not, then Blue-True's value is somewhat lower. Even if the evidence includes that someone who looks a lot like Rahul is in the restaurant, the value of Blue-True might only be \$45. Averaging them out, the value is less than \$50. But she'd only play Blue-True if it was worthwhile it play it instead of Red-True, which is worth \$50. So she shouldn't play Blue-True.

Great! Well, great except for two monumental problems. 

The first problem is that what I've said here really only helps with very simple cases, where there is a single decision problem that a single contested proposition is relevant to. There has to be some way to generalise the case to less constrained situations. 

The second (and bigger) problem is that the solution is completely ad hoc. Why should the arithmetic mean of these two things have any philosophical significance? Why not the mean of two other things? Why not some other function, like the geometric mean of them? This looks like a formula plucked out of the air, and there are literally infinitely many other formulae that would do just as well by the one criteria I've laid down so far: imply that Parveen must play red-true.

Pragmatic encroachment starts with a very elegant, very intuitive, principle: you only know the things you can reasonable take to be settled for the purposes of current deliberation. It does not look like any such elegant, intuitive, principles will lead to some theorem about averaging out the value of an option with and without new evidence.

Happily, the two problems have a common solution. But the solution requires a detour into some technical work concerning coordination games.
