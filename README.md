# Ticket_classification_using_fewshot_prompting_using_Gemini_LLM
Classify IT support tickets using few-shot prompts with Gemini models on Google Cloud Vertex AI.

---

## Overview

This project demonstrates how to classify IT support queries using Google Cloud's **Vertex AI Gemini models**. It uses a `.txt` file of few-shot examples to construct a prompt and runs inference via Python in Google Colab. Example queries include:

* "Can't log into the student portal"
* "Wi-Fi not working in the dorm"

---

##  Getting Started

### Prerequisites

* Python 3.x (via Google Colab)
* Google Cloud account with Vertex AI enabled
* Gemini model access (`gemini-2.0-flash-001` or newer)
* `google-cloud-aiplatform` Python SDK
  

---

## Project Structure

```bash
vertexai-ticket-classifier/
├── sample_input_data.csv           # Few-shot examples (input/output pairs)
├── Few_shots_prompting_using_gemini.ipynb         # Notebook for running Gemini inference
├── README.md                     # This file

```

---

## 📄 Prompt File Format

Contents of `sample_input_data.csv`:

```
Inline: My laptop won't connect to the Wi-Fi
label: CTS

Inline: I can't log into the student portal
label: CTS Campus

```

---

##  How It Works

###  Step 1: Upload Prompt File


###  Step 2: Build Prompt with New Input


###  Step 3: Call Gemini Model

---

##  Sample Input/Output

**Input:**

```
projector in frye hall is not working
```

**Output:**

```
 Classroom support
```

---

##  Use Cases

* Classifying IT helpdesk tickets
* Rapid prototyping for LLM-based classification
* Few-shot prompting with real-world data

