# No-Code AI Automation: Google Form → Groq AI (Make.com)
**Build Log — Connecting a real workflow with Google Forms, Google Sheets, Groq (Llama-3.3-70B), and Make.com.**

**By:** Sumaira Safeer

![Status](https://img.shields.io/badge/status-in%20progress-yellow) ![Type](https://img.shields.io/badge/type-no--code%20automation-blue) ![Tool](https://img.shields.io/badge/tool-Make.com-orange)

---

## 📌 Overview
This automation:
- Triggers on new Google Form submissions.
- Sends submitted data to Groq AI for summarization and categorization.
- Logs the results and prepares them for a final action (email, Slack notification, or sheet update).

Built entirely on the **Make.com free tier**, with no custom backend code required.

---

## 🔄 Workflow Architecture

```
Google Form Submission
        │
        ▼
  Google Sheets (Trigger)
        │
        ▼
   Groq AI Module (llama-3.3-70b-versatile)
        │
        ▼
  Summarization + Categorization
        │
        ▼
  Final Action (planned: Email / Slack / Sheet Update)
```

---

## 🛠️ Build Steps
| Step | Description |
|---|---|
| 1 | Set up the Google Sheets trigger and add the Groq module. |
| 2 | Configure the Groq API connection |
| 3 | Write the system prompt to define the AI agent's persona.|
| 4 | Map form fields dynamically into the user message. |

**Status:** Trigger and AI step are fully working — the execution log confirms successful runs.

---

## ⚙️ Key Technologies
- **Trigger:** Google Forms → Google Sheets
- **AI Model:** Groq (`llama-3.3-70b-versatile`)
- **Orchestration:** Make.com
- **Final Action:** Planned — email, Slack, or sheet update.

---

## 💡 Learnings
- Make.com is well suited to multi-step, no-code automation scenarios.
- Groq offers fast, low-cost inference for Llama models ideal for real-time workflows.
- Dynamic field mapping (rather than hardcoded values) makes automations far more robust and reusable.

---

## 🚧 Next Steps
- Implement the final action module (email notification, Slack alert, or sheet write-back).
- Add error handling for malformed or incomplete form submissions.
- Expand the system prompt to support additional categorization labels.

---

## 👩‍💻 Author
**Sumaira Safeer**
Computer Engineer

**Internship:** NeuroFive Solutions: Generative AI & Prompt Engineering

**LinkedIn:** [linkedin.com/in/sumaira-safeer-948804418](https://www.linkedin.com/in/sumaira-safeer-948804418/)
**GitHub:** [github.com/SumairaSafeer](https://github.com/SumairaSafeer)
