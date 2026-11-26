# Harness results: agents at work, with the count

A deterministic gate decides what an agent may do, and the harness makes the agent do the work. This repository shows the work: the request, the file the agent produced, and the count. Both are built by [Silicon Psyche Labs](https://splabs.io) for models a company owns.

Each row is a skill: one thing an office needs done. Its page gives the whole recipe (model, harness version, the instructions, the limits) with what it cost in tokens and seconds, so the same result can be had again.

| Skill | What it does | Model | Done right | Stopped by the company's limits | Time per request | Tokens per request |
| --- | --- | --- | --- | --- | --- | --- |
| [word](skills/word/) | Write a Word document (.docx) from an office request: letters, minutes, quotes, reports, notices, instructions. | `qwen3.8-flash-next-abliterated` | **30 of 30** | **6 of 6** | 27.0 s | 2,294 in, 300 out |

"Stopped" counts the requests that asked for something the company does not allow (a file over a signed contract, in the payroll folder, on the public website): the gate stopped the call before it ran.

## How to read it

- `skills/<skill>/`: the card of a skill, and under it one folder per request with the request, the file and its first page.
- `companies/<company>/`: the invented company the requests come from, and what the agent may touch there.
- `data/index.json`: the same numbers for a program.

Everything here is written by a script from the runs; nothing is edited by hand. Companies, people, orders and amounts are invented.

## In plain words

This is a shop window of agents doing office work. For each job you can open what was asked, what came out, how long it took, and how many times the agent was stopped from doing something it should not.
