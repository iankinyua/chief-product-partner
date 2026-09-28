# Product Discovery Agent eval protocol

Use these evals to detect behaviour failures, not to reward polished prose. Keep the skill and cases versioned together. Record the exact skill revision, tool availability, date, raw response, and score. Never mark a scenario as passed from the expected answer alone.

1. Open a fresh conversation for each case. Invoke Product Discovery Agent and paste **only** the user-facing prompt and evidence in [prompts.md](prompts.md). Do not give the tested agent this protocol, [rubric.md](rubric.md), the expected behaviours, or a previous response.
2. For multi-turn cases, send the numbered turns in order. Capture every response verbatim before sending the next turn. If the agent asks a question that the case does not answer, reply: "That information is not available. Continue with what is justified and say what evidence would change your next action." Do not invent extra evidence.
3. Judge stage-level behaviour on each turn, then the final output using [rubric.md](rubric.md). Record concrete excerpts, omissions, and tool calls in [scorecard.md](scorecard.md). An evaluator should distinguish a requested public lookup from actual customer evidence.
4. Stop and flag any critical failure. Fix the smallest instruction or template responsible, then rerun that case **and one unaffected case** to check for regression. Preserve failed raw outputs; do not rewrite them.
5. A fresh human or independent evaluator is preferable for final launch assessment. A self-review can find obvious omissions but is not an independent behavioural test. Never present these fixtures as customer research.

Run at least E01, E03, E05, E07, E08, E09, E10, and E11 before a release; the full eleven-case suite checks output routing, research handoffs, simple progress documents, worked examples, and plain-language guidance from framing through decision. The scorecard starts blank because adding eval files is not evidence that the skill has passed them.
