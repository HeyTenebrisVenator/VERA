# VERA

**Vulnerability Evidence Reasoning Architecture**

<img width="400" alt="vera" src="https://github.com/user-attachments/assets/7205006a-ee25-437c-8025-50ffc2cf9314" />

VERA is a research project focused on reducing false positives in automated vulnerability detection through evidence correlation, machine learning, and continuous learning techniques.

The project investigates how artificial intelligence can improve the reliability of security scanners by analyzing multiple sources of evidence before classifying a finding as a valid vulnerability.

Rather than relying solely on payload matching or signature-based detection, VERA evaluates positive and negative evidence, contextual information, application behavior, technology fingerprints, payload history, and human feedback to estimate the confidence of a finding.

---

## Research Motivation

Modern security scanners are capable of discovering thousands of potential vulnerabilities. However, a significant portion of these findings are false positives, requiring extensive manual validation by security professionals.

This challenge affects:

* Vulnerability assessment platforms
* Bug bounty programs
* Security operations teams
* Small organizations with limited security resources

VERA aims to address this problem by introducing an intelligent evidence correlation architecture capable of learning from previous observations and improving validation accuracy over time.

---

## Research Question

Can evidence correlation and machine learning reduce false positives in automated vulnerability detection systems without significantly reducing detection capability?

---

## Objectives

The primary objectives of VERA are:

* Reduce false positives in automated vulnerability detection.
* Improve confidence estimation for vulnerability findings.
* Learn from historical payload performance.
* Analyze the influence of Web Application Firewalls (WAFs).
* Learn from human-assisted validation.
* Provide explainable security decisions.
* Evaluate the effectiveness of deep learning for evidence classification.

---

## Target Vulnerabilities

The initial research focuses on five vulnerability categories:

* Cross-Site Scripting (XSS)
* Server-Side Template Injection (SSTI)
* SQL Injection (SQLi)
* Insecure Direct Object References (IDOR)
* Remote Code Execution (RCE)

These vulnerabilities were selected because they represent distinct classes of security issues and frequently generate false positives in automated scanners.

---

## Core Components

### Evidence Engine

Collects and analyzes security evidence generated during testing.

### Payload Intelligence

Tracks payload performance, execution probability, false positive rates, and contextual behavior.

### WAF Tracker

Observes how defensive technologies influence payload execution and validation results.

### Encoding Strategy Engine

Studies how different payload encodings affect detection accuracy, execution behavior, and false positive generation.

### Deep Learning Evidence Classifier

Uses transformer-based models to classify evidence as positive, negative, or neutral.

### Human Feedback Learning

Incorporates analyst validation to continuously improve future decisions.

### Explainable Confidence Engine

Provides transparent reasoning behind every decision made by the system.

---

## Expected Contributions

VERA investigates a new approach for automated vulnerability validation by combining:

* Evidence correlation
* Machine learning
* Deep learning
* Human feedback
* Continuous payload intelligence

The expected outcome is a measurable reduction in false positives while maintaining strong detection capabilities.

---

## Project Status

Current phase:

Research Design and Architecture Definition

Future phases:

* Laboratory Development
* Dataset Generation
* Model Training
* Experimental Evaluation
* Scientific Publication

---

## License

Research project under active development.
