<div align="center">

  <h1>Prakhar Shukla</h1>
  <h3>Full-Stack Engineer · Agentic AI Systems · IEEE Published Researcher</h3>
  <p><i>I build AI systems you can actually trust - fraud defense, hallucination detection, and research integrity - with held-out metrics, honest baselines, and production hardening.</i></p>

  <a href="https://www.linkedin.com/in/prakhar-shukla-471649261">
    <img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" />
  </a>
  <a href="https://prakhar-shukla.vercel.app/">
    <img src="https://img.shields.io/badge/Portfolio-Visit-10B981?style=for-the-badge&logo=vercel&logoColor=white" alt="Portfolio" />
  </a>
  <a href="mailto:prakhar230125@gmail.com">
    <img src="https://img.shields.io/badge/Email-Contact-D14836?style=for-the-badge&logo=gmail&logoColor=white" alt="Email" />
  </a>
  <a href="https://twitter.com/prakhar_builds">
    <img src="https://img.shields.io/badge/X-@prakhar__builds-000000?style=for-the-badge&logo=x&logoColor=white" alt="X" />
  </a>

  <br /><br />

  <a href="https://github.com/Prakhar2025"><img src="https://komarev.com/ghpvc/?username=Prakhar2025&label=Profile%20Views&color=6366f1&style=flat-square" alt="Profile Views" /></a>
  <a href="https://ieeexplore.ieee.org/document/11379757"><img src="https://img.shields.io/badge/IEEE-Published_Author-00629B?style=flat-square&logo=ieee&logoColor=white" alt="IEEE" /></a>
  <a href="https://github.com/Prakhar2025/TruthLayer"><img src="https://img.shields.io/badge/AWS-Top_50_Global_Finalist-FF9900?style=flat-square&logo=amazonaws&logoColor=white" alt="AWS Finalist" /></a>
  <img src="https://img.shields.io/badge/National_Winner-IIT_Delhi-8B5CF6?style=flat-square" alt="National Winner" />

</div>

---

### Snapshot

| | |
| :--- | :--- |
| **Focus** | Agentic AI fraud defense · hallucination verification · research-integrity gates |
| **Stack** | TypeScript · Next.js · Python · FastAPI · AWS (Lambda, Bedrock, DynamoDB) · PostgreSQL · MongoDB |
| **Proof** | 5 systems shipped with held-out metrics & CI-gated repro · 2 apps live on Google Play |
| **Research** | 2 published papers - IEEE PuneCon 2025 · i-manager JIP (deepfake detection) |
| **Recognition** | AWS AIdeas Top 50 Global · India AI Impact Grand Finalist (Top 2% of 40,000+) · SBI Youth Ideathon National Winner (IIT Delhi) |

---

### The AI Trust Layer

Most builders make models *faster*. I make their outputs *trustworthy* - verifiable, adversarially tested, and safe to put next to money. Five production systems, one thesis: **models propose, deterministic code decides.**

```
                     ┌──────────────────────────────────────────────┐
                     │             THE AI TRUST LAYER               │
                     │      models propose · code decides           │
                     └───────────────────────┬──────────────────────┘
          ┌──────────────────────┬───────────┴───────────┬──────────────────────┐
          ▼                      ▼                        ▼                      ▼
   ┌─────────────┐        ┌─────────────┐          ┌─────────────┐       ┌─────────────┐
   │  SENTINEL   │        │  GATEHOUSE  │          │ SIGNALGATE  │       │ TRUTHLAYER  │
   │ cross-mrcht │        │ household   │          │ quant       │       │ LLM output  │
   │ fraud graph │        │ scam agent  │          │ integrity   │       │ firewall    │
   ├─────────────┤        ├─────────────┤          ├─────────────┤       ├─────────────┤
   │ 0.857 F1    │        │ 1.00 / 1.00 │          │ 0.925 catch │       │ 95.33% prec │
   │ p50 2.3 ms  │        │ 0.0% f-gate │          │ p = 0.00029 │       │ 5-signal    │
   │ +₹38.6k/1k  │        │ $0.00026/cs │          │ byte-repro  │       │ McNemar✓    │
   └─────────────┘        └─────────────┘          └─────────────┘       └─────────────┘
   defense-only           real-household            recommends,           calibrated
   fraud scoring          soak, live                never trades          confidence
```

