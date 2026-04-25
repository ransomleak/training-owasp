# Free Interactive OWASP Training Library

**Free hands-on interactive OWASP exercises in SCORM format:**
- OWASP Top 10 for Agentic Applications (10 exercises)
- OWASP Top 10 for LLM Applications (10 exercises)


![demo](/Assets/demo.gif)

🔗 **[Browse the full library →](https://ransomleak.com/learning)** &nbsp;|&nbsp; 🎮 **[Try a live demo →](https://ransomleak.com/exercises/clawdbot-prompt-injection/)**

---

## Why this exists

AI agents, LLMs, and autonomous tools are being adopted faster than the security practices meant to govern them. While threats like phishing are well-understood, the AI wave has introduced attack vectors that most people have never encountered — prompt injection, RAG exploitation, and more. The problem isn't awareness alone. Most security training is passive: slide decks and videos that people click through and forget. 

This library takes a different approach. Every exercise drops you into an interactive 3D office environment where you face realistic scenarios in first-person. You interact with real objects — a phone, a PC running a live OS (browser, terminal, Zoom), a flipchart — and make decisions under pressure, just like you would at your desk.

Scenarios include things like:

 - Identifying hidden prompt injection instructions in uploaded documents
 - Spotting sensitive data categories that should never enter AI prompts
 - Evaluating third-party AI plugins for supply chain risks before deployment
And more!

The goal is to build muscle memory so that when you need to apply your knowledge, you remember having faced it before — and act accordingly. Every exercise ends with a quiz at a 70% pass threshold to confirm the knowledge is stuck.

---

## Format

Every exercise is a **SCORM .zip file** — ready to import into any LMS, embed into your existing training pipeline, or test on [SCORM Cloud](https://cloud.scorm.com/) before rollout.

The repo root contains full course packages. Other .zip files in corresponding folders contain standalone exercises if you want to build a custom curriculum.

**The content is fully white-labeled** — no logos, no backlinks, no strings attached. Use it however you like, more on this below.

---

## Usage & License

You're free to use, embed, and teach with this content — personally, professionally, or commercially in workshops. Redistributing or reselling the content as a standalone product is prohibited.

[![CC BY-NC 4.0][cc-by-nc-shield]][cc-by-nc]

This library is licensed under [CC BY-NC 4.0][cc-by-nc]. Free to use and share with attribution. Commercial resale of the content is prohibited.

[cc-by-nc]: https://creativecommons.org/licenses/by-nc/4.0/
[cc-by-nc-shield]: https://img.shields.io/badge/License-CC%20BY--NC%204.0-lightgrey.svg

If this project will get some traction, we'll make more exercises. So please share your feedback!

---

## Table of Contents

### OWASP Top 10 for Agentic Applications

1. [**AI Agent Goal Hijacking**](https://ransomleak.com/exercises/agentic-goal-hijack/) — Stop an autonomous AI agent from being redirected by a poisoned email containing hidden instructions by detecting hidden instructions embedded in incoming data that redirect agent objectives, tracing how a goal-hijacked agent pivots from legitimate tasks to data exfiltration, and applying input validation strategies that prevent agents from treating data as instructions.

2. [**AI Agent Tool Exploitation**](https://ransomleak.com/exercises/agentic-tool-misuse/) — Prevent an AI agent from being manipulated into using its legitimate tools to delete files and send unauthorized messages by identifying how ambiguous prompts cause agents to misuse legitimate tool access, tracing destructive tool calls triggered by manipulated input parameters, and applying least-privilege tool access policies to contain agent tool exploitation.

3. [**Agent Identity and Privilege Abuse**](https://ransomleak.com/exercises/agentic-identity-privilege-abuse/) — Prevent an AI agent from reusing inherited high-privilege credentials to access systems beyond its authorized scope by tracing how agents inherit and propagate user credentials across different system contexts, identifying confused deputy vulnerabilities where agent privilege exceeds intended scope, and applying scoped credential delegation to prevent cross-context privilege escalation.

4. [**Agentic AI Supply Chain Attack**](https://ransomleak.com/exercises/agentic-supply-chain/) — Investigate a backdoored third-party AI plugin that silently modifies agent behavior and exfiltrates sensitive data by detecting behavioral anomalies indicating a compromised third-party AI component, tracing data exfiltration pathways through backdoored plugins and MCP servers, and applying supply chain verification practices before integrating external AI tools.

5. [**AI Agent Code Injection**](https://ransomleak.com/exercises/agentic-code-execution/) — Catch an AI coding assistant before it executes a shell script containing injected commands that compromise your system by detecting injected commands hidden within AI-generated code and shell scripts, tracing how user input flows through code generation into unsandboxed execution, and applying code review and sandboxing practices to AI-generated scripts before execution.

6. [**AI Agent Memory Poisoning**](https://ransomleak.com/exercises/agentic-memory-poisoning/) — Detect adversarial content injected into an AI agent's persistent memory that corrupts all future decisions by identifying poisoned entries in an agent's persistent memory and retrieval context, tracing how corrupted memory influences downstream agent decisions across sessions, and applying memory integrity verification to detect and remove adversarial content.

7. [**Agent-to-Agent Communication Spoofing**](https://ransomleak.com/exercises/agentic-insecure-communication/) — Intercept and identify spoofed messages between AI agents in a multi-agent workflow before fabricated instructions cause damage by detecting spoofed agent identities and fabricated messages in multi-agent communication channels, tracing how unauthenticated inter-agent messages enable man-in-the-middle attacks, and applying message authentication and agent identity verification to secure multi-agent systems.

8. [**Multi-Agent Cascading Failure**](https://ransomleak.com/exercises/agentic-cascading-failures/) — Contain a minor AI hallucination before it cascades through downstream agents into a catastrophic system-wide failure by tracing error propagation from a single agent hallucination through multiple downstream systems, identifying amplification points where small errors compound into catastrophic outcomes, and applying circuit breaker patterns and human checkpoints to interrupt cascading agent failures.

9. [**Over-Trusting AI Agent Recommendations**](https://ransomleak.com/exercises/agentic-trust-exploitation/) — Catch a series of compromised AI agent recommendations that exploit your trust to approve a fraudulent transfer and a backdoored code change by recognizing automation bias patterns where consistent AI accuracy creates false confidence, identifying subtle anomalies in AI recommendations that indicate manipulation or compromise, and applying structured verification workflows that resist social engineering through AI interfaces.

10. [**Detecting a Rogue AI Agent**](https://ransomleak.com/exercises/agentic-rogue-agent/) — Investigate a compromised AI agent that appears functional while silently performing unauthorized actions and evading monitoring by detecting covert unauthorized actions performed by an agent that appears to be operating normally, tracing persistence mechanisms that allow rogue agents to survive restarts and monitoring sweeps, and applying behavioral analysis and anomaly detection to distinguish rogue agents from legitimate ones.


### OWASP Top 10 for LLM Applications

1. [**OpenClaw Prompt Injection**](https://ransomleak.com/exercises/clawdbot-prompt-injection/) — Stop an AI assistant from leaking data via hidden prompts by identifying hidden instructions in documents, preventing data exfiltration through AI tools, and recognizing prompt injection patterns.

2. [**Sensitive Data Exposure Through AI**](https://ransomleak.com/exercises/llm-sensitive-data-disclosure/) — See what happens when confidential data enters a consumer AI tool by recognizing sensitive data categories that should never enter AI prompts, tracing how pasted content persists in AI training data and logs, and applying data classification policies before using AI tools.

3. [**AI Supply Chain Compromise**](https://ransomleak.com/exercises/llm-supply-chain-attack/) — Deploy an AI plugin that hides a backdoor in plain sight by identifying supply chain risks in third-party AI models and plugins, detecting behavioral anomalies in AI components from external sources, and applying vetting procedures before deploying marketplace AI tools.

4. [**AI Training Data Poisoning**](https://ransomleak.com/exercises/llm-data-poisoning/) — Watch poisoned documents corrupt your AI's answers in real time by tracing how manipulated documents alter AI-generated outputs, identifying signs of data poisoning in AI responses, and applying content integrity controls to knowledge base inputs.

5. [**Unsafe AI Output Handling**](https://ransomleak.com/exercises/llm-improper-output-handling/) — Exploit an AI whose outputs flow unchecked into live systems by identifying injection risks when AI outputs feed into downstream systems, tracing how unsanitized AI output enables code execution, and applying output validation controls between AI and connected systems.

6. [**Over-Permissioned AI Agent**](https://ransomleak.com/exercises/llm-excessive-agency/) — Manipulate an AI assistant into misusing its own permissions by identifying excessive permissions granted to AI agents, tracing unauthorized actions performed by manipulated AI tools, and applying least-privilege principles to AI agent configurations.

7. [**AI System Prompt Extraction**](https://ransomleak.com/exercises/llm-system-prompt-leakage/) — Extract hidden instructions from a customer-facing AI chatbot by executing prompt extraction techniques against a live AI chatbot, identifying sensitive information exposed through leaked system prompts, and applying prompt hardening techniques to prevent system instruction disclosure.

8. [**RAG Pipeline Exploitation**](https://ransomleak.com/exercises/llm-vector-embedding-attack/) — Exploit a RAG pipeline to access documents beyond your clearance by identifying access control failures in vector database retrieval, tracing how adversarial embeddings corrupt search results, and applying authorization checks at the retrieval layer of RAG systems.

9. [**AI Hallucination and Misinformation**](https://ransomleak.com/exercises/llm-ai-misinformation/) — Catch fabricated statistics and fake citations in an AI report by detecting hallucinated facts and fabricated sources in AI outputs, verifying AI-generated claims against authoritative references, and applying fact-checking workflows to AI-assisted business content.

10. [**AI Denial-of-Service Attack**](https://ransomleak.com/exercises/llm-unbounded-consumption/) — Launch a denial-of-wallet attack against an unprotected AI API by identifying resource exhaustion vectors in AI API endpoints, tracing how crafted prompts escalate compute costs exponentially, and applying rate limiting and budget controls to AI service deployments.

