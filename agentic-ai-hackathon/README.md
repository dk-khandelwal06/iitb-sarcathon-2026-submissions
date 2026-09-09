# Agentic AI Hackathon 2026 — FasalRakshak

**Competition:** Agentic AI Hackathon 2026  
**Organizer:** IIT Bombay  
**Team:** Ctrl C + Ctrl V

## 🌾 Project

### FasalRakshak — फसल रक्षक

**Deadline-Aware PMFBY Loss Intimation Agent**

FasalRakshak is an agentic AI concept designed to help small and marginal farmers report crop losses under the **Pradhan Mantri Fasal Bima Yojana (PMFBY)** through **WhatsApp and voice in Hindi/Hinglish**.

The system is designed to go beyond a traditional chatbot by understanding an unstructured report, planning the required steps, using available tools, verifying information, taking action, recovering from failures, and maintaining state until a trustworthy outcome is reached.

## 🎯 Problem

Under PMFBY, farmers must file a loss intimation within the applicable **72-hour window** after crop damage.

The challenge is often not the absence of a claim, but the difficulty of completing the reporting workflow on time. Complex portals, failed communication channels, unavailable information, and mismatched details can cause valid claims to miss the deadline.

## 🤖 Agentic Workflow

FasalRakshak follows a multi-step agentic workflow:

**Report → Ingest → Clarify → Verify → Plan → Check → Confirm → Act → Verify → Recover → Status → Remember**

The system is designed to:

- Understand Hindi/Hinglish voice or text reports
- Extract information from farmer inputs and documents
- Ask targeted clarification questions
- Verify critical information through read-back
- Track the 72-hour deadline
- Check eligibility and available information
- Require explicit consent before consequential submission
- Submit through an available channel
- Verify the resulting tracking ID
- Recover from channel/API failures
- Maintain state for follow-up and status updates

## 🏗️ Proposed Architecture

**Farmer (WhatsApp / Voice)**  
↓  
**Agent Core — LLM Planning & State**  
↕  
**OCR/Vision · PMFBY APIs · IMD Weather**  
↓  
**Verified Outcome**

## 🔧 Prototype Feasibility

The proposed prototype uses:

- WhatsApp Business API
- Hindi/Hinglish ASR using Bhashini API or Whisper
- LLM-based agent planning and tool calling
- Vision / Land Record OCR
- PMFBY enrollment lookup
- IMD weather data
- SQLite/Postgres state persistence

Where real government integrations are not publicly accessible, the submission explicitly identifies the relevant components as **MOCK** or **SIMULATED** rather than presenting them as live integrations.

## 🛡️ Safety & Reliability

FasalRakshak is designed around:

- Explicit user consent before submission
- No fabricated success
- Human verification for critical extracted information
- Confidence thresholds for OCR/ASR
- Transparent failure handling
- Minimal PII retention
- Recovery and fallback pathways when channels fail

## 📊 Evaluation Plan

The proposed evaluation uses **20 scripted real-world scenarios** with target metrics covering:

- Completion Rate
- Field Extraction Accuracy
- Failure Recovery
- Time-to-Intimation

## 📄 Submission

[View the Complete FasalRakshak Idea & Feasibility Submission](CtrlC_CtrlV_FasalRakshak_Agentic_AI_Hackathon_2026.pdf)

---

### 👥 Team

**Ctrl C + Ctrl V**

- **Daksh Khandelwal**
- **Khushi Kushwah**

**IIT Jodhpur**

---

*IIT Bombay SARCathon 2026 · Agentic AI Hackathon 2026*
