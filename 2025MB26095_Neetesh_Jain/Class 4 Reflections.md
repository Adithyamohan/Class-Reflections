# Session 4: Drift does not raise an error

22 August 2026 | Neetesh Jain | 2025MB26095

---

The idea I have not been able to put down is silent degradation. A model can get quietly worse while everything around it reports healthy. No exception is thrown, no alert fires, the logs are clean. The system is confidently wrong and the monitoring agrees with it.

Ten years of engineering has trained me to trust a specific chain of reasoning. The tests pass, so the behaviour is what we specified. The error rate is flat, so nothing has broken. Every instinct I have for judging whether a system is healthy depends on failure being loud.

None of that survives here. In a system whose output is a judgement rather than a result, being wrong looks exactly like being right. There is no signal at the layer I am used to watching.

This is now the line I keep repeating to the team, and it is in our launch blockers: a definition of a risk signal with no named owner will drift away from the business within two quarters and nobody will notice, because drift does not raise errors.

**An admission about my own preferences.** When the appropriateness ladder went up, my honest first reaction was mild disappointment, because if the answer is rules then the work is boring. Ten years has given me a preference for the interesting solution that I dress up as a preference for the capable one, and I recognised it instantly. The real version of this failure is not picking an absurdly oversized tool. It is picking one that is a single rung too high, and having it work, and the cost only appearing later as something you cannot evaluate, debug, or explain to a client.

**Where I disagree with the room.** The discussion about automating work people value split between giving people back an hour and people suspecting headcount cuts. Both are real and both understate the engineer's version.

In my experience resistance is usually about blame. When a person does the task and it goes wrong, the failure is understood, there is a reason, there is a conversation. When a system does it and it goes wrong, whoever owns the system is blamed for a decision they did not make and cannot reconstruct. So automation converts an explainable mistake into an unexplainable one attached to your name, and no amount of communication about headcount addresses that. What addresses it is the audit trail. I now think of traceability as a change management feature rather than a compliance one.

**Tail risk, and a change to the register.** Our product cannot injure anyone. What it can do is quiet. Client A's commercial details appearing in Client B's briefing is a contract breach that ends a relationship rather than generating a defect ticket.

My instinct, from years of defect triage, is to rank by probability times impact. For tail cases that arithmetic misleads, because a very small number multiplied by a very large one produces a middling score that puts a relationship ending event next to a display bug. I have moved those out of the scored list into a set of absolute blockers, where the question is not how likely it is but whether we could survive it once.

**What my organisation would have to change.** All of this assumes someone is funded to check that the system is still right. Monitoring budget gets approved for availability and never for correctness. We pay for uptime dashboards and have never once funded the ongoing work of verifying that the output is still good. For a deterministic system that was defensible. Here it is the whole game, and it is a running cost with no natural owner.
