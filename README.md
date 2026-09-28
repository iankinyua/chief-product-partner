# Product Discovery Agent

A practical guide for working through a product idea before committing to build it. The assistant works beside you as a product builder: friendly, direct, and willing to challenge a weak assumption. It keeps the evidence straight and uses plain language.

The skill is designed to take an idea from an early question to a decision. If building is justified, it can then help write a product requirements document (PRD). A good discovery may also end with a change of direction or a decision to stop.

## Start here

In ChatGPT, select **Product Discovery Agent** or say:

> Use @Product Discovery Agent. I have an idea for [product]. Walk me through discovery one step at a time. Keep a simple record of what we know, what we are guessing, and what we need to check.

You can also bring a metric, a customer complaint, a proposed feature, or an existing research pack. The agent starts from what you have, rather than pretending every project begins with a blank page.

At any time, ask:

- **“Show me the whole route.”** You get all the stages and where you are.
- **“Show me the current document.”** You get a short view: Stage, What we know, What we don't know.
- **“Give me a worked example end to end.”** You get sample actions and outputs at every stage. Invented research is clearly labelled.
- **“What could make us change our minds?”** You get the strongest competing explanation and the evidence that would settle it.
- **“Draft a PRD now.”** You can get an early draft, with untested requirements marked as such.

## The route

| Step | What we work out | What comes out |
| --- | --- | --- |
| 1. Frame | Who has the problem, what happened, and what decision are we making? | A clear starting question and the missing facts. |
| 2. Understand | What different problems could sit behind the request? | A few possible explanations and how to tell them apart. |
| 3. Research | What do existing sources and recent customer behaviour show? | Sourced findings, limits, and gaps. |
| 4. Make sense of it | Which patterns survive the awkward exceptions? | A sharper account of the problem and useful opportunities. |
| 5. State the bets | What must be true for an idea to work? | Testable beliefs and signs they are wrong. |
| 6. Explore options | What different responses could help? | Options with gains, costs, and risks. |
| 7. Test | Which uncertainty matters most, and what happened when we tested it? | Preset success rules, results, and limits. |
| 8. Decide | Should we build, change direction, test again, wait, or stop? | A decision brief with reasons and a review trigger. |
| 9. Describe the build | If the decision supports it, what should the first version do? | A PRD linked to the evidence, with open questions marked. |

The stages are guides, not a promise that every idea reaches Step 9. New evidence can send us back to an earlier question.

## How we work together

The agent can check public sources, compare options, keep the record, draft interview questions, analyze evidence you provide, and challenge the proposed solution. You bring access to real customers and internal data, make business commitments, and decide what to prioritize. The agent must never claim it interviewed a person or ran a test when it did not.

A useful customer example is recent and specific: “Show me the last post you made. What did you try, where did you stop, and what did you do instead?” A statement such as “people want cheaper AI” is a starting belief. It becomes stronger only when we see who those people are and what they do.

We keep two views of the same work:

1. **A short progress view** with the current stage, what we know, what we don't know, and the next action.
2. **A full evidence record** with sources, dates, counts, limits, corrections, tests, and decisions. Making the progress view shorter must not erase the record.

## Worked example

[AI credits through mobile money](examples/ai-credits-worked-example.md) shows one idea across all nine steps. Its customer interviews, test results, costs, and decisions are **simulated**. Public facts in that example have source links. Do not use the simulated numbers as market evidence.

## Repository contents

- [`product-discovery-agent/SKILL.md`](product-discovery-agent/SKILL.md): the agent's main instructions.
- [`product-discovery-agent/references/`](product-discovery-agent/references/): detail for each stage and evidence handling.
- [`product-discovery-agent/assets/`](product-discovery-agent/assets/): templates for progress, research, decisions, worked examples, and a PRD.
- [`product-discovery-agent/evals/`](product-discovery-agent/evals/): fictional cases and a rubric for testing whether the agent behaves as intended.
- [`product-discovery-agent/agents/openai.yaml`](product-discovery-agent/agents/openai.yaml): display metadata.

The GitHub copy is a guide and versioned source. Editing it does not automatically change an already installed personal skill; that update must also be applied and saved in the skill directory. The evaluation cases are tests of the agent, not evidence about any real product.

## Current status

The skill has been checked for valid structure. The new conversation cases for the simple progress view and worked example have been written, but have not yet been run in fresh conversations. Do not mark them as passed until their actual responses are captured and scored.
