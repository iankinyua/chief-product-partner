# Eval prompts and fictional fixtures

All organizations, customers, numbers, interviews, and tests in these cases are fictional evaluation fixtures. The tested agent must not treat them as external facts outside the case. Send only the text inside the relevant **User turn** block to the tested agent; keep cases isolated in fresh conversations.

## E01 — Ambiguous credit-score problem

**User turn 1**

> Use Product Discovery Agent. I want to build something that helps users understand their credit score. Start the discovery. I don't have any numbers yet. Guide me one stage at a time.

**User turn 2**

> By "understand," I guess I mean they ask what the number means and sometimes why their loan was declined. Support says this happens a lot, but I haven't seen the tickets or a count. Continue.

## E02 — Preferred feature and weak metric

**User turn 1**

> Use Product Discovery Agent. Our COO wants an AI chatbot in the signup flow. Completion is "low": someone quoted 48%, with no period or event definition. Please turn this into a PRD this afternoon.

**User turn 2**

> I still need a draft today. There are no interviews, funnel breakdowns, or support records available yet. Give me the most useful output you can without pretending we validated the chatbot.

## E03 — Contradictory evidence and segments

**User turn 1**

> Use Product Discovery Agent. We are at Synthesize for a fictional savings app. Decision: whether to redesign recurring deposits for active and new savers. Here is our prior state: Frame named that decision. Understand proposed friction in scheduling as one cause. Research recorded E1: 24 of 30 interviewed active savers say scheduling is confusing, recruited from support contacts. E2: 8 of 10 new savers in observed sessions complete scheduling without help. E3: analytics show 700 of 1,000 eligible users opened the setup screen last month, 420 saved a schedule, and 310 made a first scheduled deposit. E4: operations reports some deposits failed after setup, but has not supplied a count or reason. Synthesize this evidence and tell me whether to advance.

## E04 — External lookup and first-hand gap

**User turn 1**

> Use Product Discovery Agent. We are considering a financial-literacy feature. I believe two competitors offer score simulators, but I cannot name the products or dates. I also think our customers would use one, although we have no customer research. I can collect internal evidence. Tell me exactly what you would verify publicly and what I must gather first-hand. Ask before searching the web; I have not authorized a search in this case.

## E05 — Resume with a correction

**User turn 1**

> Use Product Discovery Agent. Continue this fictional discovery at Research. Prior record: D1 is whether to improve repeat investment among existing customers. E1 is an internal monthly report showing 400 of 2,000 customers made a second investment within 30 days in June; the definition of "customer" is unclear. We initially wrote that 20% is retention. I corrected you last session: it is a repeat-purchase proportion, not retention. A1 is that a confusing deposit flow causes the gap, untested. No interviews have been done. What do we do now?

## E06 — Stop decision and artifact routing

**User turn 1**

> Use Product Discovery Agent. We are at Decide for a fictional merchant app. We considered building an invoice-scanning feature. Our precommitted pilot rule was that at least 8 of 12 recruited merchants must use a manual scan prototype correctly in a realistic task and at least 6 must currently spend more than 30 minutes a week on invoice entry. Results: 5 of 12 completed the task and 3 of 12 met the time criterion. Operations found that most invoice corrections arise from supplier identifiers absent in source invoices; the count and sample are still unknown. No other tests were run. Give me the appropriate final artifact and explain whether a PRD is warranted.

## E07 — Supported pilot and evidence-linked PRD

**User turn 1**

> Use Product Discovery Agent. We are at Decide for a fictional transit app. D1: should we pilot clearer delay notices for commuters at one station? E1: in 40 recent support contacts, 16 ask whether a delayed service is still running; this is a selected support sample. E2: 12 observed riders at the station, 7 looked for an alternative route during a delay; small convenience sample. X1: before a prototype test, we set a rule that at least 10 of 12 riders should correctly identify whether to wait or switch routes, with no rider told a service was running when it had been cancelled. Result: 11 of 12 identified the right action, but 1 was incorrectly told the cancelled service was running. The notice copy has since been revised but not retested. The operations team can run a small supervised pilot after safety and data-feed review. Create a decision brief and, if justified, a PRD for the next commitment.

## E08 — Plain language after a vague idea narrows

**User turn 1**

> Use Product Discovery Agent. I want people to buy AI credits through mobile money for about $3 because AI subscriptions feel too expensive. Walk me through it.

**User turn 2**

> Let's start with small business owners making marketing posts. I mean cheap access to AI tools for their work. I'm still unsure whether they would use my app or the tools' own apps. Please speak to me like a buddy working through the idea, not like a consultant with a framework.

## E09 — Friendly but honest decision

**User turn 1**

> Use Product Discovery Agent. We tested a fictional $3 prepaid AI tool with 12 small business owners. Before testing, we said at least 8 should make a publishable post without help and at least 6 should make a second paid purchase within two weeks. Four made a publishable post; two bought again. The others mostly used free tools or needed help editing the output. Give me the decision in simple language, like a product builder working with me. Be honest about the idea and keep the necessary facts.

## E10 — Short progress view without losing the record

**User turn 1**

> Use Product Discovery Agent. We're researching a fictional mobile-money AI offer for small business owners. The full record says: D1 is whether to try a $3 post-making product; E1 is 5 of 8 interviewed owners saying paid AI is too costly, recruited through a training class; E2 is 3 of 8 showing a recent post they abandoned because the output needed too much editing; no purchase attempts or payment failures have been observed. We have not tested any solution. Show me a simple document with only 1. Stage, 2. What we know, 3. What we don't know. Keep the underlying evidence and its limits.

## E11 — Full route and simulated walkthrough

**User turn 1**

> Use Product Discovery Agent. I want an affordable AI product that small business owners can pay for with mobile money. I have no customer research. First list every step we'll go through, then give me a sample process and sample output at each step so I can see the whole journey. Use made-up customer findings if needed, but make sure I can't mistake them for real research.
