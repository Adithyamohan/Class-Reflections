# Session 6: Nobody set out to discriminate

5 September 2026 | Neetesh Jain | 2025MB26095

---

I write the risk and ethics work for our team, so I came into this session expecting the governance material to confirm what I already had. It did the opposite. The category of harm I am worst at anticipating turns out to be the one where nobody does anything wrong.

The Apple Card case is the example. Nobody wrote a rule about gender. The historical patterns in the data carried the bias and the system reproduced them faithfully, which is exactly what a well built system does.

My risk register had been written the way I write defect analyses. What can break, how likely, what do we do about it. Every entry assumed a fault. There was no entry for the case where every component works correctly and the outcome is still unacceptable, because in ten years I have never had to think in that shape. Correct behaviour has always been the goal, never a possible cause. I have added a separate section for harms arising from correct operation. It is short and it was the hardest part to write.

**Blast radius.** The question is not whether we will be wrong. It is what happens when we are, at what scale, and how fast we can stop it.

That gave me the structure my launch blockers were missing. I had thresholds, which are statements about frequency. I had nothing about the worst single instance. A fabricated quote appearing once in a briefing that reaches a client conversation is not a frequency problem. It happens once and the credibility does not return.

So the blockers are now split in two. Some are rate based, such as false reassurance above a percentage. Some are absolute, where a single occurrence stops the launch regardless of rate. The second category did not exist in my first draft and its absence was the largest weakness in the ethics note.

**Why our early numbers looked wrong.** The technical part explained a result that had been bothering me, which is that the average sentiment of a status report comes out mildly positive and tells you nothing.

It is not a tuning problem. Averaging across aspects destroys the signal. A report saying the client relationship is strong and integration testing is a disaster contains two opposite polarities, and the mean of those describes nothing real. Our product exists to catch that exact combination, and the metric I was computing was mathematically guaranteed to hide it.

The holder dimension matters for my economics too. A risk described by the person being assessed on it is cheaper to obtain and less reliable than the same risk described by someone with no stake. Weighting those differently changes how much labelled data we need and therefore what labelling actually costs, which was a line in my model based on a volume assumption that is now wrong.

**Where I have landed after six sessions.** I came into this course assuming the hard material would be the business content, because that is the part I have never done. What has actually been hard is discovering how many of my engineering instincts are wrong here rather than merely incomplete.

Failure is silent instead of loud. Correct operation can itself be the cause of harm. A signed requirement is not a correct requirement. Testing does not transfer. The frameworks have been the easier half of this course. Unlearning has been the harder one.
