# EPC Platform — Smart Support Agent

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10%2B-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
  <img src="https://img.shields.io/badge/Google-Cloud-4285F4?style=for-the-badge&logo=googlecloud&logoColor=white" alt="Google Cloud" />
  <img src="https://img.shields.io/badge/AI-Agent-Workflow-8A2BE2?style=for-the-badge" alt="AI Agent Workflow" />
  <img src="https://img.shields.io/badge/Status-Prototype-34A853?style=for-the-badge" alt="Status" />
</p>

> AI-powered support operations for enterprise incident triage, clustering, similarity search, and escalation preparation.

A lightweight but practical multi-agent system for turning noisy support tickets into structured, actionable operational signals.

## Why this project exists

Support teams often get buried in repetitive tickets, duplicate reports, and slow escalations. This project helps by:

- grouping related issues into clusters
- finding similar historical incidents
- scoring business and operational impact
- assigning the right handling path
- preparing escalation-ready summaries for teams and admins

---

## What it does

```text
Support Tickets
      ↓
  Meaning Extraction
      ↓
   Ticket Clustering
      ↓
  Similar Incident Search
      ↓
    Impact Scoring
      ↓
  Escalation Prep
      ↓
  Admin Review / Workflow Action
```

This is a practical EPC-style workflow for enterprise problem consolidation.

---

## Core capabilities

- Smart classification of raw support text
- Duplicate and near-duplicate ticket grouping
- Historical incident lookup using retrieval patterns
- Risk and impact prioritization
- Escalation summaries for human review
- Admin panel for approving or rejecting clustered issues
- Guardrails around both input and output safety

---

## Project structure

```text
smart-support-agent/
├── agents/                  # Agent logic for extraction, clustering, impact scoring, escalation
├── data/                   # Sample tickets, incident snapshots, generated outputs
├── deployment/             # Workflow service and admin review panel
├── guardrails/             # Input/output validation checks
├── integrations/           # Gmail, Drive, Discord, MCP-related integrations
├── memory/                 # Firestore / BigQuery migration helpers
├── rag/                    # Embeddings and retrieval workflow
├── testing/                # Batch extraction and validation scripts
├── requirements.txt        # Python dependency list
├── help.md                 # Setup notes
├── Dockerfile              # Container setup
├── deploy_*.sh             # Deployment helpers
└── README.md               # Project overview
```

---

## Tech stack

This project brings together a practical set of tools for AI-powered support operations:

- Python for agent logic and orchestration
- Google Cloud services for storage, data access, and deployment workflows
- Firestore and BigQuery for structured operational memory
- Retrieval and embedding-based lookup for similar incident matching
- Gradio for a lightweight admin review interface
- Gmail, Drive, Discord, and MCP integrations for real-world support workflows
- Guardrails for safer input and output handling

---

## Typical workflow

1. Feed support ticket data into the extraction pipeline.
2. Normalize and structure the issue details.
3. Cluster similar tickets together.
4. Pull related historical incidents using retrieval methods.
5. Score impact and urgency.
6. Send review-ready escalation material to admins or downstream systems.

---

<p align="center">
  <strong>Built for better support signal detection, faster incident understanding, and cleaner escalation workflows.</strong>
</p>
