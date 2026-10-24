# ProofMark AI

**An evidence-first brand content governance tool**

## About the Project
ProofMark AI helps marketing teams check draft content against approved brand facts before human review. It identifies claims that are supported, conflicting, insufficiently evidenced, or missing relevant guidelines.

## Key Features
- **Brand Fact Store:** Add and manage approved brand facts.
- **Content Checker:** Analyze marketing copy using four classifications.
- **Evidence Traceability:** Link findings to relevant fact IDs.
- **Human Review:** Approve, request changes, or reject content.
- **Audit Trail:** Record review actions and timestamps.
- **Draft Versioning:** Re-check edited content before reviewing it again.
- **Guideline Gap Intelligence:** Identify missing guidance and suggest action items.
- **AI and Offline Support:** Gemini integration with rule-based fallback.

## Technology Used
- HTML
- CSS
- JavaScript
- Google Gemini API
- Browser localStorage for application data

## How to Run
1. Download or clone this repository.
2. Open the `app` folder.
3. Open `index.html` in a web browser.
4. Use the offline rule-based checking mode, or configure a Gemini API key in the app settings if available.

## Demo Scenario
The NovaSound example demonstrates how the tool evaluates claims about headphone battery life, brand trust, and intended use against stored facts.

## Important Notes
- ProofMark AI supports human review; it does not automatically publish marketing content.
- Missing evidence does not automatically mean a claim is false.
- A Gemini API key entered in the browser is stored client-side. Do not use a sensitive or production API key in a publicly deployed client-side application.

## Team — Innovators
- Saloni Chipde
- Pranjali Bakde
- Aarti Shende
- Riddhi Koche

**Project:** ProofMark AI — Round 2 Build
