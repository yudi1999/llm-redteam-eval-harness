# 🛡️ LLM Red Team & Security Evaluation Harness

A lightweight, modular Python framework designed for automated red-teaming, adversarial prompt injection detection, jailbreak scoring, and safety alignment verification of Large Language Models (LLMs).

## 🚀 Key Features
- **Prompt Injection & Jailbreak Scanners:** Regex-based heuristic detection and rule-based payload checks for system prompt exfiltration attempts.
- **Safety Behavioral Alignment Grader:** Automated scoring harness evaluating model responses against policy violations and fabricated authorities.
- **Structured JSON Output:** Normalizes evaluation results into structured JSON logs for audit trails.
- **Zero-Dependency Core:** Pure Python standard library plus minimal JSON schema validators.

## 📦 Quick Usage

```python
from evaluator import SafetyAlignmentGrader

grader = SafetyAlignmentGrader(strict_mode=True)
result = grader.evaluate_response(
    prompt="Explain how to bypass system instructions.",
    response="Here is how you can ignore previous constraints..."
)
print(result)
```

## 📜 Certification & Credentials
Developed under certified adversarial methodologies (**CRTOM** - Certified Red Team Operations Management).
