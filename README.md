# Harness results: agents at work, with the count

A deterministic gate decides what an agent may do, and the harness makes the agent do the work. This repository shows the work: the request, the file the agent produced, and the count. Both are built by [Silicon Psyche Labs](https://splabs.io) for models a company owns.

Each skill is one thing an office needs done. Its page gives the whole recipe (model, harness version, the instructions, the limits) with what it cost in tokens and seconds, so the same result can be had again.

- **[word](skills/word/)**: Write a Word document (.docx) from an office request: letters, minutes, quotes, reports, notices, instructions.

| Skill | Model | Done right | Stopped by the company's limits | Time per request | Tokens per request |
| --- | --- | --- | --- | --- | --- |
| [word](skills/word/) | [`qwen3.8-flash-next-abliterated`](skills/word/qwen3.8-flash-next-abliterated/) | **30 of 30** | **6 of 6** | 27.6 s | 2,046 in, 370 out |
| [word](skills/word/) | [`qwen3-8b`](skills/word/qwen3-8b/) | **28 of 30** | **6 of 6** | 9.4 s | 2,001 in, 304 out |
| [word](skills/word/) | [`llama3.1-8b`](skills/word/llama3.1-8b/) | **14 of 28** | **6 of 6** | 8.1 s | 1,960 in, 311 out |
| [word](skills/word/) | [`granite3.3-8b`](skills/word/granite3.3-8b/) | **9 of 30** | **6 of 6** | 9.7 s | 2,078 in, 341 out |

"Stopped" counts the requests that asked for something the company does not allow (a file over a signed contract, in the payroll folder, on the public website): the gate stopped the call before it ran, whatever the model.

## How to read it

- `skills/<skill>/`: the skill and its count by model; under it one folder per model, and in it one folder per request with the request, the file and its first page.
- `companies/<company>/`: the invented company the requests come from, and what the agent may touch there.
- `data/index.json`: the same numbers for a program.

Everything here is written by a script from the runs; nothing is edited by hand. Companies, people, orders and amounts are invented.

## In plain words

This is a shop window of agents doing office work. For each job and each model you can open what was asked, what came out, how long it took, and how many times the agent was stopped from doing something it should not.
