# MedFact Agent: AI-Powered Medical Fact Checker

Building AI course project

## Summary

MedFact Agent is an AI-powered tool that uses large language models and agentic workflows to provide trustworthy, fact-checked medical information. It searches trusted sources in real-time, compiles concise summaries, and highlights common myths or misinformation.

## Background

Online medical misinformation is a huge and growing problem. Many people search symptoms or conditions online and fall into a rabbit hole of inaccurate or misleading content. This can cause unnecessary anxiety or, worse, lead to poor health decisions.

MedFact Agent aims to solve this by:
* Automatically searching only peer-reviewed, trusted medical sources
* Filtering out noise and surfacing reliable, user-friendly summaries
* Debunking popular myths related to the queried condition

I was personally motivated by the number of friends and family who’ve misinterpreted symptoms using random health blogs or forums. This tool aims to make high-quality health knowledge more accessible and less intimidating.

## How is it used?

When a user inputs a question about a medical condition or symptom (e.g., "Is a persistent dry cough a sign of something serious?"), the LLM agent:

1. Uses the Google Search API to find up-to-date and trustworthy sources (e.g., Mayo Clinic, WebMD, CDC, peer-reviewed articles).
2. Summarizes findings clearly and concisely.
3. Cross-checks for common myths or misinformation and lists them separately with clarifications.
4. Presents everything in an easy-to-read UI.

This tool can be used by:
* Curious individuals looking to better understand their symptoms.
* Caregivers who want to verify advice.
* Educators or content creators who need reliable summaries of medical topics.

It’s most useful in everyday scenarios where someone would otherwise turn to Google or forums for health advice.


## Data sources and AI methods

The data is sourced in real-time using:
* Google Search API
* Whitelisted sources (e.g., Mayo Clinic, WebMD, MedlinePlus, PubMed, WHO)

AI methods include:
* A multi-agent architecture:  
  - **Search Agent**: Gathers relevant, reputable sources
  - **Summary Agent**: Extracts the key facts  
  - **Mythbuster Agent**: Identifies misinformation & debunks it  
  - **UI Agent**: Organizes and presents the output in a user-friendly format

LLMs (like GPT-4 or Claude) are used with retrieval-augmented generation (RAG) to ensure factual accuracy and citation integrity.

## Challenges

What the project doesn’t solve (yet):
* It does not replace medical professionals.
* It may miss rare or emerging conditions not yet well-documented.
* It cannot provide a diagnosis or personalized treatment recommendations.

Ethical considerations:
* Must ensure outputs are traceable to real sources.
* Must emphasize that this is not a substitute for medical advice.
* Risk of misuse in serious or emergency situations if not properly disclaimered.

## What next?

To scale this project:
* A real-time front-end (React/Next.js) with clean, calming UI
* Better integration with vetted APIs from WHO, CDC, etc.
* Reinforcement learning with feedback from health professionals
* Expansion into multilingual support

I’d need help from:
* Web/app developers
* Healthcare experts for fact-checking
* UX designers to optimize the experience for accessibility

## Acknowledgments

* Thanks to the University of Helsinki and Reaktor for the Building AI course!
