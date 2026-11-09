# Beyond the Chatbot

### Building and Shipping Real AI Apps with LLMs

**A Google Developer Group (GDG) on Campus — JIS University session**

*Build real AI applications, not just prompts.*


---

## About the Event

**Beyond the Chatbot** was a GDG on Campus JIS University learning session designed to take students beyond experimenting with prompts and introduce the process of building practical, reliable AI-powered applications.

The session explored how Large Language Models (LLMs) can be integrated into applications, how to work with the Gemini API, and what it takes to move from a working prototype to a more dependable application.

The event also featured an **Introduction to GDG on Campus at JIS University**, giving participants an opportunity to learn about the developer community, connect with fellow students, and understand ways to get involved.

## Event Details

| Detail | Information |
|---|---|
| Event | Beyond the Chatbot |
| Theme | Building and Shipping Real AI Apps with LLMs |
| Community | Google Developer Group on Campus — JIS University |
| Date | 5 November 2026 |
| Time | 2:00 PM – 5:00 PM |
| Venue | JIS University, Kolkata |
| Speaker | Suryanshu Paul, AI Engineer at humaineeti |
<p align="center">
<img width="700px" height="500px" alt="image" src="https://github.com/user-attachments/assets/eec764fe-42a1-4081-b0c3-5c00cde3f4a8" />
</p>


### What the Session Covers

The session focuses on the practical building blocks of modern LLM applications:

### 1. LLMs and AI Basics
- Understanding Large Language Models and how they are used in applications.
- Tokens, context windows, temperature, and hallucinations.
- Understanding the strengths and limitations of model-generated responses.

### 2. Prompt Engineering
- Structuring prompts with roles, context, rules, examples, and output formats.
- Improving consistency and clarity in model responses.
- Knowing when prompt engineering is enough and when a more advanced approach is needed.

### 3. Application Development
- Connecting applications to an LLM through an API.
- Working with the Gemini API and Python.
- Handling model responses in application code.
- Using structured output to make responses easier to validate and process.

### 4. Hands-on Tools and Techniques
- Structured JSON output.
- Retrieval-Augmented Generation (RAG).
- Embeddings and retrieval.
- Function calling and application-controlled tools.
- An introduction to AI agent workflows.

### 5. Real-world Use Cases
- Building assistants around useful information sources.
- Summarising and extracting information from documents.
- Designing workflows that are useful beyond a single prompt.
- Thinking about reliability, security, latency, and cost.

---

## Hands-on Demo: Campus Notice Assistant

A practical example discussed in the session is a **Campus Notice Assistant** built with Python and the Gemini API.

The idea is to help students work with campus notices by turning unstructured notice content into concise summaries and structured information.

The walkthrough is organised around these steps:

1. **Summarise a notice** — generate a short summary in three bullet points.
2. **Extract event information** — identify fields such as event title, date, and venue in a structured JSON response.
3. **Use function calling** — demonstrate how a model can request an application function, such as adding an event to a calendar.
4. **Improve reliability** — consider retries with exponential backoff and a fallback model.
5. **Add observability** — track details such as the model used, response latency, and token usage.

> The session material explains the demo workflow and the engineering concepts behind it. Refer to the source code present in this repository for the exact implementation and available features.

---

## From Prototype to Production

A successful model response is only one part of a real application. Production-minded development also means considering:

- **Validation:** Check model output before your application uses it.
- **Reliability:** Handle timeouts, transient errors, retries, and provider failures.
- **Fallbacks:** Have a sensible alternative when a model or service is unavailable.
- **Evaluation:** Test responses against realistic examples rather than relying on a few successful prompts.
- **Observability:** Measure latency, token usage, errors, and cost.
- **Security:** Protect API keys and treat user-provided documents as untrusted input.
- **Human oversight:** Require approval before performing sensitive or irreversible actions.

### Key Engineering Takeaways

1. Start with a simple prompt and add complexity only when the use case requires it.
2. Use RAG when the model needs to answer using external or domain-specific information.
3. Keep tool execution under application control.
4. Validate structured output before using it.
5. Measure quality, latency, and cost as part of development.
6. Design for failure instead of assuming every API call will succeed.

---

## GDG on Campus — JIS University

GDG on Campus is a student developer community that creates opportunities to learn, build, collaborate, and connect with the wider developer ecosystem.

The JIS University community aims to bring students together through technical sessions, hands-on learning, peer collaboration, and community activities.

