## Evidence, Knowledge and Cut-Elimination {#cutelim}

In the previous section I noted that my theory of evidence is committed to denying Williamson's E=K thesis. This is the thesis that says one's evidence is all and only what one knows. What I say is consistent with, and arguably committed to, one half of that thesis. Nothing I've said here provides a reason to reject the implication that if $p$ is part of one's evidence, then one knows $p$. Indeed, the story I'm telling would have to be complicated even further if that fails. But I am committed to denying the other direction. On my view, there can be cases where someone knows $p$, but $p$ is not part of their evidence. 

My main reason for this comes from the kind of cases that Shyam @Nair2019 describes as failures of 'cut-elimination'. I'll quickly set out what Nair calls cut-elimination, and why it fails, and then look at how it raises problems for E=K.

Start by assuming that we have an operator $\vDash$ such that $\Gamma \vDash A$ means that $A$ can be rationally inferred from $\Gamma$. I'm following Nair (and many others) in using a symbol usually associated with logical entailment here, though this is potentially misleading. A big plotline in what follows will be that $\vDash$, so understood, behaves very differently from familiar logics.

For the purposes of this section, I'm staying somewhat neutral on what it means to be able to rationally infer $A$ from $\Gamma$. In particular, I want everything that follows to be consistent with the interpretation that an inference is rational only if it produces knowledge. I don't think that's true; I think folks with misleading evidence can rationally form false beliefs, and I think the traveller in Dharmottara's example rationally believes there is a fire. But there is a dialectical reason for staying neutral here. I'm arguing against one important part of the 'knowledge first' program, and I don't want to do so by assuming the falsity of other parts of it. So for this section (only), I'll write in a way that is consistent with saying rational belief requires knowledge.

So one way to interpret $\Gamma \vDash A$ is that $A$ can be known on the basis of $\Gamma$. What can be known on the basis of what is a function of, among other things, who is doing the knowing, what their background evidence is, what their capacities are, and so on. Strictly speaking, that suggests we should have some subscripts on $\vDash$ for who is the knower, what their background evidence is, and so on. In the interests of readability, I'm going to leave all those implicit. Though in the next section it will be important to come back and look at whether the force of some of these arguments is diminished if we are careful about this relativisation.

So that's our important notation. The principle **Cut** that Nair focusses on is that if 1 and 2 are true, so is 3.

1. $\Gamma \vDash A$
2. $\{A\} \cup \Delta \vDash B$
3. $\Gamma \cup \Delta \vDash B$

The principle is intuitive. Indeed, it is often implicit in a lot of reasoning. Here is one instance of it in action.

> I heard from a friend that Jack went up the hill. This friend is trustworthy, so I'm happy to infer that Jack did indeed go up the hill. I heard from another friend that Jack and Jill did the same thing. This friend is also trustworthy, so I'm happy to infer that Jill did the same thing as Jack, i.e., go up the hill.

Normally we wouldn't spell out the 'happy to infer' steps, but I've included them in here to make the reasoning a bit more explicit. But note that what I didn't need to make explicit, even in this laborious reconstruction. That Jack went up the hill goes from a conclusion of the first little argument, to a premise in a later argument. The later argument says that we can conclude from the fact that Jack went up the hill, and that a friend said Jack and Jill did the same thing, that Jill went up the hill. And what matters for our purposes is that there doesn't seem to be a gap between the rationality of inferring that Jack went up the hill, and the rationality of using that as a premise in later reasoning. The idea that there is no gap here just is the idea that the principle **Cut** is true.

But while **Cut** seems intuitive in cases like this, Nair argues that it can't be right in general. (And so we have a duty, one he takes up, to explain why cases like Jack and Jill seem like good reasoning.) For my purposes, it is helpful to divide the putative counterexamples to **Cut** into two categories. I'll call them _monotonic_ and _non-monotonic_ counterexamples. The categorisation turns on whether $\Gamma \cup \Delta \vDash A$ is true. I'll call cases where it is true monotonic instances of **Cut**, and cases where it is false non-monotonic instances.

That **Cut** fails in non-monotonic cases is fairly obvious. We can see this with an example that was hackneyed a generation ago.

> $\Gamma =$ {Tweety is a bird}    
> $\Delta =$ {Tweety is a penguin}    
> $A = B =$ Tweety can fly    

From Tweety is a bird we can rationally infer that Tweety flies. And given that Tweety is a flying penguin, we can infer that she flies. But given that Tweety is a penguin and a bird, we cannot infer this. So principles 1 and 2 in **Cut** are true, but 3 is false. And the same pattern will recur any time $\Delta$ provides a defeater for the link between $\Gamma$ and $A$.

These cases will matter in what follows, but they are rather different from the monotonic examples. Here is a monotonic example, based on an argument against E=K by Alvin @Goldman2009. In many ways the argument against E=K I'm going to give is just a notational variant on Goldman's, but I think the notation helps see it in context.

Here's the crucial background assumption for the example. (I'll come back to how plausible this is after setting the example up.) The nature of $F$s around here varies, but it varies very very slowly. If we find a pattern in common to all the $F$s within distance $d$ of here, we can rationally infer that the pattern extends another mile. That's just boring induction. But we can't infer that it extends to infinity - this isn't like working out the mass of an electron. (It's more like working out the details of the diet of some animal.) Now here is the counterexample.

> $\Gamma = \Delta = \{$All the $F$s within 3 miles of here are $G$s.\$}$    
> $A =$ All the $F$s between 3 and 4 miles from here are $G$s.    
> $B =$ All the $F$s between 4 and 5 miles from here are $G$s.

