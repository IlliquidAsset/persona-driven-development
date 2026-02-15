# Persona-Driven Development (PDD)

> **"The Persona is the Mold. The Software is the Clay."**

**Author:** Kendrick Kirk, MBA, CPEP, Managing Director Kirk+Co Advisory

**Connect:** [LinkedIn](https://linkedin.com/in/kkirk) | [X/Twitter](https://x.com/KendrickCreate_) | [GitHub](https://github.com/IlliquidAsset)

---

## Overview

Persona-Driven Development (PDD) is a methodology for building AI-driven software through deep, executable personas. Rather than abstract user stories, PDD uses **CIA-Legend depth personas** as living specifications that guide every architectural decision, API design, and feature implementation.

This repository contains the complete PDD framework, including the foundational methodology, the academic SPDD paper on System Legends for APIs, and 10 real-world persona examples from Real Estate Private Equity.

---

## Quick Navigation

| Resource | Description |
|----------|-------------|
| **[Persona-Driven Development Playbook](methodology/persona-driven-development.md)** | The 8-step core methodology for implementing PDD |
| **[Extended Methodology & Literature Review](methodology/extended-methodology.md)** | Deep dive into PDD theory, research foundations, and advanced patterns |
| **[Persona Template (Master)](methodology/persona-template.md)** | Complete template for creating new personas |
| **[SPDD Paper: System Legends for APIs](paper/spdd-paper.md)** | Academic paper on System Legends for Persona-Driven Development |
| **[Persona Examples](personas/)** | 10 real-world personas from Real Estate Private Equity |

---

## What is Persona-Driven Development?

PDD inverts traditional software development. Instead of starting with requirements and building personas afterward, PDD:

1. **Creates deep, executable personas** with 5 dimensions of System Legend depth
2. **Uses personas as specifications** that drive architecture, API design, and feature prioritization
3. **Treats personas as living documents** that evolve with the product
4. **Enables AI systems** to understand context, intent, and constraints at a human level

### The 8-Step Playbook

1. **Define Core Personas** - Identify the 3-5 primary user archetypes
2. **Build System Legends** - Create 5-dimensional depth profiles for each persona
3. **Map Workflows** - Document how each persona interacts with the system
4. **Design APIs** - Build APIs that speak the language of each persona
5. **Implement Features** - Develop features guided by persona needs
6. **Test with Personas** - Validate against persona workflows, not just requirements
7. **Iterate & Evolve** - Update personas as the product and market evolve
8. **Scale Across Teams** - Distribute personas as shared mental models

---

## The PDD Visual Summary

![Persona-Driven Development Infographic](assets/pdd-infographic.png)

*The infographic above illustrates the core PDD concept: treating software as clay and personas as molds to erase "happy path" bias. It visualizes the 15% corruption gap in legacy system integrations and how System Legends (high-fidelity personas) reduce data corruption to 0% by forcing AI to implement defensive programming patterns.*

---

## What is SPDD (System Legends for Persona-Driven Development)?

SPDD extends PDD by formalizing **System Legends** — the 5-dimensional depth profiles that make personas executable:

### The 5 Dimensions of System Legend

1. **Cognitive Model** - How the persona thinks about problems, constraints, and solutions
2. **Operational Context** - The real-world environment, tools, and workflows
3. **Decision Criteria** - What matters most: speed, accuracy, compliance, cost, risk?
4. **Integration Points** - How this persona connects to other personas and systems
5. **Failure Modes** - What breaks the persona's workflow? What are the consequences?

These dimensions transform personas from marketing artifacts into **executable specifications** that guide:
- API design (endpoints, parameters, error handling)
- Feature prioritization (what solves real problems?)
- Architecture decisions (what scales for this persona's needs?)
- AI system prompts (how should the system reason about this persona's context?)

---

## Why This Matters: The Pro Forma Analogy

In finance, a **pro forma** is a forward-looking financial statement that guides investment decisions. It's not a prediction—it's a model of how the business *should* work.

**Personas are the pro formas of software development.**

Just as investors use pro formas to:
- Understand business assumptions
- Identify key value drivers
- Test sensitivity to changes
- Communicate strategy to stakeholders

**PDD uses personas to:**
- Clarify product assumptions
- Identify critical user workflows
- Test feature impact on different user types
- Align teams around shared mental models

Without personas, software development is like investing without pro formas: reactive, misaligned, and prone to building the wrong thing.

---

## Real-World Example: Real Estate Private Equity

This repository includes 10 personas from a real estate private equity platform:

- **Investor** - LP seeking returns and transparency
- **Finance** - CFO managing capital calls and distributions
- **IR (Investor Relations)** - Communicating with LPs
- **Lender** - Debt provider managing covenants
- **PM (Portfolio Manager)** - Acquiring and managing assets
- **BD (Business Development)** - Sourcing deals
- **Admin** - Operational support and compliance
- **Analyst** - Due diligence and underwriting
- **Underserved** - Emerging market participants
- **Internal Power** - Executive decision-making

Each persona includes:
- **Role & Responsibilities** - What they do
- **Goals & Constraints** - What matters to them
- **Workflows** - How they interact with the system
- **System Legend** - The 5-dimensional depth profile
- **API Needs** - What endpoints and data they require
- **Failure Modes** - What breaks their workflow

---

## Related Work

PDD builds on established research in user-centered design and domain-driven development:

- **[TSCL (Task-Specific Cognitive Load)](https://example.com)** - Understanding how personas process information
- **[TSRL (Task-Specific Role Learning)](https://example.com)** - How personas learn and adapt to new systems

---

## Getting Started

1. **Read the [Persona-Driven Development Playbook](methodology/persona-driven-development.md)** to understand the core methodology
2. **Review the [SPDD Paper](paper/spdd-paper.md)** for the theoretical foundation
3. **Study the [Persona Examples](personas/)** to see PDD in practice
4. **Use the [Persona Template](methodology/persona-template.md)** to create personas for your own product

---

## Citation

If you use PDD or SPDD in your work, please cite:

```bibtex
@article{kirk2024pdd,
  title={Persona-Driven Development: Using System Legends as Executable Specifications},
  author={Kirk, Kendrick},
  year={2024},
  organization={Kirk+Co Advisory}
}

@article{kirk2024spdd,
  title={SPDD: System Legends for Persona-Driven Development},
  author={Kirk, Kendrick},
  year={2024},
  organization={Kirk+Co Advisory}
}
```

---

## License

This work is provided as-is for educational and commercial use. Attribution to Kendrick Kirk and Kirk+Co Advisory is appreciated.

---

## Questions or Feedback?

Connect with Kendrick Kirk:
- **LinkedIn:** [linkedin.com/in/kkirk](https://linkedin.com/in/kkirk)
- **X/Twitter:** [@KendrickCreate_](https://x.com/KendrickCreate_)
- **GitHub:** [github.com/IlliquidAsset](https://github.com/IlliquidAsset)

---

**Last Updated:** February 2026
