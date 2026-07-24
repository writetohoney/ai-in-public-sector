# AI policy agents

This folder holds small, applied AI tools built for the course — both instructor examples
and student **Track B** prototypes from the [final project](../assignments/final-project.md).
Building something is part of understanding it: the fastest way to see what these tools can and
cannot do in a public-sector setting is to try to make one work.

## How to add an agent

Each agent lives in its own subfolder. Copy [`example-agent/`](./example-agent) as a starting
point. A complete agent folder should contain:

- `README.md` — what the agent does, who it is for, and its governance considerations and limitations
- the code (e.g. `app.py`, `agent.py`) and a `requirements.txt`
- any `templates/` and `static/` assets
- a short **design rationale** (the Track B deliverable): the problem addressed, the technical
  approach, the governance considerations, and the limitations

## Governance note — required for every agent

Because these are public-sector tools, every agent in this repo must document, in its README:

1. **Purpose** — the specific problem it addresses and who it serves.
2. **Data** — what data it uses, where that data comes from, and its provenance.
3. **Accountability** — who is answerable for the agent's outputs.
4. **Contestability** — how a person affected by an output could get an explanation and challenge it.
5. **Limitations** — where it should *not* be trusted or used.

An agent that cannot answer 3 and 4 is not ready to make or shape a consequential public-sector
decision. That is a course principle, not a formality.

Points 3 and 4 are the same questions the course applies to whole institutions — *who is
accountable*, and *how does an affected person get an explanation and challenge it* — as
Dimensions 6 and 7 of the [adaptive capacity diagnostic](../resources/adaptive-capacity-diagnostic.md).
A tool you build yourself is the smallest scale at which they can be answered honestly, which
makes it a good place to practise.
