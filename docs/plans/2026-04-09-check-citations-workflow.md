# Check Citations Workflow Implementation Plan

> **For Claude:** REQUIRED SUB-SKILL: Use superpowers:executing-plans to implement this plan task-by-task.

**Goal:** Implement a specialized workflow to verify the existence of academic citations and identify their Qualis rating (SBC/CAPES).

**Architecture:** A multi-step workflow (`workflows/check-citations.md`) that guides the AI agent to use search tools (Google Scholar/Web) to validate papers and consult official/community datasets for Qualis classification.

**Tech Stack:** Markdown (Workflow), AI Search Tools, BibTeX validation.

---

### Task 1: Update Reference Knowledge

**Files:**
- Modify: `references/qualis-guide.md`
- Modify: `references/citation-methods.md`

**Step 1: Add new Qualis 2025-2028 rules to guide**
Update `references/qualis-guide.md` with the new focus on bibliometric metrics (h5-index for conferences and CiteScore for journals).

**Step 2: Update citation methods with BibTeX best practices**
Ensure `references/citation-methods.md` includes instructions on how to validate a BibTeX entry against search results.

---

### Task 2: Create the Check Citations Workflow

**Files:**
- Create: `workflows/check-citations.md`

**Step 1: Define the intake phase**
Create the `<intake>` section to ask for the citation (Raw text, BibTeX, or Title/Author).

**Step 2: Define the verification process**
Create the `<process>` section with 4 steps:
1. **Search:** Use `google_web_search` to find the paper on Google Scholar/DBLP.
2. **Venue ID:** Extract the name of the Journal or Conference.
3. **Qualis Lookup:** Search for the venue's Qualis on Sucupira or PPGCC/PUCRS tool.
4. **BibTeX Sync:** Generate or correct the BibTeX entry based on found data.

**Step 3: Define success criteria**
Add `<success_criteria>` including "Paper verified", "Venue identified", and "BibTeX validated".

---

### Task 3: Integrate into Main Skill Router

**Files:**
- Modify: `SKILL.md`

**Step 1: Add new option to Intake**
Add "8. **Verificar citações** — Quero validar se uma referência existe e checar seu Qualis" to the `<intake>` list.

**Step 2: Update Routing table**
Add the mapping for option 8 to `workflows/check-citations.md`.

---

### Task 4: Final Validation (Dogfooding)

**Step 1: Run verification test**
Test the workflow by asking: "Verifique a citação: 'Attention is All You Need', Vaswani et al. 2017. Qual o Qualis da conferência?"
Expected: AI finds the paper (NIPS/NeurIPS) and identifies its high impact (Qualis A1).

**Step 2: Commit and Push**
Final commit with all changes.
