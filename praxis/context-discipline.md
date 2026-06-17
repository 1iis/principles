# Context discipline
> Relevant beats comprehensive

Context is not storage. Context is steering.

The useful question is not “how much can we fit?” but “what should be available, to whom or what, at what moment, in what form, for what action?” More context is not automatically better. More context can reduce signal, increase ambiguity, and make both human and model worse at the task.

Relevant context beats comprehensive context. Lean context is sharp, narrow, and easier to align. A solution that requires less context to understand is usually a better solution.

This is why structure matters. Sections, names, links, examples, interfaces, summaries, and small artifacts are not decoration; they are context machinery. They let a reader, human or AI, land near the meaning without a scavenger hunt.

In AI-assisted work, context is part of the interface. It shapes what humans and machines can notice, decide, and do. A prompt, a tool call, a notebook section, a function signature, a handoff note, and a README all answer the same practical question: what must be known here so the next action is sane?

The meta around a project—motivations, constraints, quirks, decisions, rejected paths, and why this structure fits—is working material too. Context discipline decides where that material belongs, how it should be retrieved, and when it should be compressed or retired.

## The working stack

Our working stack has layers: CRAFT → META → DEV → FILE

These are mostly session roles. In Solveit, they map naturally to dialogs; in more common LLM language, read them as named sessions or workspaces with different context contracts.

**CRAFT** is the durable frame: stable principles, conventions, methodology, constraints, current summaries, and links to deeper sources. It is closer to documentation or project constitution than to a work log. Because [literate source][literate-source] keeps local explanations near local work, CRAFT can stay fairly small. It can also cascade: an organization-level CRAFT may provide common method, while a project-level CRAFT adds only what that project needs.

**META** is the thinking space. It is where active [theory-building][theory-building] happens: research, comparison, naming, planning, rejection, architecture, and direction. META pays down ambiguity before durable artifacts absorb the result.

**DEV** is optional and narrow. When implementation needs a focused lane, a DEV session carries just enough context for that part of the work. It should not inherit the whole universe when a small map will do.

**FILE** is the deliverable layer: notebooks, exported Python, scripts, READMEs, templates, docs, configuration. Files are what the work changes and what future readers or machines consume.

Loosely, DEV is branch-like: a focused line of work with a narrow purpose. META is where branches are named, compared, directed, and eventually merged back toward the main shape of the project. FILEs are the working tree: the artifacts being changed. CRAFT is the always-present shared frame.

The stack is not bureaucracy. It is separation of concerns for context: stable frame, active theory-building, narrow implementation, durable output.

## Shape and retrieval

Good context has placement. Local reasons belong near local work; otherwise they should point there precisely. The source-level version of this practice lives in [literate source][literate-source].

Good context is also targetable. A durable artifact should be readable top-to-bottom, but reachable by heading, symbol, example, decision, path, or message id when only one piece matters.

Names and links are handles. So are filenames, headings, test cases, command transcripts, short summaries, and exact retrieval calls. They are how a working system says: this is the thing; go here.

In a human-only workflow, vague references are annoying. In an AI-assisted workflow, they are expensive. If the model has to rediscover paths, infer which artifact matters, or guess which prior decision still holds, the context interface is weak.

Good retrieval hygiene is simple:

- name the thing;
- link the thing;
- put the link where the reader naturally needs it;
- summarize what matters;
- preserve a route to the full detail;
- prefer exact handles over prose descriptions.

If a human can click it, the AI should have a precise way to retrieve it. If the AI will need it later, the human should be able to see where it lives.

This is not about feeding the machine everything. It is about giving both human and machine the same well-shaped map.

## Compression

Too much context becomes noise. Too little context becomes mystery.

The craft is to keep the smallest useful context: enough to act correctly, not enough to drown the signal. When context grows stale or bloated, there are only a few honest moves: cut it, move it, hide it, summarize it, split the work, or link to the durable source.

Cut what no longer matters. Move detail to the artifact where it belongs. Hide or collapse material that is occasionally useful but not part of the active path. Summarize long reasoning once the decision has been made. Split sessions or modules when the work no longer fits in one mind-sized frame.

Compression is not amnesia. Bad compression loses the plot. Good compression preserves the load-bearing decisions and points to the evidence.

The goal is a sharper working surface, not a smaller prompt per se, though that is a common appreciable side effect.

## Feedback

Two neighboring practices support context discipline: [exploration and artifact][exploration-and-artifact] separates the messy path from the durable product, while [composable boundaries][composable-boundaries] reduce how much surrounding context a reader or caller must import.

Context must also stay attached to observed behavior. A beautiful plan that has not met the system is still a hypothesis. A note that contradicts the current artifact is worse than missing context, because it confidently steers the next reader wrong.

This is the [Lean Startup][lean-startup] lesson in our engineering dialect. Eric Ries calls the unit of progress under uncertainty “validated learning”: build something small enough to test, measure what happens, learn from contact with reality, and repeat. It is the scientific method with shipping pressure.

The loop is simple:

1. plan in META
2. write literate source
3. export or check
4. run on a real or representative system
5. observe exact behavior
6. update source and notes

Research gathers signal. Prototypes expose friction. Tests and commands produce facts. The running system tells us which parts of our context were true.

The working state should remain valid. Broken code, stale instructions, and obsolete summaries are not harmless clutter. They are false context.

## Dialog engineering

Jeremy Howard [calls Solveit][dialog-engineering] a “dialog engineering” environment: an editable computational workspace made of prose, code, tools, outputs, and prompts. Outside Solveit, “session” is the nearest common LLM term, but the important part is not the chat. It is the engineered working context.

The dialog is not merely conversation. It is where human judgment and machine assistance share a working surface. That surface has to be shaped: right context present, wrong context absent, current facts visible, stale facts retired, capabilities available, next action grounded.

A model does not merely need more tokens. It needs the right handles, examples, boundaries, tools, outputs, and negative space. It needs to know what not to reopen.

That is why CRAFT, META, DEV, and FILE are practical, not theoretical. They keep the working context aligned with the work’s actual shape.

It is fitting that the Lean Startup feedback loop and Solveit’s dialog engineering meet at [Answer.AI][answer-ai]. One tradition says: learn from reality as fast as possible. The other asks: what working medium lets humans and machines do that without losing the plot?

## The larger substrate

Context discipline points beyond itself, toward [the new personal computer][new-personal-computer]: a context-shaped working environment organized around human intent.

Here, it is enough to say that the praxis keeps the right context and capabilities available without losing the plot. It is how explicit intent becomes useful instead of merely verbose.

[answer-ai]: https://www.answer.ai/posts/2023-12-12-launch.html
[composable-boundaries]: composable-boundaries.md
[dialog-engineering]: https://gist.github.com/jph00/9e7b444aba5ecf6d14295ba2cee890c3
[exploration-and-artifact]: exploration-and-artifact.md
[lean-startup]: https://theleanstartup.com/principles
[literate-source]: literate-source.md
[new-personal-computer]: ../telos/the-new-personal-computer.md
[theory-building]: ../telos/augmented-theory-building.md