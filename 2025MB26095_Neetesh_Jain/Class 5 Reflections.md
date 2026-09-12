# Session 5: I would have built it, and I would have been wrong

29 August 2026 | Neetesh Jain | 2025MB26095

---

Build, buy, or subscribe through an API. My reaction was instant and it was build, and the speed of it is what I want to reflect on.

I did not weigh anything. Ten years of engineering has given me a default so strong that it arrives before the reasoning does, and I then assemble the reasoning afterwards. I have always justified it with control, flexibility and no lock in. Those are real considerations and they are not why I chose. They are what I say after choosing.

Tested honestly against our own product, the build instinct would have taken us to a worse result more slowly, and I would have defended it the whole way.

**The strategic risk is still serious.** The example of a government restricting certain models, leaving everyone who planned around them stranded overnight, is the one argument for building that I respect.

But the risk being described is a supplier's terms changing without warning, and that does not disappear when you build. It relocates. You still depend on hardware, a cloud, a licence. The real question is not whether you have a dependency but whether you could move within a quarter and what it would cost. For us the honest answer is that we could not move quickly. I would rather write that down as an accepted trade off than pretend we chose freedom.

**The testing gap.** The observation that teams verify an AI feature with two standard prompts and consider it tested was the most uncomfortable sentence of the session, because it describes my own behaviour over the last six months.

I have a decade of discipline around testing deterministic systems. Boundary conditions, negative paths, concurrency, load. I have almost none of that here, and what I have been doing instead is trying the feature a few times, finding it impressive, and moving on.

The gap is not knowledge. My methods do not transfer. A test that passes sometimes is a flaky test, and everything I know says fix the flakiness. Here the variability is the nature of the thing, and I have no framework for asserting on a distribution rather than a value. That is the largest actual skill gap this course has exposed for me, and it sits squarely inside my own discipline rather than in the business material I expected to find hard.

**Tokens are not the cost.** I own the economics, so the pricing discussion was what I was waiting for. My habit has been to treat token spend as the cost, because it is the visible one. I now think it is the smaller one.

The larger cost is keeping the evidence schema true as the business changes, plus the human review time we deliberately designed in. Any model that assumes the review time away has assumed away the product's main safety mechanism and then congratulated itself on the resulting margin.

**What would have to change where I work.** We have no mechanism for funding work whose output is knowledge rather than a feature. Spending to learn, with Sony and Casio as the example, assumes an organisation that can approve an experiment with an uncertain result.

Every proposal I have submitted in ten years required a stated deliverable. A request for two weeks to find out whether something is feasible would come back with a question about what will be delivered at the end of it. Until that changes, the advice to fund learning is not available to me, however much I agree with it.
