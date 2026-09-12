# Reflection: Session 6

5 September 2026 | Gangrade Pranjal Jitendra | 2025MB26023

---

I expected the sentiment analysis section to be background. It was the most useful thing in the course so far, because task two of our product is exactly this and I had been treating it as a prompt engineering exercise.

The opinion quintuple is what I did not have: entity, aspect, sentiment, holder, time. I was extracting sentiment and a source record. Not separating aspect from entity means a report saying the client relationship is strong and integration testing is a disaster collapses into an average that describes nothing, and catching that exact combination is why our product exists. The holder matters just as much, because a risk described by the person being judged on it is a different signal from the same risk described by an architect. And a concern raised eight weeks running is a different object from one raised once. We had the timestamp and no logic using it. We have rewritten the extraction schema around this.

**Why it is harder than it looks.** Status reports are full of implicit opinion. "We are continuing to work with the client to align on sign off criteria" contains no negative word and anyone in delivery reads it instantly as trouble. The negative content is entirely in the fact that alignment is still being worked on in week nine. A general purpose model scores that as neutral. So our labelled data cannot be generic. It has to come from people who read these documents for a living, marking what they inferred rather than what the words said, and that costs more than we budgeted.

**The black box method.** Start from the outcome, define inputs and outputs, then ask what must happen inside, and choose the technique last. I would have claimed I do this. Tested honestly, my instinct is to ask what the platform can do and find the shape of problem that fits, which is starting with the technology in different clothes. The warning about optimising the wrong thing beautifully is the real risk. A perfect risk extractor is useless if what stops engagements failing is not detection but whether anyone acts. Time from first signal to first governance action is the only measure on our list that tests the product rather than the machine.

**The articulation gap.** The crying child cannot tell you what is wrong. When we interviewed delivery managers they described a time problem, not enough hours. Build to the stated need and you build a summariser. The actual need is that attention goes to whoever is making noise rather than to whatever is most at risk. That is a different product. I have blamed clients for bad requirements for eight years, and extracting the real need is my job, not theirs.

**Consent.** Consultants write status reports to communicate project status. They did not write them so a model could infer risk about their own engagement. The data is the firm's and the purpose has changed. This is not a compliance box, it is the survival condition, because if people believe their words are being read for signals about their honesty, the words get vaguer and our input disappears.

**After six sessions.** Almost none of this was about models. I came in as a technical person hoping to learn the product side. The technical part was never what I was missing.
