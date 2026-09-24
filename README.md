# Foundry IQ RAG Playbook

A hands-on playbook for building, securing, and tuning Retrieval-Augmented Generation (RAG) and multi-agent solutions with **Microsoft Foundry IQ**, **Azure AI Search**, and **Microsoft Fabric**.

This repository is based on the official Microsoft TechLab **[Building Intelligent Solutions with Microsoft Foundry IQ](https://github.com/microsoft/TechLab-Building-Intelligent-Solutions-with-Microsoft-Foundry-IQ)**. The official lab is the source of truth for the scenario and the step-by-step instructions. This playbook adds what we learned by reproducing the lab end to end in a customer-like environment: a private-network AI Landing Zone, plus demos focused on RAG accuracy, freshness, and evaluation.

> **Lab assets:** the files that ship with the official TechLab environment (notebook, ontology package, agent scripts, and documents) are available in [`lab-assets/`](lab-assets/). Synthetic data created for this playbook is in [`data/`](data/).

---

## Lab overview

![Foundry IQ solution architecture](https://github.com/microsoft/TechLab-Building-Intelligent-Solutions-with-Microsoft-Foundry-IQ/raw/main/Media/FIQArchi.png)

*Architecture diagram from the official Microsoft TechLab.*

The lab shows how **Foundry IQ** acts as a single intelligence layer that turns enterprise data and knowledge into trusted, business-aware actions performed by AI agents.

The story follows **Zava**, a fictional retailer that runs hundreds of physical stores and a growing online store. Zava has plenty of data, but its leadership struggles to turn it into timely decisions:

- Business knowledge is spread across many systems and documents.
- Insights arrive too late to influence decisions in the moment.
- AI solutions lack a shared understanding of business terms and rules.
- There is no common business language to guide AI agents during critical periods, such as the holiday sales season.

To solve this, Zava adopts Foundry IQ as the foundation that connects business context, enterprise knowledge, and AI execution.

---

## Personas in the scenario

| Persona | Role | What they care about |
|---|---|---|
| **April** | Chief Executive Officer | Revenue, growth, and customer experience |
| **Rupesh** | Chief Data Officer | Business definitions, data governance, and trust |
| **Miguel** | AI Engineer / Data Scientist | Designing intelligent and well-governed AI agents |
| **Ryan** | End customer | The experience he gets from AI-driven decisions |

---

## Foundry IQ: from business intelligence to intelligent action

Instead of letting agents reason over raw data or assumptions, Foundry IQ grounds them in **shared business definitions, policies, and enterprise knowledge**. This keeps agent behavior aligned with how the business actually operates and reduces guesses and hallucinations.

In the lab, you build and observe:

- A **Supervisor Agent** that routes each request to the right specialist.
- **Specialized agents** for sales assistance, loyalty and rewards campaigns, and inventory.
- **Knowledge grounding** with Foundry IQ over enterprise documents, product catalogs, and policies.
- **Tool calling** to a Microsoft Fabric Data Agent for structured business data.
- **Governed, observable, and auditable** agents, with guardrails, tracing, and evaluations.

### End-to-end scenario: holiday sales at Zava

During a high-pressure holiday sales period, the agents work together:

- The **Sales Associate Agent** recommends products from the catalog.
- The **Rewards Campaign Agent** applies loyalty tiers and personalized discounts.
- The **Inventory Agent** checks stock levels and stockout risk in the Fabric Lakehouse.

Every decision is traceable, observable, and governed.

### What the lab demonstrates

- A shared business language for AI.
- Agent reasoning grounded in enterprise knowledge and governance.
- Safe, collaborative, multi-agent execution.
- The journey from insight, to intelligence, to action.

---

## What this playbook adds

| Area | What you will find here |
|---|---|
| **Private networking** | How we ran the lab inside an AI Landing Zone with private endpoints, agent network injection, shared private links, and centralized private DNS |
| **Troubleshooting** | Real issues we hit and how we fixed them (DNS, identities, permissions, policies) |
| **RAG quality** | Hands-on demos on accuracy, data freshness, and structured vs. unstructured data |
| **Evaluation** | How to measure RAG quality instead of guessing |

*Content is being added incrementally.*

---

## References

- Official lab: [microsoft/TechLab-Building-Intelligent-Solutions-with-Microsoft-Foundry-IQ](https://github.com/microsoft/TechLab-Building-Intelligent-Solutions-with-Microsoft-Foundry-IQ)
- Companion lab: [microsoft/TechLab-Building-Intelligent-Solutions-with-Microsoft-Work-IQ](https://github.com/microsoft/TechLab-Building-Intelligent-Solutions-with-Microsoft-Work-IQ)
