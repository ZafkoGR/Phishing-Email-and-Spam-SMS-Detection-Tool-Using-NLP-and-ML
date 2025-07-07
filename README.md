# 📩 AI-Based Phishing Email & SMS Spam Detection Tool

This project delivers a natural-language, machine-learning system that classifies incoming messages as **spam/phishing** or **ham** with millisecond-level latency—ideal for real-time inbox or gateway protection.

---

## 📘 Project Background  

This tool constitutes **Chapter 5.1** of my Master’s thesis, *Practical AI in Cyberwarfare and Cybersecurity*, and is officially included in the submitted manuscript.

**Author**: Konstantinos Zafeiropoulos (Student ID 20390293)  
**Institution**: University of West Attica – Faculty of Engineering, Department of Informatics and Computer Engineering  

> 📚 The full thesis (including this tool) will be published in the institutional repository **«Πολυνόη» (Polynoe)** and indexed on **Google Scholar** by **September 2025**.

---

## 1️⃣ Why AI is Needed  

- Spam and phishing messages use obfuscation (`V!agra`, homographs, spoofed domains) and natural-language tricks.  
- AI models **learn semantic and statistical patterns** at scale, outperforming rigid keyword lists.  
- Provides **instant** (< 0.2 ms) classifications across thousands of messages.

---

## 2️⃣ Can This Be Done Without AI?  

Rule-based filters:  
- Are easily bypassed by new misspellings or context shifts.  
- Require constant manual updates.  
- Miss cleverly disguised fraud.  

✅ AI offers adaptive learning, context awareness, and superior recall/precision.

---

## 3️⃣ AI Algorithm Used  

- **Logistic Regression** (supervised binary classifier)  
- **TF-IDF Vectorization** for text featurization  
- NLTK preprocessing: lower-casing, stop-word removal, tokenization  

Fast, interpretable, and well-suited for high-dimensional text data.

---

## 4️⃣ Tool & AI Architecture  

### 🔄 Workflow  

1. **Input**: Raw SMS or email text  
2. **Preprocessing**:  
   - Lower-case conversion  
   - Stop-word removal  
   - TF-IDF transformation  
3. **Modeling**: Logistic Regression classifier  
4. **Output**: `spam` (0) or `ham` (1) label  

Latency ≈ 0.18 ms per message on modern CPUs.

---

## 5️⃣ AI Subcategory  

✅ **Supervised Machine Learning** → **Binary Text Classification (NLP)**

---

## 6️⃣ Purpose & Social Impact  

- **Block** phishing and spam before they reach end-users.  
- **Prevent** financial fraud, credential theft, and social-engineering attacks.  
- **Educate** users via explainable outputs (top spam terms, class balance).

---

## 7️⃣ Dataset Overview  

| Dataset Name            | Type | Content Description | Labels |
|-------------------------|------|---------------------|--------|
| `spam_sms_emails.csv`   | SMS + Email | Real-world messages with spam tactics and legitimate (ham) samples | `spam`, `ham` |

---
