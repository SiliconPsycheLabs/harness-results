# Harness results: agents at work, with the count

A deterministic gate decides what an agent may do, and the harness makes the agent do the work. This repository shows the work: the request, the file the agent produced, and the count. Both are built by [Silicon Psyche Labs](https://splabs.io) for models a company owns.

Each skill is one thing an office needs done. Its page gives the whole recipe (model, harness version, the instructions, the limits) with what it cost in tokens and seconds, so the same result can be had again.

- **[accounts_payable](skills/accounts_payable/)**: The accounts payable job from start to end: read the supplier invoice that arrived as a PDF, enter it in the accounting application, write to the supplier that it was received and when it will be paid.
- **[browser](skills/browser/)**: Keep the supplier register up to date by working in the accounting application through its own pages, in a real browser: find the supplier, change its contact details, save.
- **[calendar](skills/calendar/)**: Book a meeting in the company calendar: find the first time when everyone is free and create the event with the right people.
- **[credit_control](skills/credit_control/)**: Credit control from start to end: find a customer's overdue invoices in the accounting application and send one payment reminder for each, to the customer's address on file.
- **[customer_support](skills/customer_support/)**: Customer support from start to end: a customer's message arrives, the agent finds the order in the database or the answer in the company's terms, proposes a refund that a person approves, and replies to the customer's address on file.
- **[database](skills/database/)**: Answer a business question from the company's database: write the query, read the rows, and save the answer with the query it comes from.
- **[doc_search](skills/doc_search/)**: Answer a colleague's question from the company's own documents: find the document, read it, and save the answer with the document it comes from.
- **[excel](skills/excel/)**: Write an Excel sheet (.xlsx) from an office request: a table with typed columns and a total row computed by a formula.
- **[filing](skills/filing/)**: File the documents that arrive: copy each one from the inbox into the right folder of the company's documents, and tidy folders by moving files.
- **[fx_rates](skills/fx_rates/)**: Convert a foreign-currency invoice into euros at the European Central Bank's reference rate of its date, by calling an outside service, and save the conversion with the address it comes from.
- **[mail](skills/mail/)**: Write and send a mail to a supplier or a colleague, with the attachments asked, only to addresses the company allows.
- **[meeting_desk](skills/meeting_desk/)**: Organising a meeting from start to end: find the first time when everyone is free, book it in the company calendar, write the agenda as a Word file and send the invitation to every attendee with the agenda attached.
- **[payment_run](skills/payment_run/)**: A payment run from start to end: pay a supplier's open invoices in the accounting application, each payment confirmed by a person of the administration, then send the supplier the payment advice.
- **[payments](skills/payments/)**: Prepare the payment of validated supplier bills in the accounting application: every payment waits for a person, and a bank account that is not the one on file is never paid.
- **[pdf](skills/pdf/)**: Read a supplier invoice in PDF and save its data as a record: supplier, number, dates, lines, net total and the page the total is on.
- **[powerpoint](skills/powerpoint/)**: Write a PowerPoint presentation (.pptx) from a colleague's request: a title slide and content slides with bullet points or a table.
- **[purchasing](skills/purchasing/)**: A purchase from start to end: read the suppliers' quotes, choose the one with the lower total, write the purchase order as an Excel sheet and send it to that supplier once the purchasing manager confirms.
- **[sales_report](skills/sales_report/)**: A sales report from start to end: take the figures from the company's database with one query, put them in an Excel sheet with a total, and send the sheet to the colleague who asked.
- **[supplier_bill](skills/supplier_bill/)**: Enter a supplier invoice in the accounting application as a draft bill: supplier, number, dates, lines and net total.
- **[web_search](skills/web_search/)**: Answer a question by searching an open encyclopedia on the web: find the page, read it, and save the answer with the address it comes from.
- **[word](skills/word/)**: Write a Word document (.docx) from an office request: letters, minutes, quotes, reports, notices, instructions.

| Skill | Model | Done right | Stopped by the company's limits | Time per request | Tokens per request |
| --- | --- | --- | --- | --- | --- |
| [accounts_payable](skills/accounts_payable/) | [`qwen3-8b`](skills/accounts_payable/qwen3-8b/) | **20 of 20** | **6 of 6** | 11.7 s | 11,014 in, 404 out |
| [accounts_payable](skills/accounts_payable/) | [`qwen3.8-flash-next-abliterated`](skills/accounts_payable/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 52.6 s | 11,073 in, 434 out |
| [accounts_payable](skills/accounts_payable/) | [`llama3.1-8b`](skills/accounts_payable/llama3.1-8b/) | **16 of 20** | **6 of 6** | 11.3 s | 10,953 in, 429 out |
| [accounts_payable](skills/accounts_payable/) | [`granite3.3-8b`](skills/accounts_payable/granite3.3-8b/) | **9 of 20** | **6 of 6** | 16.1 s | 13,739 in, 491 out |
| [browser](skills/browser/) | [`qwen3.8-flash-next-abliterated`](skills/browser/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 82.1 s | 5,786 in, 205 out |
| [browser](skills/browser/) | [`qwen3-8b`](skills/browser/qwen3-8b/) | **19 of 20** | **6 of 6** | 53.9 s | 6,819 in, 209 out |
| [browser](skills/browser/) | [`llama3.1-8b`](skills/browser/llama3.1-8b/) | **16 of 20** | **6 of 6** | 54.1 s | 6,852 in, 202 out |
| [browser](skills/browser/) | [`granite3.3-8b`](skills/browser/granite3.3-8b/) | **7 of 20** | **6 of 6** | 42.6 s | 6,058 in, 161 out |
| [calendar](skills/calendar/) | [`qwen3-8b`](skills/calendar/qwen3-8b/) | **20 of 20** | **6 of 6** | 8.0 s | 6,955 in, 287 out |
| [calendar](skills/calendar/) | [`qwen3.8-flash-next-abliterated`](skills/calendar/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 24.1 s | 6,991 in, 299 out |
| [calendar](skills/calendar/) | [`granite3.3-8b`](skills/calendar/granite3.3-8b/) | **19 of 20** | **6 of 6** | 8.5 s | 7,316 in, 327 out |
| [calendar](skills/calendar/) | [`llama3.1-8b`](skills/calendar/llama3.1-8b/) | **18 of 20** | **6 of 6** | 7.1 s | 6,829 in, 274 out |
| [credit_control](skills/credit_control/) | [`granite3.3-8b`](skills/credit_control/granite3.3-8b/) | **20 of 20** | **6 of 6** | 9.1 s | 3,910 in, 307 out |
| [credit_control](skills/credit_control/) | [`qwen3-8b`](skills/credit_control/qwen3-8b/) | **20 of 20** | **6 of 6** | 10.8 s | 3,771 in, 345 out |
| [credit_control](skills/credit_control/) | [`llama3.1-8b`](skills/credit_control/llama3.1-8b/) | **20 of 20** | **6 of 6** | 14.1 s | 6,740 in, 460 out |
| [credit_control](skills/credit_control/) | [`qwen3.8-flash-next-abliterated`](skills/credit_control/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 24.9 s | 3,887 in, 390 out |
| [customer_support](skills/customer_support/) | [`qwen3.8-flash-next-abliterated`](skills/customer_support/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 20.7 s | 8,223 in, 313 out |
| [customer_support](skills/customer_support/) | [`granite3.3-8b`](skills/customer_support/granite3.3-8b/) | **17 of 20** | **6 of 6** | 8.9 s | 7,578 in, 318 out |
| [customer_support](skills/customer_support/) | [`qwen3-8b`](skills/customer_support/qwen3-8b/) | **16 of 20** | **6 of 6** | 6.3 s | 7,192 in, 268 out |
| [customer_support](skills/customer_support/) | [`llama3.1-8b`](skills/customer_support/llama3.1-8b/) | **16 of 19** | **6 of 6** | 7.4 s | 6,417 in, 274 out |
| [database](skills/database/) | [`qwen3.8-flash-next-abliterated`](skills/database/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 19.8 s | 2,855 in, 310 out |
| [database](skills/database/) | [`qwen3-8b`](skills/database/qwen3-8b/) | **19 of 20** | **6 of 6** | 9.7 s | 2,838 in, 317 out |
| [database](skills/database/) | [`llama3.1-8b`](skills/database/llama3.1-8b/) | **18 of 20** | **6 of 6** | 7.3 s | 2,811 in, 282 out |
| [database](skills/database/) | [`granite3.3-8b`](skills/database/granite3.3-8b/) | **14 of 20** | **6 of 6** | 8.8 s | 4,399 in, 366 out |
| [doc_search](skills/doc_search/) | [`llama3.1-8b`](skills/doc_search/llama3.1-8b/) | **20 of 20** | **6 of 6** | 5.0 s | 3,902 in, 194 out |
| [doc_search](skills/doc_search/) | [`qwen3-8b`](skills/doc_search/qwen3-8b/) | **20 of 20** | **6 of 6** | 5.4 s | 3,800 in, 189 out |
| [doc_search](skills/doc_search/) | [`qwen3.8-flash-next-abliterated`](skills/doc_search/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 14.6 s | 3,643 in, 198 out |
| [doc_search](skills/doc_search/) | [`granite3.3-8b`](skills/doc_search/granite3.3-8b/) | **2 of 20** | **6 of 6** | 2.0 s | 1,610 in, 84 out |
| [excel](skills/excel/) | [`qwen3-8b`](skills/excel/qwen3-8b/) | **20 of 20** | **6 of 6** | 5.6 s | 1,924 in, 250 out |
| [excel](skills/excel/) | [`granite3.3-8b`](skills/excel/granite3.3-8b/) | **20 of 20** | **6 of 6** | 7.6 s | 1,991 in, 273 out |
| [excel](skills/excel/) | [`qwen3.8-flash-next-abliterated`](skills/excel/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 31.4 s | 2,020 in, 359 out |
| [excel](skills/excel/) | [`llama3.1-8b`](skills/excel/llama3.1-8b/) | **2 of 20** | **6 of 6** | 0.7 s | 801 in, 24 out |
| [filing](skills/filing/) | [`llama3.1-8b`](skills/filing/llama3.1-8b/) | **20 of 20** | **6 of 6** | 4.7 s | 3,400 in, 182 out |
| [filing](skills/filing/) | [`qwen3.8-flash-next-abliterated`](skills/filing/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 15.4 s | 3,657 in, 218 out |
| [filing](skills/filing/) | [`qwen3-8b`](skills/filing/qwen3-8b/) | **16 of 20** | **6 of 6** | 5.6 s | 3,485 in, 204 out |
| [filing](skills/filing/) | [`granite3.3-8b`](skills/filing/granite3.3-8b/) | **4 of 20** | **6 of 6** | 4.0 s | 2,540 in, 159 out |
| [fx_rates](skills/fx_rates/) | [`qwen3-8b`](skills/fx_rates/qwen3-8b/) | **20 of 20** | **6 of 6** | 5.0 s | 2,991 in, 223 out |
| [fx_rates](skills/fx_rates/) | [`qwen3.8-flash-next-abliterated`](skills/fx_rates/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 13.9 s | 2,980 in, 219 out |
| [fx_rates](skills/fx_rates/) | [`llama3.1-8b`](skills/fx_rates/llama3.1-8b/) | **19 of 20** | **6 of 6** | 4.9 s | 2,902 in, 188 out |
| [fx_rates](skills/fx_rates/) | [`granite3.3-8b`](skills/fx_rates/granite3.3-8b/) | **17 of 20** | **6 of 6** | 7.0 s | 3,164 in, 253 out |
| [mail](skills/mail/) | [`qwen3.8-flash-next-abliterated`](skills/mail/qwen3.8-flash-next-abliterated/) | **16 of 20** | **6 of 6** | 27.1 s | 2,141 in, 245 out |
| [mail](skills/mail/) | [`qwen3-8b`](skills/mail/qwen3-8b/) | **15 of 20** | **6 of 6** | 5.0 s | 2,111 in, 225 out |
| [mail](skills/mail/) | [`llama3.1-8b`](skills/mail/llama3.1-8b/) | **14 of 20** | **6 of 6** | 4.9 s | 2,088 in, 192 out |
| [mail](skills/mail/) | [`granite3.3-8b`](skills/mail/granite3.3-8b/) | **11 of 20** | **6 of 6** | 7.2 s | 2,266 in, 270 out |
| [meeting_desk](skills/meeting_desk/) | [`qwen3.8-flash-next-abliterated`](skills/meeting_desk/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 44.1 s | 17,362 in, 564 out |
| [meeting_desk](skills/meeting_desk/) | [`qwen3-8b`](skills/meeting_desk/qwen3-8b/) | **19 of 20** | **6 of 6** | 15.2 s | 17,250 in, 532 out |
| [meeting_desk](skills/meeting_desk/) | [`granite3.3-8b`](skills/meeting_desk/granite3.3-8b/) | **19 of 20** | **6 of 6** | 22.6 s | 21,053 in, 702 out |
| [meeting_desk](skills/meeting_desk/) | [`llama3.1-8b`](skills/meeting_desk/llama3.1-8b/) | **18 of 20** | **6 of 6** | 14.3 s | 18,663 in, 516 out |
| [payment_run](skills/payment_run/) | [`qwen3-8b`](skills/payment_run/qwen3-8b/) | **20 of 20** | **6 of 6** | 9.5 s | 6,994 in, 359 out |
| [payment_run](skills/payment_run/) | [`llama3.1-8b`](skills/payment_run/llama3.1-8b/) | **20 of 20** | **6 of 6** | 10.3 s | 7,345 in, 316 out |
| [payment_run](skills/payment_run/) | [`qwen3.8-flash-next-abliterated`](skills/payment_run/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 22.4 s | 7,084 in, 368 out |
| [payment_run](skills/payment_run/) | [`granite3.3-8b`](skills/payment_run/granite3.3-8b/) | **19 of 20** | **6 of 6** | 13.6 s | 8,069 in, 405 out |
| [payments](skills/payments/) | [`llama3.1-8b`](skills/payments/llama3.1-8b/) | **20 of 20** | **6 of 6** | 8.2 s | 3,612 in, 193 out |
| [payments](skills/payments/) | [`granite3.3-8b`](skills/payments/granite3.3-8b/) | **20 of 20** | **6 of 6** | 8.4 s | 3,431 in, 219 out |
| [payments](skills/payments/) | [`qwen3-8b`](skills/payments/qwen3-8b/) | **20 of 20** | **6 of 6** | 9.9 s | 3,289 in, 234 out |
| [payments](skills/payments/) | [`qwen3.8-flash-next-abliterated`](skills/payments/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 39.9 s | 3,326 in, 244 out |
| [pdf](skills/pdf/) | [`qwen3-8b`](skills/pdf/qwen3-8b/) | **20 of 20** | **6 of 6** | 5.5 s | 3,204 in, 246 out |
| [pdf](skills/pdf/) | [`qwen3.8-flash-next-abliterated`](skills/pdf/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 31.1 s | 3,211 in, 290 out |
| [pdf](skills/pdf/) | [`granite3.3-8b`](skills/pdf/granite3.3-8b/) | **17 of 20** | **6 of 6** | 7.1 s | 3,334 in, 262 out |
| [pdf](skills/pdf/) | [`llama3.1-8b`](skills/pdf/llama3.1-8b/) | **13 of 20** | **6 of 6** | 6.1 s | 3,116 in, 215 out |
| [powerpoint](skills/powerpoint/) | [`granite3.3-8b`](skills/powerpoint/granite3.3-8b/) | **20 of 20** | **6 of 6** | 8.6 s | 2,349 in, 332 out |
| [powerpoint](skills/powerpoint/) | [`qwen3.8-flash-next-abliterated`](skills/powerpoint/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 29.4 s | 2,230 in, 349 out |
| [powerpoint](skills/powerpoint/) | [`qwen3-8b`](skills/powerpoint/qwen3-8b/) | **18 of 20** | **6 of 6** | 7.4 s | 2,205 in, 274 out |
| [powerpoint](skills/powerpoint/) | [`llama3.1-8b`](skills/powerpoint/llama3.1-8b/) | **17 of 20** | **6 of 6** | 6.7 s | 2,166 in, 271 out |
| [purchasing](skills/purchasing/) | [`qwen3.8-flash-next-abliterated`](skills/purchasing/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 36.0 s | 10,825 in, 440 out |
| [purchasing](skills/purchasing/) | [`llama3.1-8b`](skills/purchasing/llama3.1-8b/) | **14 of 20** | **6 of 6** | 10.3 s | 10,451 in, 370 out |
| [purchasing](skills/purchasing/) | [`qwen3-8b`](skills/purchasing/qwen3-8b/) | **12 of 19** | **5 of 5** | 13.1 s | 10,507 in, 423 out |
| [purchasing](skills/purchasing/) | [`granite3.3-8b`](skills/purchasing/granite3.3-8b/) | **0 of 20** | **6 of 6** | 20.3 s | 16,291 in, 726 out |
| [sales_report](skills/sales_report/) | [`qwen3-8b`](skills/sales_report/qwen3-8b/) | **20 of 20** | **6 of 6** | 8.8 s | 8,415 in, 388 out |
| [sales_report](skills/sales_report/) | [`qwen3.8-flash-next-abliterated`](skills/sales_report/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 27.2 s | 8,436 in, 380 out |
| [sales_report](skills/sales_report/) | [`llama3.1-8b`](skills/sales_report/llama3.1-8b/) | **17 of 20** | **6 of 6** | 9.3 s | 8,194 in, 348 out |
| [sales_report](skills/sales_report/) | [`granite3.3-8b`](skills/sales_report/granite3.3-8b/) | **11 of 17** | **6 of 6** | 16.6 s | 13,133 in, 571 out |
| [supplier_bill](skills/supplier_bill/) | [`qwen3-8b`](skills/supplier_bill/qwen3-8b/) | **20 of 20** | **6 of 6** | 7.5 s | 3,264 in, 221 out |
| [supplier_bill](skills/supplier_bill/) | [`qwen3.8-flash-next-abliterated`](skills/supplier_bill/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 22.3 s | 3,271 in, 231 out |
| [supplier_bill](skills/supplier_bill/) | [`llama3.1-8b`](skills/supplier_bill/llama3.1-8b/) | **19 of 20** | **6 of 6** | 6.0 s | 3,174 in, 202 out |
| [supplier_bill](skills/supplier_bill/) | [`granite3.3-8b`](skills/supplier_bill/granite3.3-8b/) | **2 of 20** | **6 of 6** | 1.4 s | 2,131 in, 55 out |
| [web_search](skills/web_search/) | [`llama3.1-8b`](skills/web_search/llama3.1-8b/) | **20 of 20** | **6 of 6** | 4.6 s | 4,445 in, 164 out |
| [web_search](skills/web_search/) | [`qwen3.8-flash-next-abliterated`](skills/web_search/qwen3.8-flash-next-abliterated/) | **20 of 20** | **6 of 6** | 12.1 s | 4,573 in, 178 out |
| [web_search](skills/web_search/) | [`qwen3-8b`](skills/web_search/qwen3-8b/) | **19 of 20** | **6 of 6** | 3.7 s | 4,500 in, 164 out |
| [web_search](skills/web_search/) | [`granite3.3-8b`](skills/web_search/granite3.3-8b/) | **0 of 20** | **6 of 6** | 2.0 s | 1,561 in, 71 out |
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
