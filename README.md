# academic-paper-writing — Academic Research Paper Writing Skill

A Claude Agent Skill that embeds a comprehensive set of academic research paper writing rules, constraints, and review checklists directly into the model's workflow.

Instead of merely explaining writing concepts, this Skill enables Claude to actively apply academic writing standards while helping users draft, revise, critique, and evaluate research papers.

> The guidance in this Skill is independently distilled and rewritten from the Sacred Heart University Library research guide *Organizing Academic Research Papers* (itself based on materials by Dr. Robert V. Labaree of USC Libraries). No original text is reproduced. See [`NOTICE`](./NOTICE) for attribution and copyright information.

---

## ✨ Features

### Core Academic Writing Principles

Applies a consistent set of academic writing standards throughout the entire paper, including:

* Research-question-driven structure
* Thesis-first argumentation
* Evidence-based reasoning
* Formal and precise academic tone
* Careful use of terminology
* Proper attribution of all non-original ideas and materials

### Section-Specific Guidance

Provides detailed constraints and review criteria for the major components of an academic paper:

* Research Design
* Topic Selection & Research Questions
* Title
* Outline Development
* Paragraph Construction
* Abstract
* Introduction
* Literature Review
* Methodology
* Results
* Discussion
* Limitations
* Conclusion
* Proofreading & Editing
* Citation Practices & Plagiarism Prevention

### On-Demand Reference Materials

Includes two supplementary reference documents:

* Academic style, grammar, citation, and plagiarism guidance
* Detailed section-level explanations, frameworks, and classifications

### Final Submission Checklist

A comprehensive quality-control checklist for evaluating a manuscript before submission.

---

## 🎯 When It Activates

This Skill is automatically relevant whenever you are planning, drafting, revising, reviewing, or grading:

* Research papers
* Journal articles
* Thesis or dissertation chapters
* Course papers
* Research proposals
* Literature reviews

Examples:

* "Can you review my abstract?"
* "Is this a strong research question?"
* "Help tighten the discussion section."
* "What should be included in the methodology?"
* "Make this paragraph more academic."
* "How can I avoid plagiarism here?"

When such tasks arise, Claude can apply the Skill's writing constraints directly to the work rather than merely describing best practices.

---

## 📦 Repository Structure

```text
academic-paper-writing-skill/
├── README.md
├── LICENSE
├── NOTICE
├── .gitignore
├── academic-paper-writing/
│   ├── SKILL.md
│   └── references/
│       ├── section-reference.md
│       └── style-grammar-citation.md
└── dist/
    └── academic-paper-writing.skill
```

### Contents

* **SKILL.md** — Main workflow, principles, section-level constraints, and review checklist
* **section-reference.md** — Detailed guidance for individual paper sections
* **style-grammar-citation.md** — Academic style, grammar, citation, and plagiarism reference
* **academic-paper-writing.skill** — Packaged skill ready for installation

---

## 🚀 Installation

### Option 1: Install the Packaged Skill (Recommended)

1. Download [`dist/academic-paper-writing.skill`](./dist/academic-paper-writing.skill).
2. Open Claude.
3. Navigate to **Settings → Capabilities → Skills**.
4. Upload the `.skill` file.

### Option 2: Use the Source Files

Place the entire `academic-paper-writing/` directory into your Skills directory, or load it according to the documentation of Claude Code, Claude Desktop, or other compatible Claude environments.

To package the Skill yourself:

```bash
python -m scripts.package_skill <skill-directory> <output-directory>
```

---

## 🧩 Scope

This Skill focuses on the core academic paper writing workflow distilled from approximately 22 pages of the original guide.

The following content categories were intentionally excluded:

* Oral presentation guidance
* Group project management
* Book reviews
* Field reports
* Policy memos
* Glossaries and resource indexes
* Content alert services
* Supplemental reading lists

These topics may be added in future contributions if needed.

---

## 📚 Attribution

Source materials:

* Sacred Heart University Library — *Organizing Academic Research Papers*
* USC Libraries — Dr. Robert V. Labaree, *Organizing Your Social Sciences Research Paper*

This repository contains an independent reinterpretation, synthesis, and rewrite of the underlying guidance for educational and research-assistance purposes. Proper attribution to the original institutions and authors is maintained.

See [`NOTICE`](./NOTICE) for details.

---

## 📄 License

The original wording, structure, packaging, and implementation contained in this repository are released under the MIT License.

Please note that the MIT License applies only to the repository author's original contributions and does not grant rights to any underlying copyrighted source materials.

Review [`NOTICE`](./NOTICE) before redistribution or reuse. This repository does not provide legal advice.

---

## 🤝 Contributing

Contributions are welcome.

Feel free to submit Issues or Pull Requests to:

* Improve wording or guidance
* Add new academic writing constraints
* Expand section-specific coverage
* Correct mistakes or inconsistencies

Please avoid copying substantial portions of the original source material. All contributions should follow the project's principle of independent summarization and reinterpretation.