If what I said was right, then this is a counterexample to **Cut**. $\Gamma \vDash A$ is true because it says given evidence about all the $F$s within 3 miles of here, we can infer that all the $F$s within 4 miles are like them. And $\{A\} \cup \vDash B$ is true because because it says given evidence about all the $F$s within 4 miles of here, we can infer that all the $F$s within 5 miles are like them. But $\Gamma \cup \Delta \vDash A$ is false, because it purports to say that given evidence about the $F$s within 3 miles of here, we can infer that all the $F$s within 5 miles are alike. And that's an inductive bridge too far.

I don't know if there are instances of $F$ and $G$ where this particular pattern obtains. That is, I don't know if there are instances of $F$ and $G$ where given a perfect correlation holding within $d$ miles, we can rationally infer it holds within $d + 1$ miles, but not $d + 2$ miles.  It seems likely to me that something like this could be right. 

But note that what I really need for the argument is independent of how we think spatial distance relates to rational inductive inference. What I really need is that there is some similarity metric such that inductive inference is rational across short jumps in that similarity metric, but not across long jumps. One kind of similarity is physical distance from a salient point. But that's not the only kind, and rarely the most important kind.

What is really needed to get this argument going is that there is some similarity metric with an 'inductive margin of inference'. What I mean by an inductive margin of inference is that given that all the $F$s that differ from a salient point (along this metric) by amount $d$ are $G$, it is rational to infer that all the $F$s that differ from that salient point by amount $d + m$ are $G$, but not that all the $F$s that differ from that salient point by amount $d + 2m$ are $G$. And it seems very plausible to me that there are some metrics, and values of $F, G, d, m$ such that that's true. 

For example, given what I know about Miami's weather, I can infer that it won't snow there for the next few hundred Christmases. Indeed, I know that. But I can't know that it won't snow there for the next few million Christmases. There is some point, and I don't know what it is, where my inductive knowledge about Miami's snowfall (or lack thereof) gives out.

But while such cases are plausible, they are weird. And I don't propose to offer any particular story about them. Here's what is weird. It will be easier to go back to the case where the metric is physical distance to set this out, but the weirdness will extend to all cases. Imagine we investigate the area within 3 miles of here thoroughly, and find that all the $F$s are $G$s. We infer, and now know, that all the $F$s within 4 miles of here are $G$s. We keep investigating, and keep observing, and after a while we've observed all the $F$s within 4 miles. And they are all $G$, as we knew they would be. But now we are in a position to infer that all the $F$s within 5 miles are $G$. Observing something that we knew to be true gives us a reason to do something, i.e., make a further inference, that we couldn't do before. That's weird, and I'm going to come back in the next section to how it relates to the story I told about knowledge in chapter \@ref(knowledge).

But for now I want to note that it undermines the E=K principle. There is a difference between knowing $A$ and being able to use $A$ to support further inductive inferences. It is very natural to call that the difference between knowing $A$ and having $A$ as evidence.

The reasoning that I've been criticising violates a principle Jonathan Weisberg calls **No Feedback** [@Weisberg2010 533-4]. This principle says that if a conclusion is derived from some premises, plus some intermediary conclusions, then it is only justified if it could, at least in principle, be derived from those premises alone. A natural way to read this is that we have some evidence, and things that we know on the basis of that evidence have a different functional role from the evidence. They can't do what the evidence itself can do, even if known. This looks like a problem for E=K, as Weisberg himself notes [-@Weisberg2010 536].

The non-monotonic cases where cut elimination fails are also tricky for the E=K theorist, but ultimately not as problematic. Here's how to bring out the problem, and also ultimately how to solve it.

On day 1, Ankita gets as evidence that Tweety is a flying bird, while Bojan gets as evidence that Tweety is a bird, and infers that Tweety flies. At this stage he knows, as Ankita does, that Tweety flies; this was a perfectly good inference. On day 2, they both get as evidence that Tweety is a penguin. Now Ankita knows something special: Tweety is a flying penguin. But Bojan doesn't know this. He can no longer infer that Tweety flies, so doesn't know that Tweety is a flying penguin. And the mystery is to explain what's happened.

The theorist who rejects E=K has an easy explanation. Ankita and Bojan had different evidence on day 1, though they knew the same things. Then when more evidence was added into their evidence set, they could do different things. That's the full mystery solved.

The theorist who accepts E=K can't say just this. They have to say that although Bojan did have as part of his evidence that Tweety flies back on day 1, on day 2 this is no longer part of his evidence. Why is it not? Presumably because it was defeated by the new information. Why was it defeated? The explanation for that can't be that given the new information, his old evidence didn't support the belief that Tweety flies. That can't be right because Tweety's being a penguin doesn't get in the way of the 'inference' Tweety flies, therefore she flies. Instead the story must be, somehow, that this old evidence was defeated, not just the inference from the evidence to this knowledge.

I'm not sure that the E=K theorist has a good story to tell here. But I'm not sure that they don't either. Alexander @Bird2004, in the context of replying to a similar objection, points out that everyone is going to need a theory of evidential defeat. That's right. Unless evidence is taken to be something that is infallible and indefeasible, we have to have some story for how it can be lost. And I certainly don't want evidence to be infallible and indefeasible; if that were true we wouldn't have very much evidence. So the puzzle for the E=K theorist - why does Bojan lose this evidence at this time - is a puzzle for everyone.

This case is still a problem for E=K. The theorist who rejects E=K has, at least in my opinion, a much nicer story to tell about why Bojan doesn't know that Tweety is a bird. But a problem is not a refutation; and the puzzle this case raises for E=K is a puzzle everyone has to solve.

The real problems for E=K come from the monotonic counter-instances to cut-elimination. If any such cases exist, it looks like we need to distinguish between things the thinker knows by inference, and things they know by observation, in order to assess their inferences. That's to say, some knowledge will not play the charactistic role of evidence. And that suggests that E=K is false.

