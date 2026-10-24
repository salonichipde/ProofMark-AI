# ProofMark AI
### An Evidence-First Brand Content Governance Tool

**Live Demo:** https://salonichipde.github.io/ProofMark-AI/proofmark.html  
**Source Code:** https://github.com/salonichipde/ProofMark-AI

## 1. Problem Statement

Marketing teams need to create content that is accurate, trustworthy, and consistent with approved brand information. However, unsupported claims, outdated facts, and missing guidelines can lead to misleading content and reduce customer trust.

ProofMark AI addresses this problem by checking marketing content against approved brand facts and supporting human review before content is finalized.

## 2. Our Solution

ProofMark AI is a lightweight, evidence-first content governance tool. It helps teams identify unsupported or conflicting claims, trace findings to approved evidence, review risks, and maintain an audit trail of content decisions.

The system combines rule-based checking with optional Google Gemini API integration and keeps human reviewers responsible for final approval.

## 3. Key Features

- **Brand Fact Store:** Create, update, and manage approved brand facts.
- **Content Checker:** Classify claims as Supported, Conflicting, Insufficient Evidence, or Guideline Gap.
- **Evidence Traceability:** Connect content findings to relevant fact IDs.
- **Smart Claim Analyzer:** Break complex marketing copy into individual claims and suggest evidence-based rewrites.
- **Claim Impact Radar:** Identify previously checked claims that may be affected when a brand fact changes.
- **Smart Risk Radar:** Organize findings into explainable risk levels to help reviewers prioritize their work.
- **Human Review Workflow:** Approve content, request changes, or reject it.
- **Audit Trail and Versioning:** Track review actions and require rechecking after relevant edits.
- **Guideline Gap Intelligence:** Highlight missing guidance and suggest possible action items for review.
- **Trust Passport Hub:** Generate a report containing a content snapshot, evidence references, review information, and risk summary. Export reports as HTML or JSON, or use the print dialog to save a PDF.
- **AI and Offline Support:** Use optional Gemini integration or the built-in rule-based checking mode.

## 4. End-to-End Workflow

1. Add approved brand facts to the Brand Fact Store.
2. Enter marketing copy into the Content Checker.
3. Review the classification and supporting evidence for each claim.
4. Use Smart Claim Analyzer to examine individual claims and suggest grounded wording.
5. Check the Claim Impact Radar when relevant brand facts change.
6. Use Smart Risk Radar to prioritize findings that need attention.
7. Recheck edited content and send it through human review.
8. Generate a Trust Passport report to summarize the reviewed content and its evidence.

## 5. Technology Stack

- **Frontend:** HTML, CSS, JavaScript
- **AI Integration:** Google Gemini API (optional)
- **Offline Checking:** Rule-based JavaScript logic
- **Data Storage:** Browser localStorage
- **Deployment:** GitHub Pages

The current application is a lightweight browser-based project and does not require a separate backend server or a package installation to run.

## 6. Demo Scenario

The project includes a NovaSound headphone example with brand facts such as battery life.

For example:

- **Approved claim:** “NovaSound headphones offer up to 12 hours of battery life on a single charge.”
- **Conflicting claim:** “NovaSound headphones offer up to 20 hours of battery life on a single charge.”

The checker compares these claims with the stored brand evidence. The Smart Claim Analyzer can suggest grounded wording, after which the revised content can be checked again before review.

## 7. Testing and Validation

The following workflows were manually tested during development:

- A claim matching the approved 12-hour battery fact was classified as Supported.
- A claim stating 20 hours was classified as Conflicting.
- Applying a grounded rewrite and checking the revised claim again returned Supported.
- Changing the NS-01 battery-life fact from 10 to 12 hours caused the Claim Impact Radar to flag affected claims for review.
- Smart Risk Radar opened and displayed risk information.
- Trust Passport generation, HTML and JSON exports, and the print/PDF workflow were tested.

These are manual test observations, not a guarantee that every possible claim will be classified correctly.

## 8. Limitations and Responsible Use

- Automated checking can miss context, wording variations, or complex claims.
- AI-generated suggestions should be reviewed before use.
- Results depend on the quality and completeness of the approved brand facts.
- Browser localStorage keeps data in the current browser and is not a shared team database.
- The client-side audit trail is not tamper-proof and should not be treated as a secure compliance record.
- A Trust Passport is an internal evidence and review report, not an independent certification.
- A Gemini API key entered in a browser-based app may be exposed to users of that browser or application. Do not place a sensitive production key in a public client-side deployment.

ProofMark AI supports human decision-making; it does not automatically publish marketing content.

## 9. How to Run Locally

1. Clone or download this repository.
2. Open the `app` folder.
3. Open `index.html` in a modern web browser.
4. Select **Load Demo Data** to try the NovaSound example.
5. Test the checking, analysis, review, risk, and report workflows.

The rule-based mode can be used without configuring Gemini. Gemini integration requires a valid API key and network access.

## 10. Team — Innovators

- Saloni Chipde
- Pranjali Bakde
- Aarti Shende
- Riddhi Koche

**Project:** ProofMark AI — Round 2 Build
