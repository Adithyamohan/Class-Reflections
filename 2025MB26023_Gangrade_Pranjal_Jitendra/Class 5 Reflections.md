# Reflection: Session 5

29 August 2026 | Gangrade Pranjal Jitendra | 2025MB26023

---

Data, model, API, user experience. Then the claim that AI products are won or lost at the UX layer, and that a legal disclaimer is not a design.

I did not want to agree. I am the build lead and my instinct is that the hard problems are in extraction and ranking. But I can prove the point from our own work. Our confidence design has three states: high means the action is drafted and ready to approve, medium shows the recommendation alongside the evidence pointing the other way, low means the agent says it cannot judge and shows raw evidence. That design took one conversation. The extraction pipeline took weeks. The three state design decides whether a manager over trusts the thing. Extraction quality mostly decides how often we are embarrassed. Only one of those kills the product.

We have not solved the related problem, which is that a ranked list with numbers beside it communicates precision whether we intended it or not. Position four is a different quality of claim from position one and our interface makes them look identical.

**Build versus buy.** Our position is buy the platform, build the judgement layer. The data already sits in Salesforce and the platform inherits sharing, field level security and audit trail for free. Rebuilding that outside means a second copy of confidential client data, which is the biggest risk in the product.

What the session added was the instruction to own the capability and not the model. Tested against us, what is ours is the evidence schema, the risk taxonomy, the ranking logic, the confidence rules and the approval workflow. None of it is the model. That is a better statement of our moat than the one we had written.

I am less comfortable about lock in. We are betting on a platform, not just an API format, and per conversation pricing scales with exactly the thing we want to grow. Applying Porter now and Porter eighteen months out is the right discipline and we have not done it properly.

**Materiality.** The intranet example was a team wanting a full UI for a hierarchy that had not changed once in years. I ran the test over our backlog and two items failed it, both about engagement setup, which happens twice a quarter. We were treating it as a workflow because it is one. It is just not frequent or painful.

**Human in the loop is a hill to climb, not a word to speak.** The fatigue argument landed on me personally within seconds. I approve Cursor's changes far more readily than a colleague's pull request, and the volume is higher. What I had not designed for is the thirty seconds in which someone decides: why it escalated, what was uncertain, what was missing, and whether the data is stale. We built the evidence trail for auditing after the fact. We also capture rejection reasons and nothing about approvals, which biases our data toward disagreement.

**Unconvinced.** The claim that a small model would often beat the support systems firms pay crores for may be true. I cannot verify it, and it is the kind of claim that is satisfying to believe.
