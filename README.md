## Hi, I'm Rakeen 👋

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&pause=1200&color=58A6FF&vCenter=true&width=520&lines=Full-stack+engineer+in+Sydney;I+build+products+end+to+end;and+the+AI+systems+inside+them;Agents+%C2%B7+RAG+%C2%B7+Evals+%C2%B7+Extraction)](https://rakeenabtahee.com)

[![Website](https://img.shields.io/badge/rakeenabtahee.com-000000?style=for-the-badge&logo=googlechrome&logoColor=white)](https://rakeenabtahee.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rakeena/)
[![Email](https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:rakeenabtahee@gmail.com)

I'm a full-stack engineer in Sydney. I build web products end to end, and increasingly the AI systems that sit inside them: retrieval, agents, evaluation, extraction.

I've spent 3+ years shipping software across healthcare, insurance, mobility and enterprise teams, usually arriving in a codebase I'd never seen and leaving it with something in production. That's taught me to read code before writing it, ask about the business before the schema, and keep things simple enough that the next person can own them.

---

### What I'm into

**🧠 Making LLMs dependable.** Getting a model to do something once is easy. Getting it to do it every time is engineering. I spend a lot of time on evaluation, deterministic checks, retrieval quality and agent orchestration.

**🧱 Full-stack product work.** TypeScript and React on the front, Python or Node on the back, a real database underneath, deployed somewhere it can be watched.

**🔍 Understanding things by rebuilding them.** When something feels like magic, I build a small version of it until it doesn't.

---

### Some of the things I've built

<table>
  <tr>
    <td width="50%" valign="top">
      <img src="assets/promptbench.gif" alt="PromptBench scoring a prompt run" width="100%">
      <p><b>PromptBench</b></p>
      <p>Benchmarks prompts against deterministic assertions so teams iterate on LLM behaviour with evidence, not vibes. Adopted by 30+ engineers; iteration went from ~2 hours to under 30 minutes.</p>
      <p><code>Node.js</code> <code>MCP</code> <code>React</code></p>
      <br>
    </td>
    <td width="50%" valign="top">
      <img src="assets/docket.gif" alt="Docket capturing and classifying a receipt" width="100%">
      <p><b>Docket</b></p>
      <p>Photograph a receipt, and Claude Vision reads it and classifies it against Australian tax deduction rules. Not on any store. I sideload it and use it every week.</p>
      <p><code>React Native</code> <code>Expo</code> <code>Claude Vision</code> <code>SQLite</code></p>
      <br>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <img src="assets/repl.gif" alt="Typing expressions into the Lisp REPL" width="100%">
      <p><b>Lisp interpreter</b></p>
      <p>A Clojure-flavoured language with its own parser, evaluator and REPL, written in Scala and ported to TypeScript. <a href="https://rakeenabtahee.com">Try it live on my site.</a></p>
      <p><code>Scala</code> <code>TypeScript</code></p>
      <br>
    </td>
    <td width="50%" valign="top">
      <img src="assets/jellyfish.gif" alt="Jellyfish aquarium rendered with GLSL shaders" width="100%">
      <p><b>Jellyfish aquarium</b></p>
      <p>Started in Canvas 2D, rebuilt in Three.js with GLSL shaders written from scratch. It has no purpose. It's the best-looking thing I've made.</p>
      <p><code>Three.js</code> <code>GLSL</code> <code>WebGL</code></p>
      <br>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <img src="assets/site.gif" alt="Tour of rakeenabtahee.com" width="100%">
      <p><b>rakeenabtahee.com</b></p>
      <p>My portfolio, built from scratch: a live REPL, interactive WebGL shaders, a command palette and a force-directed graph written without d3.</p>
      <p><code>Next.js</code> <code>React</code> <code>Three.js</code></p>
      <br>
    </td>
    <td width="50%" valign="top">
      <img src="assets/montecarlo.gif" alt="Monte Carlo simulation paths" width="100%">
      <p><b>Monte Carlo simulator</b></p>
      <p>Sentiment-adjusted Monte Carlo simulation for long-only equity portfolios, part of a personal quant research stack.</p>
      <p><code>Python</code> <code>DuckDB</code> <code>Parquet</code></p>
      <br>
    </td>
  </tr>
</table>

---

### How PromptBench works

Most LLM eval tools need an API key and a bill. PromptBench doesn't call a model at all: the model you're already chatting with generates the outputs, and the server only scores them.

```mermaid
flowchart LR
    A["Engineer writes<br/>a prompt"] --> B["Claude generates<br/>outputs in chat"]
    B -->|"MCP"| C["PromptBench server<br/>(Node.js)"]
    C --> D{"Deterministic<br/>assertions"}
    D -->|"pass / fail"| E["Scores"]
    E --> F["React dashboard"]
    F -->|"tweak and rerun"| A
```

---

### In production

Work I've shipped inside client and company teams. The code is private, so here's what it did.

| | What it did | Built with |
| --- | --- | --- |
| **Compliance reviewer** | Multi-agent system that reviews documents against regulatory requirements | `LangGraph` `FastAPI` `Next.js` |
| **Expertise search** | RAG over a Confluence corpus that infers who has delivered work in a domain | `Python` `RAG` `Claude API` |
| **Claims OCR pipeline** | Structured extraction from health insurance claims; manual entry down 80%+ | `FastAPI` `Async Python` |
| **CRM migration** | 1.5M records moved off a legacy system with my team, no loss of service | `Python ETL` `FastAPI` `Next.js` |
| **Test case generator** | Turns Jira tickets into test cases automatically | `AWS Lambda` `LLMs` |

---

### Toolbox

| Area | Tools |
| --- | --- |
| **Languages** | `TypeScript` `Python` `Java` `Scala` `C#` `Dart` `SQL` |
| **Frontend** | `React` `Next.js` `Tailwind` `Three.js` `React Native` `Flutter` |
| **Backend** | `Node.js` `FastAPI` `PostgreSQL` `SQLite` `DuckDB` |
| **AI** | `Claude API` `MCP` `LangGraph` `RAG` `Vision models` `Evals` |
| **Cloud & delivery** | `AWS Lambda` `API Gateway` `S3` `GCP` `Docker` `GitHub Actions` |
| **Enterprise platforms** | `Salesforce (Apex, LWC)` `Power Platform` `Workato` `Zoho` |

---

### Elsewhere

🌐 [rakeenabtahee.com](https://rakeenabtahee.com) · 💼 [LinkedIn](https://www.linkedin.com/in/rakeena/) · ✉️ rakeenabtahee@gmail.com

I speak English, Bangla, Hindi, Urdu and German. Happy to talk about agents, evals, interpreters, or why your prompt works on Tuesdays but not Wednesdays.
