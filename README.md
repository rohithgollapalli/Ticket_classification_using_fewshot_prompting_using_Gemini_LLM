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
```

---

##  Project Structure

```bash
vertexai-ticket-classifier/
├── prompt_examples.txt           # Few-shot examples (input/output pairs)
├── inference_colab.ipynb         # Notebook for running Gemini inference
├── README.md                     # This file
└── requirements.txt              # Optional dependency file
```

---

## 📄 Prompt File Format

Contents of `prompt_examples.txt`:

```
Input: My laptop won't connect to the Wi-Fi
Output: Network Issues

Input: I can't log into the student portal
Output: Portal Access

Input: Forgot my email password
Output: Account & Login
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

---

##  Future Improvements

* Add support for dynamic prompts via web UI
* Fine-tune with larger custom datasets
* Automate prompt generation from CSV
