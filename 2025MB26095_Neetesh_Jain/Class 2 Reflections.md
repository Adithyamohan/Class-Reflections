# Session 2: Good enough is a hard sentence for an engineer

1 August 2026 | Neetesh Jain | 2025MB26095

---

You launch when the product is good enough, not when it is good. Wait for good and you launch into a market that has moved.

I have argued against this my whole career without knowing it had a name. Every time I have pushed back on a date, the real content of my objection was that the thing was not good yet. Not broken, not unsafe, just not good. Thin error handling, inconsistent logging, three places where an unlucky retry would double charge.

Some of those were correct and some were craft dressed up as risk, and I had no way of telling which at the time. The test offered here is whether it does the job for the customer without harming them. By that test, inconsistent logging is not a launch objection. It is my objection.

**Where I think the advice is wrong for software.** Deferring decisions until late, with structure fixed early and paint colour left open, works cleanly for physical things because the structural decisions announce themselves. In software the expensive irreversible decisions do not look structural. They look small.

The data model is the clearest case. Deciding what a record means, what it is keyed on and what it can relate to is a two hour conversation early and a twelve month migration later. It has none of the appearance of a foundation, and nobody in a planning meeting has ever flagged a field definition as a one way door.

So I accept the principle and think the entire difficulty is in classification, which the session moved past quickly. My working rule is that the one way doors in software are the ones that change the meaning of stored data, and nearly everything else can wait. I would like to test that rule rather than trust it.

**TRL, and something I had misfiled.** The readiness scale from 1 to 9 was new to me in name only. What the fuller version adds is that there are several distinct stages between a working demo and a thing that survives in its real environment, and that most failures live in those middle stages rather than at either end.

That matters for the economics I am building. I had been modelling cost at two points, prototype and steady state. The long middle where it works in a controlled setting and not yet in the real one was priced at zero, and it is probably the most expensive part.

**Spending someone else's money.** Engineers are kept a long way from this. In ten years nobody has told me what the thing I was building cost to build or what it earned. I was trusted with the architecture and not the arithmetic, and I never questioned the split. I assumed the numbers were above my level and, honestly, that they were somebody else's problem, which was restful.

Now that I own the economic model, the first thing I noticed is that the numbers change my technical opinions. A design choice that adds one API call per engagement is invisible to me as an engineer and material across a practice. I have made that kind of choice many times without knowing it had a price. I do not think engineers are deliberately shielded from this. I think nobody has considered that telling them would change what they build. It would have changed what I built.
