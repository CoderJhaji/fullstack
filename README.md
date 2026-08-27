# TrustHire

### AI-Powered Fake Job & Offer Letter Detection

TrustHire is an AI-powered platform designed to protect students from fake job offers, fraudulent internships, scam emails, and fake offer letters.

Students often receive job and internship opportunities through emails, social media, and online platforms. However, existing job portals mainly focus on listing opportunities and may not verify an offer after it is issued. TrustHire addresses this gap by analyzing job-related text and identifying patterns commonly associated with fraudulent opportunities.

## Problem

Students frequently encounter fake internships and job offers online. Common warning signs include:

* Unrealistic salary promises
* Requests for payment or registration fees
* Urgent or threatening language
* Lack of an interview process
* Suspicious or public email domains
* Reused scam templates
* Fraudulent or suspicious offer letters

Existing systems generally do not provide students with a dedicated scam risk score, offer-letter verification, behavioral scam detection, or a centralized way to identify suspicious opportunities.

## Our Solution

TrustHire analyzes the content of job offers, internship postings, emails, and offer letters using a combination of Natural Language Processing, machine learning, and behavioral indicators.

The system:

1. Accepts an offer letter or email text as input.
2. Extracts and preprocesses the relevant text.
3. Analyzes linguistic and behavioral patterns.
4. Predicts the probability that the opportunity is fraudulent.
5. Identifies important scam indicators.
6. Displays a risk level and explains why the opportunity may be suspicious.

The output provides students with a simple and understandable assessment instead of requiring them to manually identify scam indicators.

## Key Features

### Fake Offer Letter Detection

Upload an offer letter and analyze its content for suspicious patterns and potential fraud indicators.

### Fake Email Detection

Analyze recruitment emails and identify indicators such as payment requests, urgency, suspicious domains, and scam-like language.

### Scam Risk Score

TrustHire provides a scam probability score to help students quickly understand the potential risk associated with an opportunity.

### Risk Classification

Opportunities are categorized into:

* **Low Risk** — relatively safe indicators
* **Medium Risk** — suspicious indicators detected
* **High Risk** — strong indicators of a potential scam

### Red Flag Detection

The system can identify patterns such as:

* Payment or fee requests
* Unrealistic salary claims
* Urgency tactics
* Absence of interviews
* Public/non-corporate email domains
* Suspicious linguistic patterns
* Repetitive scam templates

TrustHire combines textual analysis with behavioral indicators instead of relying only on keyword matching.

### AI-Powered Explanation

After detecting potential risk factors, the system provides a human-readable explanation of why an offer may be suspicious and gives safety-oriented guidance.

## Technology Stack

### Frontend

* HTML
* CSS
* JavaScript
* Web-based user interface

### Backend

* Backend API for processing detection requests
* Text extraction and preprocessing
* ML-based scam detection

### Database

* **Supabase** — used as the project's database/backend service
* Supabase Free Tier is used for the project

### Machine Learning

TrustHire uses an ML-based detection approach for identifying fraudulent job opportunities. The model analyzes textual and behavioral features to classify opportunities according to their risk level.

### AI Explanation Layer

* OpenAI/LLM-based explanation layer
* Converts detected risk factors into easy-to-understand explanations and safety tips.

## System Workflow

```text
User
  │
  ├── Upload Offer Letter
  │
  └── Paste Email / Job Text
          │
          ▼
     Backend API
          │
          ▼
   Text Extraction
          │
          ▼
  Text Preprocessing
          │
          ▼
   ML Scam Detection
          │
          ▼
   Scam Probability
          │
          ▼
   Risk Classification
   ┌──────┼─────────┐
   ▼      ▼         ▼
  Low   Medium     High
          │
          ▼
     Red Flags
          │
          ▼
   AI Explanation
          │
          ▼
   Student Dashboard
```

## Detection Approach

TrustHire uses a hybrid approach combining linguistic and behavioral analysis.

### Linguistic Analysis

The system analyzes:

* Writing style
* Tone
* Sentence patterns
* Suspicious terminology
* Repetitive templates
* Unrealistic claims

### Behavioral Analysis

The system also considers behavioral signals such as:

* Payment requests
* No interview process
* Urgency
* Public email domains
* Suspicious recruitment behavior

Combining these signals helps provide more meaningful detection than simple keyword matching.

## Database

TrustHire uses **Supabase Free Tier** for storing application data and supporting the backend.

Supabase can be used to manage:

* User information
* Detection history
* Scam analysis results
* Risk scores
* Detected red flags

## Project Structure

```text
TrustHire/
│
├── frontend/
│   ├── index.html
│   ├── style.css
│   └── script.js
│
├── backend/
│   ├── api/
│   ├── models/
│   └── services/
│
├── ml/
│   ├── model/
│   └── preprocessing/
│
├── README.md
└── requirements.txt
```

> The exact folder structure may differ depending on your implementation.

## Why TrustHire?

Traditional job platforms primarily help users discover job opportunities. TrustHire focuses on an additional and important step: **helping students determine whether an opportunity they have received is trustworthy.**

Instead of simply showing a job listing, TrustHire gives users:

**Detection → Risk Score → Red Flags → Explanation → Safer Decision**

## Future Scope

TrustHire can be extended into a more proactive fraud-prevention platform.

### Screenshot-Based Detection

Users could upload screenshots of chats or emails. OCR could extract the text and analyze it for scam patterns.

### Real-Time Browser Protection

A browser extension could analyze job postings while users browse recruitment websites and warn them about suspicious listings.

### Behavioral ML Fraud Detection

Advanced machine learning could detect scam behavior even when scammers change names, email addresses, or domains.

### Scam Template Fingerprinting

The system could identify repeated fraudulent document and message templates used by scammers.

### Scam Network Intelligence

Future versions could connect suspicious emails, phone numbers, and payment identifiers to identify larger organized scam networks.

## Team

**Team Name:** TrustHire

**Team Members:**

* Shalini Kumari
* Muskan Gautam
* Muskan 

## Disclaimer

TrustHire is intended to assist students in identifying potentially fraudulent opportunities. A detection result should be treated as a risk assessment rather than a guarantee that an opportunity is genuine or fraudulent.

