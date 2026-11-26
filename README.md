# Harness results: agents at work, with the count

A deterministic gate decides what an agent may do, and the harness makes the agent do the work. This repository shows the work: the request, the file the agent produced, and the count. Both are built by [Silicon Psyche Labs](https://splabs.io) for models a company owns.

Each skill is one thing an office needs done. Its page gives the whole recipe (model, harness version, the instructions, the limits) with what it cost in tokens and seconds, so the same result can be had again.

- **[excel](skills/excel/)**: Write an Excel sheet (.xlsx) from an office request: a table with typed columns and a total row computed by a formula.
- **[mail](skills/mail/)**: Write and send a mail to a supplier or a colleague, with the attachments asked, only to addresses the company allows.
- **[payments](skills/payments/)**: Prepare the payment of validated supplier bills in the accounting application: every payment waits for a person, and a bank account that is not the one on file is never paid.
- **[pdf](skills/pdf/)**: Read a supplier invoice in PDF and save its data as a record: supplier, number, dates, lines, net total and the page the total is on.
- **[supplier_bill](skills/supplier_bill/)**: Enter a supplier invoice in the accounting application as a draft bill: supplier, number, dates, lines and net total.
- **[word](skills/word/)**: Write a Word document (.docx) from an office request: letters, minutes, quotes, reports, notices, instructions.

| Skill | Model | Done right | Stopped by the company's limits | Time per request | Tokens per request |
| --- | --- | --- | --- | --- | --- |
| [excel](skills/excel/) | [`qwen3-8b`](skills/excel/qwen3-8b/) | **20 of 20** | **6 of 6** | 5.6 s | 1,924 in, 250 out |
| [excel](skills/excel/) | [`granite3.3-8b`](skills/excel/granite3.3-8b/) | **20 of 20** | **6 of 6** | 7.6 s | 1,991 in, 273 out |
| [excel](skills/excel/) | [`qwen3.8-flash-next-abliterated`](skills/excel/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 31.4 s | 2,020 in, 359 out |
| [excel](skills/excel/) | [`llama3.1-8b`](skills/excel/llama3.1-8b/) | **2 of 20** | **6 of 6** | 0.7 s | 801 in, 24 out |
| [mail](skills/mail/) | [`qwen3.8-flash-next-abliterated`](skills/mail/qwen3.8-flash-next-abliterated/) | **16 of 20** | **6 of 6** | 27.1 s | 2,141 in, 245 out |
| [mail](skills/mail/) | [`qwen3-8b`](skills/mail/qwen3-8b/) | **15 of 20** | **6 of 6** | 5.0 s | 2,111 in, 225 out |
| [mail](skills/mail/) | [`llama3.1-8b`](skills/mail/llama3.1-8b/) | **14 of 20** | **6 of 6** | 4.9 s | 2,088 in, 192 out |
| [mail](skills/mail/) | [`granite3.3-8b`](skills/mail/granite3.3-8b/) | **11 of 20** | **6 of 6** | 7.2 s | 2,266 in, 270 out |
| [payments](skills/payments/) | [`llama3.1-8b`](skills/payments/llama3.1-8b/) | **20 of 20** | **6 of 6** | 8.2 s | 3,612 in, 193 out |
| [payments](skills/payments/) | [`granite3.3-8b`](skills/payments/granite3.3-8b/) | **20 of 20** | **6 of 6** | 8.4 s | 3,431 in, 219 out |
| [payments](skills/payments/) | [`qwen3-8b`](skills/payments/qwen3-8b/) | **20 of 20** | **6 of 6** | 9.9 s | 3,289 in, 234 out |
| [payments](skills/payments/) | [`qwen3.8-flash-next-abliterated`](skills/payments/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 39.9 s | 3,326 in, 244 out |
| [pdf](skills/pdf/) | [`qwen3-8b`](skills/pdf/qwen3-8b/) | **20 of 20** | **6 of 6** | 5.5 s | 3,204 in, 246 out |
| [pdf](skills/pdf/) | [`qwen3.8-flash-next-abliterated`](skills/pdf/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 31.1 s | 3,211 in, 290 out |
| [pdf](skills/pdf/) | [`granite3.3-8b`](skills/pdf/granite3.3-8b/) | **17 of 20** | **6 of 6** | 7.1 s | 3,334 in, 262 out |
| [pdf](skills/pdf/) | [`llama3.1-8b`](skills/pdf/llama3.1-8b/) | **13 of 20** | **6 of 6** | 6.1 s | 3,116 in, 215 out |
| [supplier_bill](skills/supplier_bill/) | [`qwen3-8b`](skills/supplier_bill/qwen3-8b/) | **20 of 20** | **6 of 6** | 7.5 s | 3,264 in, 221 out |
| [supplier_bill](skills/supplier_bill/) | [`qwen3.8-flash-next-abliterated`](skills/supplier_bill/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 22.3 s | 3,271 in, 231 out |
| [supplier_bill](skills/supplier_bill/) | [`llama3.1-8b`](skills/supplier_bill/llama3.1-8b/) | **19 of 20** | **6 of 6** | 6.0 s | 3,174 in, 202 out |
| [supplier_bill](skills/supplier_bill/) | [`granite3.3-8b`](skills/supplier_bill/granite3.3-8b/) | **2 of 20** | **6 of 6** | 1.4 s | 2,131 in, 55 out |
| [word](skills/word/) | [`qwen3.8-flash-next-abliterated`](skills/word/qwen3.8-flash-next-abliterated/) | **30 of 30** | **6 of 6** | 27.6 s | 2,046 in, 370 out |
| [word](skills/word/) | [`qwen3-8b`](skills/word/qwen3-8b/) | **28 of 30** | **6 of 6** | 9.4 s | 2,001 in, 304 out |
| [word](skills/word/) | [`llama3.1-8b`](skills/word/llama3.1-8b/) | **14 of 28** | **6 of 6** | 8.1 s | 1,960 in, 311 out |
| [word](skills/word/) | [`granite3.3-8b`](skills/word/granite3.3-8b/) | **9 of 30** | **6 of 6** | 9.7 s | 2,078 in, 341 out |

"Stopped" counts the requests that asked for something the company does not allow (a file over a signed contract, a new supplier added to the register, a supplier's bank account changed): the gate stopped the call before it ran, whatever the model.

## How to read it

- `skills/<skill>/`: the skill and its count by model; under it one folder per model, and in it one folder per request with the request, the result (a file and its first page, or the application's screen) and the record of the run.
- `companies/<company>/`: the invented company the requests come from, and what the agent may touch there.
- `data/index.json`: the same numbers for a program.

Everything here is written by a script from the runs; nothing is edited by hand. Companies, people, orders and amounts are invented.

## In plain words

This is a shop window of agents doing office work. For each job and each model you can open what was asked, what came out, how long it took, and how many times the agent was stopped from doing something it should not.
