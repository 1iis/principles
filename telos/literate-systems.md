# Literate systems
> Intent belongs in the medium

Literate systems make intent operational.

Knowing intent is required to engineer fitting processes. Literate programming gave this old fact a concrete form for software: Knuth showed that explanations and instructions may belong together in pairs, built into the structure of the medium itself.

The program is not merely a sequence of commands for the processor, but a text addressed to cognitive beings capable of understanding. The processor needs executable instructions; the human needs the reasons, structure, and order of thought that make those instructions intelligible.

And now, so does the LLM. Knuth’s idea became newly operational because LLMs can use explanations. A compiler ignores intent; a model can use it. Names, prose, examples, outputs, and structure become semantic signals, as much semantic material for the LLM to navigate and replicate.

The LLM is a machine that has leveled up from namespace to ontological space; it is able to manipulate semantics and navigate the structure of meaning. This does not solve understanding in any final philosophical sense. But it does change the engineering facts: semantic material can now guide the machine directly.

A literate system extends that idea from the program to the working medium itself. Prose, code, data, outputs, links, examples, tests, and structure live close enough to inform each other. The artifact is not only something the processor can execute. It is something a person and their LLM can read, understand, maintain, and return to.

This is why notebooks matter. At their best, they are not scratchpads with outputs attached, but readable computational media: places where thought, experiment, result, and explanation can share the same surface. [Wolfram notebooks][wolfram-notebooks], [IPython][ipython-history], [Jupyter][jupyter], [nbdev][nbdev], and [Solveit][solveit] all explore this territory in different ways.[^notebook-lineage]


With tool calling, LLMs can also interact with the working environment: run code, inspect files, read outputs, compare behavior, and revise. Calling this an “agent” often hides the simpler mechanism behind a real step change: prose, code, tools, execution, and feedback now share one loop.

The ideal is not “everything in one file.” The ideal is proximity of meaning. The context needed by a reader, human or AI, should be available without a scavenger hunt.

That proximity serves [intelligible systems][intelligible-systems]. Human-readable structure becomes machine-readable orientation.

The broader practice is [context discipline][context-discipline]: keeping the right intent available in the right place without turning the medium into a dump.

Exploration and durable artifacts do not have to be the same thing. The log is process; the artifact is product. A clean artifact can exist because messy exploration happened elsewhere. In our praxis, this becomes [literate source][literate-source]: writing artifacts so the why and the how remain close enough for understanding to compound.

At the level of personal computing, this points toward [the new personal computer][new-personal-computer]: a working environment where structured human intent and executable capability share a medium.

[^notebook-lineage]: Adjacent systems and descendants include [MATLAB Live Editor][matlab-live-editor], Quarto, Observable notebooks, Google Colab, Modal notebooks, and many other notebook-like, live, or publishable computational environments. They are not all the same thing, but they rhyme: prose, code, data, outputs, and sharing move closer together.

[matlab-live-editor]: https://www.mathworks.com/help/matlab/live-scripts-and-functions.html
[wolfram-notebooks]: https://www.wolfram.com/notebooks/
[ipython-history]: https://ipython.readthedocs.io/en/stable/about/history.html
[jupyter]: https://jupyter.org/about
[nbdev]: https://nbdev.fast.ai/
[solveit]: https://www.fast.ai/posts/2025-11-07-solveit-features.html

[literate-source]: ../praxis/literate-source.md
[context-discipline]: ../praxis/context-discipline.md
[new-personal-computer]: the-new-personal-computer.md
[intelligible-systems]: intelligible-systems.md