The event also included an introduction to GDG on Campus JIS University and its community.

---

## Meet the New Organizers
<p align="center">
<img width="500px" height="500px" alt="image" src="https://github.com/user-attachments/assets/767e760e-a1f4-4477-a139-033b0403cc1f" />
</p>
The photograph above captures the certificate presentation during the event. **The three certificate recipients shown in the photograph are the new organizers of GDG on Campus JIS University.**

This marks an important step for the community as the new organizing team takes forward its activities, learning initiatives, and student engagement.

We congratulate the new organizers and look forward to the sessions, workshops, collaborations, and opportunities they will help create for the JIS University developer community.

*The photograph is shared as an event record. Individual names and roles are not listed here.*

---

## Moments from the Session

### The Speaker in Action
<p align="center">
<img width="600px" height="600px" alt="image" src="https://github.com/user-attachments/assets/770861a7-e364-428f-900a-5b63b2979c53" />
</p>
A moment from the technical session, where concepts around APIs and building AI-powered applications were discussed with participants.


## Suggested Learning Path

Whether you are just starting with AI or already building applications, use this as a practical path after the session.

### Beginner Track

| Stage | Focus | Try this |
|---|---|---|
| 1 | Python fundamentals | Practise functions, loops, and file handling. |
| 2 | Gemini API | Make a first model call from a Python script. |
| 3 | Prompting | Build a notice or lecture-notes summariser. |
| 4 | Structured output | Extract dates, venues, and titles into JSON. |

### Intermediate / Builder Track

| Stage | Focus | Try this |
|---|---|---|
| 1 | RAG | Build question answering over syllabus PDFs. |
| 2 | Function calling | Connect a model to a calculator or calendar function. |
| 3 | Reliability | Add timeouts, retries, and a fallback. |
| 4 | Evaluation | Test the app with a small set of realistic questions. |
| 5 | Deployment | Deploy the project and monitor usage and errors. |

---

## Getting Started

The examples and concepts are based on Python and the Gemini API.

### Prerequisites

- Python 3.10 or later.
- A Google account.
- A Gemini API key from [Google AI Studio](https://aistudio.google.com/).
- Basic familiarity with Python and the command line.

### Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd <YOUR_REPOSITORY_FOLDER>
```

Replace the placeholders with your repository URL and folder name.

### Create a Virtual Environment

**Windows (PowerShell):**

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

**macOS / Linux:**

```bash
python3 -m venv .venv
source .venv/bin/activate
```

### Install the Packages

The session uses the Google Gen AI Python SDK and Pydantic for structured output.

```bash
pip install -U google-genai pydantic
```

If a `requirements.txt` is included in the repository, you can install its dependencies with:

```bash
pip install -r requirements.txt
```

### Configure Your Gemini API Key

Set your API key as an environment variable. Never hard-code it in source files or commit it to Git.

**Windows (PowerShell):**

```powershell
$env:GEMINI_API_KEY="YOUR_API_KEY"
```

**macOS / Linux:**

```bash
export GEMINI_API_KEY="YOUR_API_KEY"
```

Get your API key from [Google AI Studio](https://aistudio.google.com/).

### Run the Demo

Use the entry-point filename and instructions provided by the actual source code in this repository. For a Python entry file, the command will generally look like:

```bash
python <entry_file>.py
```

---
## Useful Resources

- [Gemini API Documentation](https://ai.google.dev/gemini-api/docs)
- [Google AI Studio](https://aistudio.google.com/)
- [Google Gemini Cookbook](https://github.com/google-gemini/cookbook)
- [Kaggle](https://www.kaggle.com/)
- [GDG Community Events](https://gdg.community.dev/)

---

## Contributing

Contributions that improve the examples, documentation, code quality, tests, or learning experience are welcome.

1. Fork this repository.
2. Create a feature branch.
3. Make your changes and test them.
4. Open a pull request with a clear description.

Please do not commit API keys, credentials, private notices, or other sensitive information.

## Acknowledgements

A big thank you to **Suryanshu Paul** for sharing practical insights into building and shipping real AI applications, and to everyone who contributed to making the GDG on Campus JIS University session possible.

Thank you to the organizers, volunteers, and participants who made the event a space for learning, collaboration, and community.

---

**Google Developer Group on Campus — JIS University**

*Learn. Build. Connect.*

**Beyond the Chatbot — Build real AI applications, not just prompts.**
