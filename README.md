# Adaptive Fraction Tutor

An AI-driven adaptive learning system that estimates a student's mastery of 
fractions, identifies weaknesses, and personalises practice — instead of 
giving every learner the same fixed sequence.

## Problem

Children aged 9-12 have very different levels of understanding, but 
conventional digital practice often gives everyone the same learning path.

## Core Question

Can adaptive, AI-driven instruction improve fraction mastery outcomes 
compared to a fixed learning sequence?

## Target Learners

Ages 9-12, learning fractions:
- Understanding fractions
- Equivalent fractions
- Comparing fractions
- Adding fractions
- Subtracting fractions
- Fraction word problems

## System Architecture

Diagnostic assessment
↓
Learner model (Bayesian Knowledge Tracing) — estimates mastery per skill
↓
Adaptive engine — selects next question/activity
↓
Question + explanation (RAG + LLM)
↓
Learner response
↓
Answer/misconception analysis
↓
Update mastery estimate


## Approach

- **Learner model:** Bayesian Knowledge Tracing (BKT) — tracks probability 
  of skill mastery, updates after each response.
- **Adaptive engine:** selects next question based on current mastery 
  estimates.
- **RAG:** grounds explanations in curriculum material rather than 
  free-form LLM output.
- **Evaluation:** adaptive sequence vs fixed sequence, compared on 
  mastery prediction accuracy and questions needed to reach mastery.

## Status

🚧 In progress — currently building the learner model.

## Scope

Not included in this version: full math curriculum, multiple age groups, 
voice interface, real classroom data, computer vision.

## Why This Project

Built to demonstrate applied AI/ML skills (personalisation, evaluation, 
LLMs, RAG) in an education context, with a focus on grounded, measurable 
learning outcomes rather than a generic chatbot.
