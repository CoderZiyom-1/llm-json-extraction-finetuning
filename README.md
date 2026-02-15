# **llm-json-extraction-finetuning**

This project demonstrates fine-tuning a Large Language Model to extract structured JSON data from unstructured text inputs.

The goal is to convert messy real-world text into clean, machine-readable JSON format using a domain-adapted LLM.

**Problem Statement**

Extracting structured information from natural language is a common industry problem in:

1. Resume parsing

2. Invoice processing

3. Form automation

4. Customer support logs

4. Legal / medical documents

5. Traditional rule-based systems fail when text format changes.

This project solves that using LLM fine-tuning.

Instead of prompt engineering alone, the model is fine-tuned on a custom dataset to:

1. Understand context
2. Identify key entities
3. Output strict JSON format

**Custom training dataset:**

json_extraction_dataset_500.json

Contains:

Input: Natural language text

Output: Structured JSON

Example:

Input: John Doe lives in Bangalore and works at Infosys.


Output:

{
  "name": "John Doe",
  "location": "Bangalore",
  "company": "Infosys"
}

**Model Fine Tuning**

Fine-tuning pipeline implemented in:

Fine-Tuning.ipynb

Steps covered:

a. Dataset formatting

b. Instruction-style training

c. Model adaptation

d. Structured output alignment


**Model Configuration**

Modelfile


Defines:

A. Base model

B. Training parameters

C. Output format behavior

**Outcome**

The fine-tuned model:

Produces consistent JSON outputs

Handles noisy text inputs

Reduces hallucination vs prompt-only methods

**Use Cases**

1. Resume parsers

2. Lead extraction

3. Document automation

4. CRM data ingestion

4. AI workflow pipelines

**Tech Stack**

1. Python

2. LLM Fine-Tuning

3. JSON Structured Outputs

4. Prompt Formatting

5. Instruction Tuning

**Future improvements**

1. Increase dataset size

2. Multi-schema extraction

3. Real-time API deployment

This project demonstrates practical LLM adaptation for real-world automation tasks where structured data extraction is required at scale.
