# Cognition Loop: Building Autonomous ReAct Agents

Welcome to the Cognition Loop. This project bridges the gap between basic conversational chatbots and autonomous, action-driven AI systems.

## The Final Vision

Current consumer LLMs are passive systems: they require a user prompt, generate text, and halt. This project shifts that paradigm. Over the next eight weeks, you will engineer an active, autonomous agent capable of reasoning through multi-step problems and executing actions in the real world.

By the end of this project, you will build an orchestration engine capable of executing complex instructions such as:
> *"Query the internal documentation database for troubleshooting steps regarding error code 404, summarize the fix, and then open a web browser to order a replacement ethernet cable from Amazon."*

To achieve this, the agent will independently:
1. Formulate a plan.
2. Utilize a Retrieval-Augmented Generation (RAG) tool to search internal documents.
3. Utilize browser automation tools (Selenium/Playwright) to interact with live websites.
4. Process the observations and complete the objective without human intervention.

##  Week 1: Required Reading & Technical Resources

Before writing the control logic, it is critical to understand the underlying architecture of modern AI. Review these resources before starting the tasks.

### 1. Conceptual Foundations
* **The Mechanics of LLMs:** [[1hr Talk] Intro to Large Language Models by Andrej Karpathy](https://www.youtube.com/watch?v=zjkBMFhNj_g) — Demystifies how standard generative models are trained and why they hallucinate. Understand the training pipeline, tokenization, and the fundamental limitations of standard generative models.
* **The Shift to Agentic AI:** [Andrew Ng Explores The Rise Of AI Agents](https://www.youtube.com/watch?v=KrRD7r7y7NY) — Explains the conceptual shift from direct prompting to systems that utilize reflection, tool use, and planning.
* **The ReAct Framework:** [Prompt Engineering Guide: ReAct](https://www.promptingguide.ai/techniques/react) — Differentiate between standard prompting, Chain of Thought, and the ReAct methodology.
* **4Data Serialization (JSON & APIs)** - Understand why autonomous agents rely on strictly structured JSON data rather than conversational text to trigger external code.
### 2. Core API Documentation
* **Google GenAI SDK (Python):** [Official Documentation](https://ai.google.dev/api/python/google/genai) — Bookmark this. You will need it for understanding how to pass System Instructions, force JSON schemas, and handle rate limits.




