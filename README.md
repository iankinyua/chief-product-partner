# Product Discovery Agent

A practical guide for working through a product idea before committing to build it. The assistant works beside you as a product builder: friendly, direct, and willing to challenge a weak assumption. It keeps the evidence straight and uses plain language.

The skill is designed to take an idea from an early question to a decision. If building is justified, it can then help write a product requirements document (PRD). A good discovery may also end with a change of direction or a decision to stop.

## Download the skill

1. At the top of this GitHub page, click **Code → Download ZIP**.
2. Extract the downloaded repository ZIP.
3. Inside it, find the **`product-discovery-agent`** folder. This is the skill; the repository's `README.md` and `examples` folder are guides, not part of the upload.
4. Compress just the **`product-discovery-agent`** folder into a new ZIP. On Windows, right-click the folder and choose **Compress to ZIP file** (or **Send to → Compressed (zipped) folder**). On Mac, right-click and choose **Compress "product-discovery-agent"**.
5. Check that opening your new ZIP shows **`product-discovery-agent/SKILL.md`**, along with its `assets`, `references`, and other folders. If the ZIP opens with the whole repository or with `SKILL.md` at the top level, zip the skill folder again.

Keep this new ZIP for the upload steps below. Downloading a GitHub ZIP does **not** install the skill in either app.

## Install in Claude

1. Open [Claude](https://claude.ai/) and go to **Customize → Skills**.
2. Click **+ → Create skill → Upload a skill**.
3. Select the ZIP you made above.
4. When Product Discovery Agent appears in your skills list, turn it **on**.
5. Start a new chat and try: “Use Product Discovery Agent to help me explore an idea for cheaper AI access for small business owners. Start with the problem.”

If **Skills** is missing or greyed out, check whether code execution is enabled in Claude's settings. In an organization, an admin may control skill creation. See [Claude's skill instructions](https://support.claude.com/en/articles/12512180-use-skills-in-claude).

## Install in ChatGPT

1. In ChatGPT, open **Plugins → Skills** in the sidebar.
2. Click **Create → Upload from your computer** and select the ZIP you made above.
3. Wait for the upload scan. If ChatGPT asks you to review the skill, review it before using it.
4. Start a new chat. Type `@` and select **Product Discovery Agent**, or ask ChatGPT to use it by name. Try the same small business idea prompt above.

If you cannot see **Plugins → Skills** or the upload option, it may not be available on your account or your workspace may have disabled uploads. The GitHub link alone does not install it. See [OpenAI's ChatGPT skill instructions](https://help.openai.com/en/articles/20001066-skills-in-chatgpt). For local Codex use, see [OpenAI's skill setup guide](https://learn.chatgpt.com/docs/build-skills).

## Start here

Once the skill is installed, start a new chat. Here is the same first request in each app:

### In ChatGPT

Type `@`, choose **Product Discovery Agent** from the list, then send:

> I want to help small business owners buy affordable AI access using mobile money. Walk me through product discovery one step at a time. Start by helping me define the problem. Keep a simple record of what we know and what we still need to check.

### In Claude

Make sure **Product Discovery Agent** is on under **Customize → Skills**. Then start a new chat and send:

> Use my Product Discovery Agent skill. I want to help small business owners buy affordable AI access using mobile money. Walk me through product discovery one step at a time. Start by helping me define the problem. Keep a simple record of what we know and what we still need to check.

For a different idea, replace the small business sentence with your own. For example:

> I have an idea for [product] for [customer]. Help me check whether the problem is real before we decide what to build.

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
