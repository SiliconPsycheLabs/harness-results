# Skill: word

Write a Word document (.docx) from an office request: letters, minutes, quotes, reports, notices, instructions.

The agent does not write a program to make the file. It fills the fields of a tool, and a program of ours writes the file, the same way every time. Before the tool runs, the call goes to the gate: a deterministic check on the fields and on where the file would be written.

## The count by model

The same requests, the same rules, the same instructions; only the model changes.

| Model | Done right | Stopped by the company's limits | Written outside with the gate only watching | Time per request | Tokens per request | Runs ended on an error | Skill version |
| --- | --- | --- | --- | --- | --- | --- | --- |
| [`qwen3.8-flash-next-abliterated`](qwen3.8-flash-next-abliterated/) | **30 of 30** | **6 of 6** | 6 of 6 | 27.6 s | 2,046 in, 370 out | 0 of 72 | 0.1.1 |
| [`qwen3-8b`](qwen3-8b/) | **28 of 30** | **6 of 6** | 6 of 6 | 9.4 s | 2,001 in, 304 out | 0 of 72 | 0.1.1 |
| [`llama3.1-8b`](llama3.1-8b/) | **14 of 28** | **6 of 6** | 5 of 6 | 8.1 s | 1,960 in, 311 out | 4 of 72 | 0.1.0 |
| [`granite3.3-8b`](granite3.3-8b/) | **9 of 30** | **6 of 6** | 6 of 6 | 9.7 s | 2,078 in, 341 out | 0 of 72 | 0.1.1 |

"Done right" is read from the file by a program (title, every name, date and amount, the structure asked) and counts the requests whose run did not end on an error; it does not judge the prose. The seconds were measured on servers that were doing other work at the same time, so they say what it took that day, not the model's own speed.

## In plain words

The same office job was given to several open models. The rules stopped every forbidden save whatever the model; how many documents came out right depends on the model, and the table says by how much.
