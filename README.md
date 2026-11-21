# Junhyun Park · Data Engineer

I build and run data pipelines for a B2B data SaaS, and I am moving into AI agents that work on that data.

I started in RPA, automating work people did by hand and collecting ERP data with UiPath. Now I run Airflow and GCP jobs that collect each customer's data every day, find missing data on the day it goes missing, and trace a dashboard number back to its source rows. At work I built a prototype agent (Claude Agent SDK) that investigates failed transformations, while I make the final call.

**Now:** engineering with AI coding agents under explicit checks. I set the requirements, design and expected results; the agents write most of the code; I check every change against those expected results.

## Projects

- **[minidelta](https://github.com/junhyun-dev/minidelta)**: Delta Lake reads, appends and partition-pruned counts in about 1,000 lines of Python, built in four iterations. It ends at 1,229 expected results (Delta's acceptance tests, Spark-written tables and my own contract tests), all passing.

## Competitions (2026)

- Stanford Predictive AI Evaluation Competition: my report on predicting which benchmark items an AI model will solve was accepted at the NeurIPS 2026 PAIEC workshop, with a poster.
- [Lexsi AI Safety and Alignment Hackathon](https://github.com/junhyun-dev/tiny-aya-korean-safety-steering), top 25% of 369 teams in stage one: on the same 255 harmful requests, a small multilingual model gives the requested content about as often in Korean as in English, but warns where it would refuse in English.
- [SimulacraBench](https://github.com/junhyun-dev/simulacrabench) (NeurIPS 2026 competition): code and report source for my final submission, which predicts survey answer shares with a tabular foundation model used in context.
- [Swarm Alignment Hackathon](https://github.com/junhyun-dev/agent-attribution-gaps) (Apart Research): in my own repository, used for 38 days by 1,576 coding-agent sessions and runs (7,986 commits), how far the logs they already write show which agent changed what.

## Open source

- [docling-project/docling-serve #691](https://github.com/docling-project/docling-serve/pull/691), merged 2026-09: the UI's OCR switch was not passed to conversion requests. Fix and regression test.
- [storytold/photocraft #6882](https://github.com/storytold/photocraft/pull/6882), merged 2026-10: brought 18 Korean UI strings in line with the project's existing terms and tone.

## Elsewhere

- Blog and project notes (Korean): [junhyun-engineering.vercel.app](https://junhyun-engineering.vercel.app)
- Databricks Certified Generative AI Engineer Associate (2026)
