### Updates and Modals {#modalupdate}

The version of IRT that I defend here gives a big role to conditional attitudes.^[This section is based on material from my -@Weatherson2016[sect. 1].] That's something that it has in common with everything I've written about IRT. But I used to have a particular pair of views about how to understand conditional attitudes. In particular, I took the following two claims to be at least close approximations to the truth about conditional attitudes.

1. An attitude conditional on $p$ is (usually) the same as the attitude one would have after updating on $p$.
2. The way to update on $p$ is to conditionalise.

The first is at best an approximation for familiar reasons. I can think that no one knows whether $p$ is true, and even think that this is true conditional on $p$. But after updating on $p$, I will no longer think that. So we have to be a bit careful in applying principle 1; it has counterexamples. But it is still a useful heuristic, and that's how I'll use it.

What wasn't originally obvious to me was that there are counterexamples to principle 2 as well. And they are more significant for the way IRT should be understood. I used to describe the picture of belief I was defending as the view that to believe something is to have a credence in it that's close enough to 1 for current purposes. That's still a decent heuristic, but it isn't always right. When someone is interested in modal questions, credence 1 might be insufficient for belief. To see how this might be so, it helps to start with some points Thony @Gillies2010 makes about the relationship between modals, conditionals and updating. 

When modal questions are on the table, updating will not be the same as conditionalising. This is shown by the following example. (A similar example is in @Kratzer2012 [94].)

> I have lost my marbles. I know that just one of them -- Red or Yellow -- is in the box. But I don't know which. I find myself saying things like ..."If Yellow isn't in the box, the Red must be." (4:13)

What matters for the purposes of this book is not whether this conditional is true, but whether its truth is consistent with the Ramsey test view of conditionals. And Gillies argues that it is.

> The Ramsey test -- the schoolyard version, anyway -- is a test for when an indicative conditional is acceptable given your beliefs. It says that (if *p*)(*q*) is acceptable in belief state *B* iff *q* is acceptable in the derived or subordinate state *B*-plus-the-information-that-*p*. (4:27)

And he notes that this can explain what goes on with the marbles conditional. Add the information that Yellow isn't in the box, and it isn't just true, but must be true, that Red is in the box.

Note though that while we can explain this conditional using the Ramsey test, we can't explain it using any version of the idea that probabilities of conditionals are conditional probabilities. The probability that Red must be in the box is 0. The probability that Yellow isn't in the box is not 0. So conditional on Yellow not being in the box, the probability that Red must be in the box is still 0. Yet the conditional is perfectly assertable.

There is, and this is Gillies's key point, something about the behaviour of modals in the consequents of conditionals that we can't capture using conditional probabilities, or indeed many other standard tools. And what goes for consequents of conditionals goes for updated beliefs too. Learn that Yellow isn't in the box, and you'll conclude that Red must be. But that learning can't go via conditionalisation; just conditionalise on the new information and the probability that Red must be in the box goes from 0 to 0.

Now it's a hard problem to say exactly how this alternative to updating by conditionalisation should work. But very roughly, the idea is that at least some of the time, we update by eliminating worlds from the space of possibilities. This affects dramatically the probability of propositions whose truth is sensitive to which worlds are in the space of possibiilties.

And this matters when we are considering modal questions. For example, if we are considering the question _Must q be true?_, then it is plausible that unconditionally the answer is no, and indeed the unconditional probability that $q$ must be true is 0, but that conditional on $p$, $q$ must be true.

We don't even have to be considering modals directly for this to happen. Assume that actions $A$ and $B$ have the same outcome conditional on $q$, but $A$ is better than $B$ in every $\neg q$ possibility. Then if we are considering the question _Is A better than B?_, it will matter whether it must be the case that $q$.

Assume that $q$ could have probability 1 without it being the case that $q$ must be true. (This is controversial, but I'll offer arguments in sections \@ref(lockecoin) and \@ref(lockegames) that it is possible.) Then unconditionally, $A$ is better than $B$, even though they have the same expected utility. That's because weak dominance is a good principle of practical reasoning: If $A$ might be better than $B$ and must not be worse, then $A$ is better than $B$. But by hypothesis, conditional on $p$, $A$ is not better than $B$. So in this case $p$ will not be believed; conditional on $p$ the question _Is A better than B_ gets a different answer to what it gets unconditionally.

Note though that all I said to get this example going is that $p$ rules out $\neg q$, and $q$ has probability 1. That means $p$ could have any probability at all, up to probability 1. So it's possible that conditional on $p$, some relevant questions get different answers to what they get unconditionally, even though $p$ has probability 1. So belief can't be a matter of having probability close enough to 1 for practical purposes; sometimes even probability 1 is insufficient.
