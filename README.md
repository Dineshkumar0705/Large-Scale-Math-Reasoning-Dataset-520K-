# **Large-Scale Math Reasoning Dataset (520K)**

A large-scale, high-quality synthetic mathematics dataset containing over 520,000 verified math problems, spanning from basic arithmetic to Olympiad-level reasoning.

This dataset is designed for mathematical reasoning, LLM training & fine-tuning, symbolic reasoning research, and educational AI systems.


# Overview

The Large-Scale Math Reasoning Dataset (520K) is a unified corpus of math problems generated programmatically using a deterministic, template-driven pipeline.

It covers the full spectrum of difficulty:
	•	Basic school-level arithmetic
	•	Intermediate algebra and number theory
	•	Geometry and trigonometry
	•	Advanced Olympiad-level mathematics

Every problem includes:
	•	A clear problem prompt
	•	Step-by-step reasoning
	•	A verified final answer
	•	Rich metadata for filtering and analysis



# Dataset Contents
	•	Total Problems: ~520,416
	•	Format: JSON Lines (.jsonl)
	•	Files:
	•	dataset.jsonl — complete dataset
	•	README.md — documentation

Each line in the dataset is a single JSON object.


# Problem Schema

Each record contains the following fields:
	•	id — unique SHA-256 hash
	•	problem_id — template-based unique identifier
	•	chapter — topic or chapter name
	•	prompt — math problem text
	•	response — step-by-step reasoning ending with final answer
	•	answer — non-negative integer result
	•	metadata:
	•	difficulty (basic / medium / hard / olympiad)
	•	template
	•	source
	•	timestamp



# Chapter-wise Distribution (Approx.)

Quadratics — 115,629
Algebraic Expressions — 83,581
Linear Equations — 68,359
Factors & Multiples — 59,861
Modular Arithmetic — 53,213
Integers — 40,699
Natural Numbers — 37,511
Arithmetic Sequences — 8,252
Polynomials — 5,439
Geometry – Lines & Angles — 3,383
Divisibility & Modular Logic — 1,196

Olympiad Algebra — 14,680
Olympiad Number Theory — 15,296
Olympiad Geometry — 4,404
Olympiad Combinatorics — 3,894
Olympiad Trigonometry — 5,019

Total (Approx.) — 520,416



# Data Quality Guarantees

Every record in this dataset satisfies the following:
	•	Fully deduplicated (by ID and prompt)
	•	Arithmetic consistency verified
	•	No negative answers
	•	Deterministic generation
	•	Unique IDs per problem
	•	Clean and normalized schema



# Generation Pipeline (High-Level)
	1.	Template-driven problem generators
	2.	Parameterized value sampling
	3.	Deterministic expansion
	4.	Arithmetic validation
	5.	Removal of negative or invalid answers
	6.	Deduplication by ID and prompt
	7.	Schema normalization
	8.	Final audit and export

No external datasets, textbooks, or copyrighted sources were used.



# Intended Use Cases
	•	Mathematical reasoning model training
	•	LLM fine-tuning (math & reasoning)
	•	Olympiad-level AI benchmarks
	•	Curriculum-aligned educational systems
	•	Research in numerical & symbolic reasoning
	•	Kaggle notebooks and competitions



# Usage Notes
	•	Answers are non-negative integers only
	•	Problems range from basic to Olympiad level
	•	Dataset is fully synthetic
	•	Suitable for research and educational use



# License

Creative Commons Attribution 4.0 International (CC BY 4.0)

You are free to share, adapt, and use commercially, provided proper attribution is given.



# Citation

APA citation:

Dinesh Kumar Thiyagarajan (2025).
Large-Scale Math Reasoning Dataset (520K).
Kaggle.
https://doi.org/10.34740/kaggle/dsv/14354544


# Author

Dinesh Kumar Thiyagarajan
Independent AI Researcher
Focus areas: Mathematical reasoning, synthetic data generation, symbolic AI


# Future Plans
	•	Model training benchmarks
	•	Difficulty-wise dataset splits
	•	Curriculum-aligned subsets
	•	AIMO-style evaluation notebooks


# Acknowledgement

If you find this dataset useful:
	•	Cite the dataset
	•	Share your work
	•	Build models on top of it

Happy reasoning 🧮🔥