---

### Featured - Fraud Defense & Research Integrity

#### 1. [Sentinel - Cross-Merchant Fraud Ring Watchroom](https://github.com/Prakhar2025/Sentinel)
[![Source](https://img.shields.io/badge/Source-View-181717?style=flat&logo=github&logoColor=white)](https://github.com/Prakhar2025/Sentinel)
[![Live Console](https://img.shields.io/badge/Live_Console-Open-22C55E?style=flat&logo=vercel&logoColor=white)](https://d1uo4g1v7ecl77.cloudfront.net)
[![Demo](https://img.shields.io/badge/Demo-5_min_video-FF0000?style=flat&logo=youtube&logoColor=white)](https://youtu.be/Mds3NXkNxHw)

> Defense-only fraud detection for cross-merchant identity reuse - catches the same UPI ID, phone, or device fingerprint recycled across merchants, with explainable verdicts and errors costed in rupees. Recommends, never auto-blocks.

- Identity link graph (fan-out + `0.6^hops` taint) → deterministic 7-feature scorer → `ALLOW / REVIEW / BLOCK_REC` with an evidence bundle; the LLM (Bedrock) writes the analyst narrative only - it never scores
- **Measured (held-out, seed 42):** precision **0.833** · recall **0.882** · F1 **0.857** · 2/2 rings caught · **0** silent frauds · **+₹38,665 net / 1,000 events** · p50 **2.3 ms** · total LLM spend **<$0.10**
- Honest disclosure: a GBDT baseline edges the rules on F1 (0.909 vs 0.857) - reported, not buried; the deterministic scorer keeps the audit contract a money-adjacent system needs
- Hardening: champion/challenger shadow scoring · Prometheus · Postgres/SQLite parity · **90% coverage gate**, strict mypy, CI-gated Docker
- **Stack:** Python · FastAPI · Next.js 15 · AWS Bedrock · DynamoDB · PostgreSQL

#### 2. [Gatehouse - Autonomous Fraud-Defense Agent for Households](https://github.com/Prakhar2025/gatehouse)
[![Source](https://img.shields.io/badge/Source-View-181717?style=flat&logo=github&logoColor=white)](https://github.com/Prakhar2025/gatehouse)
[![Live Console](https://img.shields.io/badge/Live_Console-Open-22C55E?style=flat&logo=vercel&logoColor=white)](https://d2p659vmmc9l0e.cloudfront.net)
[![Demo](https://img.shields.io/badge/Demo-5_min_video-FF0000?style=flat&logo=youtube&logoColor=white)](https://youtu.be/n695eKHMIbY)

> Family members forward any suspicious message or payment request; a Strands agent team investigates it like a professional fraud analyst and escalates only genuine decisions to the family guardian, with a hash-chained evidence bundle.

- Strands agent loop over closed tools (link reputation · brand-claim adjudication · UPI grammar · HMAC-keyed threat graph) - the agent chooses *which check to run*; code composes the verdict. No tool accepts message content or returns a verdict, so the model can't launder untrusted text into evidence. Any loop failure falls back to a deterministic sweep and says so
- **Measured (staging eval, real Nova Micro leg):** precision **1.00** · recall **1.00** (95% CI [0.9887, 1.0]) · false-gate rate **0.0%** - root-caused down from 30.6% pre-calibration and re-verified · **$0.00026 / case** · live soak on real households
- Graduated silence law (`SILENT_KILL → AGENT_SCREEN → BADGED_RING → PASS`): settled scams never page a human; degraded cases always stay visible. PII scrubbing proven by CI canary strings
- **Stack:** Python · Strands Agents SDK · AWS Lambda · Bedrock (Nova Micro) · DynamoDB · EventBridge · Next.js

#### 3. [SignalGate - Agentic Research-Integrity Gate](https://github.com/Prakhar2025/SignalGate)
[![Source](https://img.shields.io/badge/Source-View-181717?style=flat&logo=github&logoColor=white)](https://github.com/Prakhar2025/SignalGate)
[![Repro](https://img.shields.io/badge/Eval-Byte--identical_in_CI-8B5CF6?style=flat)](https://github.com/Prakhar2025/SignalGate)

> Candidate quant trading signals investigated like fraud cases - statistical probes as tools, verdicts with receipts, silence unless a signal deserves a researcher's hour. Recommends, never trades.

- Static lint + investigator agent + 4 sandboxed verification probes (timestamp alignment · label permutation · regime subsample · turnover/cost sanity) → `REJECT_SPURIOUS / NEEDS_REVIEW / PROMISING`, each with numeric receipts; thresholds live in code, never in the model
- **Measured (60 seeded cases, 6 strata, 48 dev / 12 sealed hold-out):** spurious catch **0.925** vs lint baseline 0.475 (+0.450) · prose-hidden lookahead **0.0 → 1.0** · false-reject **0.0** · McNemar **p = 0.00029** · byte-identical repro asserted in CI
- Honest changelog: a bare-prompt agent hit 1.0 catch but false-rejected 0.875 of sound signals - the four probes are the contribution that restored false-reject to 0.0
- **Stack:** Python · FastAPI · Typer CLI · HTMX/Tailwind (zero Node build) · sandboxed subprocess probes

---

### Featured - AI Trust Layer Foundations

#### [TruthLayer - AI Hallucination Firewall](https://github.com/Prakhar2025/TruthLayer)
[![Source](https://img.shields.io/badge/Source-View-181717?style=flat&logo=github&logoColor=white)](https://github.com/Prakhar2025/TruthLayer)
[![Live Demo](https://img.shields.io/badge/Live_Demo-Visit-22C55E?style=flat&logo=vercel&logoColor=white)](https://truth-layer.vercel.app/)
[![AWS AIdeas](https://img.shields.io/badge/Top_50_Global_Finalist-AWS_10%2C000_AIdeas-FF9900?style=flat&logo=amazonaws&logoColor=white)](https://github.com/Prakhar2025/TruthLayer)

> A five-signal verification engine that checks LLM outputs against source documents - catching numerical transpositions, negation flips, and self-contradictions that embedding-only systems miss.

- Amazon Bedrock Titan Embeddings V2 (1024-dim) → cosine relevance + entity-contradiction engine + intra-response consistency → `VERIFIED / UNCERTAIN / UNSUPPORTED`, with **Platt-scaled calibrated confidence** (a real posterior, not a rescaled cosine distance)
- **Measured (300-case adversarial benchmark):** precision **95.33%** · accuracy **90.33%** · F1 **90.79%** - superiority over a cosine-only baseline proven by **McNemar's test (p < 0.05)**
- Serverless AWS (Lambda + API Gateway + DynamoDB) · Python + TypeScript SDKs · Next.js dashboard
- **Top 50 Global Finalist - AWS 10,000 AIdeas Competition**
- **Stack:** Python · Next.js · AWS Lambda · Bedrock

#### [ScamShield - Agentic AI Honeypot](https://github.com/Prakhar2025/Agentic-Honey-Pot)
[![Source](https://img.shields.io/badge/Source-View-181717?style=flat&logo=github&logoColor=white)](https://github.com/Prakhar2025/Agentic-Honey-Pot)
[![Live Demo](https://img.shields.io/badge/Live_Demo-Visit-22C55E?style=flat&logo=vercel&logoColor=white)](https://scamshield-honeypot.vercel.app/)

> Autonomous honeypot that engages scammers in multi-turn conversation, extracts financial intelligence, and classifies scam types in real time.

- 5 adaptive LLM personas (LLaMA 3.3-70b via Groq) · 8 scam-type classifications · **85–90% intelligence extraction accuracy** (phones, UPI IDs, bank accounts, phishing URLs) · Next.js dashboard · MongoDB Atlas
- **Grand Finalist - India AI Impact Buildathon 2026 (Top 2% of 40,000+)**, presented at Bharat Mandapam, New Delhi
- **Stack:** Python · FastAPI · Next.js · Groq · MongoDB

#### [EthAum AI - SaaS Marketplace](https://github.com/Prakhar2025/EthAum-Venture-Partners)
[![Source](https://img.shields.io/badge/Source-View-181717?style=flat&logo=github&logoColor=white)](https://github.com/Prakhar2025/EthAum-Venture-Partners)
[![Live Demo](https://img.shields.io/badge/Live_Demo-Visit-22C55E?style=flat&logo=vercel&logoColor=white)](https://ethaumai.vercel.app/)
[![API Docs](https://img.shields.io/badge/API_Docs-OpenAPI-85EA2D?style=flat&logo=swagger)](https://ethaum-venture-partners.onrender.com/docs)

> Full-stack AI SaaS marketplace (Product Hunt + G2 + Gartner) for Series A–D startups - AI Trust Score, sentiment analysis, upvotes, enterprise pilot marketplace.

- Role-based access (Founder, Buyer, Admin) · 50+ REST endpoints · 7,000+ lines, solo-built and fully deployed
- **Stack:** Next.js 14 · FastAPI · PostgreSQL · Supabase · Clerk Auth

<details>
<summary><b>More builds</b></summary>

- [VentureNode - Autonomous AI OS for Startups](https://github.com/Prakhar2025/VentureNode) - multi-agent LangGraph pipeline for idea analysis and market research *(TypeScript · LangGraph · Notion MCP · Next.js)*
- [Canvas AI - Generative UI Workspace](https://github.com/Prakhar2025/canvas.ai) - natural language → state-managed UI, 9 generative components, 10 AI tools *(Next.js 15 · Tambo AI SDK · Framer Motion)* · [demo](https://youtu.be/RehnLLqULJ8)

</details>

---

### How I engineer

*The part I'd want a senior reviewer to read.*

- **Models propose, code decides.** Scoring and verdicts are deterministic and seed-reproducible; LLMs write narratives, never verdicts or money-movement decisions.
- **Honest baselines.** I publish where a GBDT beats my rules (Sentinel), where a bare-prompt agent false-rejects (SignalGate), and where calibration started broken (Gatehouse) - with the artifacts committed beside the fix.
- **Byte-identical repro.** Every claimed number regenerates from one `make` command with fixed seeds, asserted in CI.
- **Degrade explicitly.** Store down → spool-and-503 · LLM down → `SKIPPED` banner · probe timeout → disclosed. Never a silent pass, never autonomous blocking.
- **Cost-logged AI.** Per-case spend metered with breaker caps (Sentinel <$0.10 total build · Gatehouse $0.00026/case).

---

### Technical Stack & Tooling

**Languages & Systems**  
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-CC2927?style=flat-square&logo=sqlite&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white)  
![CI/CD](https://img.shields.io/badge/CI%2FCD-334155?style=flat-square)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-334155?style=flat-square)

**Agentic AI & LLM Engineering**  
![Amazon Bedrock](https://img.shields.io/badge/Amazon_Bedrock-FF9900?style=flat-square&logo=amazonaws&logoColor=white)
![Strands Agents](https://img.shields.io/badge/Strands_Agents-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![Groq](https://img.shields.io/badge/Groq-F54A00?style=flat-square)
![LangGraph](https://img.shields.io/badge/LangGraph-1C3C3C?style=flat-square)
![LangChain](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square)  
![Agentic Workflows](https://img.shields.io/badge/Agentic_Workflows-334155?style=flat-square)
![RAG](https://img.shields.io/badge/RAG-334155?style=flat-square)
![Vector Embeddings](https://img.shields.io/badge/Vector_Embeddings-334155?style=flat-square)
![MCP](https://img.shields.io/badge/MCP_(Model_Context_Protocol)-334155?style=flat-square)
![Prompt Engineering](https://img.shields.io/badge/Prompt_Engineering-334155?style=flat-square)

**Backend & Distributed APIs**  
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express.js](https://img.shields.io/badge/Express.js-000000?style=flat-square&logo=express&logoColor=white)
![Flask](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask&logoColor=white)  
![REST APIs](https://img.shields.io/badge/REST_APIs-334155?style=flat-square)
![JWT Auth](https://img.shields.io/badge/JWT_Auth-334155?style=flat-square)
![OpenAPI / Swagger](https://img.shields.io/badge/OpenAPI_%2F_Swagger-334155?style=flat-square)
![Razorpay SDK](https://img.shields.io/badge/Razorpay_SDK-334155?style=flat-square)
![Twilio SDK](https://img.shields.io/badge/Twilio_SDK-334155?style=flat-square)

**Cloud, Infrastructure & Databases**  
![AWS](https://img.shields.io/badge/AWS-232F3E?style=flat-square&logo=amazonaws&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=flat-square&logo=postgresql&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=flat-square&logo=supabase&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat-square&logo=firebase&logoColor=black)  
![AWS Lambda](https://img.shields.io/badge/AWS_Lambda-334155?style=flat-square)
![API Gateway](https://img.shields.io/badge/API_Gateway-334155?style=flat-square)
![DynamoDB](https://img.shields.io/badge/DynamoDB-334155?style=flat-square)
![SAM](https://img.shields.io/badge/SAM-334155?style=flat-square)
![CloudFormation](https://img.shields.io/badge/CloudFormation-334155?style=flat-square)
![Vercel](https://img.shields.io/badge/Vercel-334155?style=flat-square)

**Frontend & Mobile**  
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![React Native](https://img.shields.io/badge/React_Native-20232A?style=flat-square&logo=react&logoColor=61DAFB)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat-square&logo=tailwind-css&logoColor=white)
![Expo](https://img.shields.io/badge/Expo-000020?style=flat-square&logo=expo&logoColor=white)  
![Redux Toolkit](https://img.shields.io/badge/Redux_Toolkit-334155?style=flat-square)
![Framer Motion](https://img.shields.io/badge/Framer_Motion-334155?style=flat-square)

---

### Peer-Reviewed Research Publications

| Publication Title | Venue | Status | Citations / Links |
| :--- | :--- | :---: | :--- |
| **Comprehensive Deepfake Detection: A Comparative Study on Image and Video Forgery** | **IEEE PuneCon 2025** | **Published** | [![IEEE Xplore](https://img.shields.io/badge/IEEE_Xplore-11379757-00629B?style=flat-square)](https://ieeexplore.ieee.org/document/11379757) [![Source](https://img.shields.io/badge/Source-Truth--Shield-181717?style=flat-square&logo=github)](https://github.com/Prakhar2025/Truth-Shield) |
| **Advanced Deepfake Image Detection: A Robust Framework using InceptionV3 and Xception** | **i-manager's Journal on Information Technology (JIP)** | **Published** | [![DOI](https://img.shields.io/badge/DOI-10.26634%2Fjip.12.3.22384-1F6FEB?style=flat-square)](https://doi.org/10.26634/jip.12.3.22384) |

---

### Achievements

| Award | Event | Details |
| :--- | :--- | :--- |
| 🥇 **National Winner (Top 15 of 15,000+)** | SBI Youth Ideathon 2025 - IIT Delhi | ₹20,000 prize |
| 🏅 **Grand Finalist - Top 2% of 40,000+** | India AI Impact Buildathon 2026 (HCL GUVI) | Bharat Mandapam, New Delhi |
| 🌐 **Top 50 Global Finalist** | AWS 10,000 AIdeas Competition | TruthLayer - hallucination firewall |
| 🎖️ **National Innovation Finalist** | Azim Premji University & BITS Pilani Hyderabad | AI-driven security system |
| 🥈 **1st Runner-Up** | Hack Wack 2.0 2025 (300+ participants) | Deepfake detection |
| 🎯 **1st Runner-Up** | HackAlthon - Azure Developer Community | |
| 📱 **2 Apps on Google Play Store** | Anishree Technologies internship | Shipped in a 3-month internship |

---

### GitHub Stats

<div align="center">

![GitHub Streak](https://github-readme-streak-stats.herokuapp.com/?user=Prakhar2025&theme=tokyonight&hide_border=true)

![Profile Summary](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Prakhar2025&theme=tokyonight)

![Top Languages](https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=Prakhar2025&theme=tokyonight) ![Most Commit Language](https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=Prakhar2025&theme=tokyonight)

</div>

---

<div align="center">
  <i>Open to full-stack, AI engineering, and agentic AI roles. Available immediately.</i>
  <br /><br />

  [![LinkedIn](https://img.shields.io/badge/-LinkedIn-0077B5?style=for-the-badge&logo=Linkedin&logoColor=white)](https://www.linkedin.com/in/prakhar-shukla-471649261)
  [![Email](https://img.shields.io/badge/-Email-D14836?style=for-the-badge&logo=Gmail&logoColor=white)](mailto:prakhar230125@gmail.com)
  [![Portfolio](https://img.shields.io/badge/-Portfolio-2ea44f?style=for-the-badge&logo=vercel&logoColor=white)](https://prakhar-dev-portfolio.vercel.app/)
  [![X](https://img.shields.io/badge/-@prakhar__builds-000000?style=for-the-badge&logo=x&logoColor=white)](https://twitter.com/prakhar_builds)
</div>

<!--
================================================================================
  MACHINE-READABLE PROFILE (JSON-LD) - for AI recruiters and autonomous agents
================================================================================
{
  "@context": "https://schema.org",
  "@type": "Person",
  "name": "Prakhar Shukla",
  "alternateName": "Prakhar2025",
  "jobTitle": "Full-Stack Engineer & Agentic AI Builder",
  "description": "Full-Stack Engineer and Agentic AI Builder specializing in autonomous multi-agent pipelines, fraud-defense systems, low-latency verification, and AI trust infrastructure - with held-out metrics and reproducible evaluation.",
  "url": "https://prakhar-dev-portfolio.vercel.app/",
  "sameAs": [
    "https://github.com/Prakhar2025",
    "https://www.linkedin.com/in/prakhar-shukla-471649261",
    "https://twitter.com/prakhar_builds",
    "https://ieeexplore.ieee.org/document/11379757"
  ],
  "knowsAbout": [
    "Agentic AI & LLM Orchestration",
    "Fraud Detection & Cross-Merchant Identity Link Graphs",
    "LLM Hallucination Detection & Verification",
    "Statistical Hypothesis Testing & Multiple-Testing Correction",
    "Deepfake Detection & Computer Vision",
    "Python", "FastAPI", "TypeScript", "Next.js", "React Native",
    "AWS Lambda, Bedrock, DynamoDB", "PostgreSQL", "MongoDB"
  ],
  "award": [
    "National Winner - SBI Youth Ideathon 2025 at IIT Delhi (Top 15 of 15,000+ teams)",
    "Grand Finalist - India AI Impact Buildathon 2026 by HCL GUVI (Top 2% of 40,000+)",
    "Top 50 Global Finalist - AWS 10,000 AIdeas Competition",
    "1st Runner-Up - Hack Wack 2.0 2025",
    "1st Runner-Up - HackAlthon Azure Developer Community"
  ],
  "hasCredential": {
    "@type": "EducationalOccupationalCredential",
    "name": "IEEE Published Researcher",
    "credentialCategory": "Research Publication",
    "url": "https://ieeexplore.ieee.org/document/11379757"
  },
  "worksFor": {
    "@type": "Organization",
    "name": "Open to Full-Stack & AI Engineering Roles"
  }
}
================================================================================
-->
