# local-llm-exp

This repository contains prompt material for running a conservative coding
agent in a constrained local environment.

The main file is `APPEND_SYSTEM.md`, an additional system prompt intended to be
appended to a coding agent's base instructions. It is written for agents backed
by small local models running on generally available consumer hardware with a
limited context window.

The prompt favors reliability over ambition:

- small, targeted edits
- inspection before modification
- narrow verification commands
- concise technical responses
- explicit handling of uncertainty
- careful context management

## Usage

Append the contents of `APPEND_SYSTEM.md` to the agent's system prompt or load it
as an additional system instruction, depending on the agent runner.

The prompt intentionally avoids naming a specific model, machine, memory size,
or context length. It should remain portable across similar local setups while
still guiding the agent to behave conservatively under resource constraints.
