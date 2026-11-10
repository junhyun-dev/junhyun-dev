# Junhyun Park · Data Engineer

I build and run data pipelines for a B2B data SaaS: Airflow and GCP jobs that collect each customer's data every day. Most of my recent work is on the cases where the batch succeeds but the data is wrong.

**Now:** finding missing data on the same day it goes missing, tracing a dashboard number back through the transformation models to the source rows, and letting AI agents work on that data under explicit checks. The domain I am going deep in is medical data (OMOP CDM).

## Projects

- **[fhir-indicator-line](https://github.com/junhyun-dev/fhir-indicator-line)**: two hospitals' records (synthetic FHIR and the MIMIC-IV demo) mapped to OMOP CDM 5.4 with dbt and DuckDB, giving the same blood pressure control rate from both. Adding the second hospital changed only its staging and code mapping. Every result is compared with expected outputs counted separately from the pipeline.
- **[minidelta](https://github.com/junhyun-dev/minidelta)**: Delta Lake reads, appends and partition-pruned counts in about 1,000 lines of Python, built in four iterations. Each iteration passed all of its expected results on the first implementation, ending at 1,229 (Delta's acceptance tests, Spark-written tables and my own contract tests).
- **[tiny-aya-korean-safety-steering](https://github.com/junhyun-dev/tiny-aya-korean-safety-steering)** (Lexsi AI Safety and Alignment Hackathon, November 2026): on the same 255 harmful requests, a small multilingual model gives the requested content about as often in Korean as in English, but warns where it would refuse in English. Inference-time steering turns those warnings into refusals, but with a stricter gate that keeps false refusals near their original level, Korean answers that give the requested content stay at 18%.

## Open source

- [docling-project/docling-serve #691](https://github.com/docling-project/docling-serve/pull/691), merged 2026-09: the UI's OCR switch was not passed to conversion requests. Fix and regression test.
- [storytold/photocraft #6882](https://github.com/storytold/photocraft/pull/6882), merged 2026-10: brought 18 Korean UI strings in line with the project's existing terms and tone.
- [OHDSI/dbt-synthea #154](https://github.com/OHDSI/dbt-synthea/issues/154): reported that `encounter_stop_date` always equals the start date (argument order in a `COALESCE`).

## How I work

I decide what to build, the design and the expected results. AI coding agents (Claude Code, Codex) write most of the code, and I check every change against expected results prepared beforehand.

Many agents share one repository in my workspace. For the Swarm Alignment Hackathon (Apart Research, November 2026) I measured how far their own logs show which agent changed what, across 38 days, 1,576 agent sessions and runs, and 7,986 commits: [agent-attribution-gaps](https://github.com/junhyun-dev/agent-attribution-gaps).

## Elsewhere

- Blog and project notes (Korean): [junhyun-engineering.vercel.app](https://junhyun-engineering.vercel.app)
- Databricks Certified Generative AI Engineer Associate (2026)
