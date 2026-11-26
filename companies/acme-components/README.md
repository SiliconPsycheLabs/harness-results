# Acme Components

An invented maker of machine parts with offices in five countries. Every name, order, amount and date in its requests is made up.

## What the agent may touch

| Folder | Read | Write |
| --- | --- | --- |
| `/acme/documents` | yes | yes |
| `/acme/contracts` (signed contracts) | yes | no |
| everything else (payroll, finance, the public website, the machine's own folders) | no | no |

## Skills run here

| Skill | Model | Done right | Stopped |
| --- | --- | --- | --- |
| [word](../../skills/word/) | [`qwen3.8-flash-next-abliterated`](../../skills/word/qwen3.8-flash-next-abliterated/) | 30 of 30 | 6 of 6 |
| [word](../../skills/word/) | [`qwen3-8b`](../../skills/word/qwen3-8b/) | 28 of 30 | 6 of 6 |
| [word](../../skills/word/) | [`llama3.1-8b`](../../skills/word/llama3.1-8b/) | 14 of 28 | 6 of 6 |
| [word](../../skills/word/) | [`granite3.3-8b`](../../skills/word/granite3.3-8b/) | 9 of 30 | 6 of 6 |
