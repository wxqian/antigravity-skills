# Antigravity Skills User Manual

**Document Version:** v2.0.1  
**Total Skills:** 46

This document provides a detailed introduction to all available Skills in the current workspace. These Skills offer a wide range of capabilities, from document processing and artistic creation to full-stack development and testing.

You can invoke these skills in dialogue via `@[skill-name]` or `/skill-name`.

---

## Table of Contents

1. [Algorithmic Art](#1-algorithmic-art)
2. [Brand Guidelines](#2-brand-guidelines)
3. [Canvas Design](#3-canvas-design)
4. [Doc Co-authoring](#4-doc-co-authoring)
5. [DOCX (Word Processing)](#5-docx-word-processing)
6. [Frontend Design](#6-frontend-design)
7. [Internal Comms](#7-internal-comms)
8. [NotebookLM (Knowledge Base Q&A)](#8-notebooklm-knowledge-base-qa)
9. [MCP Builder (MCP Server Construction)](#9-mcp-builder-mcp-server-construction)
10. [PDF Processing](#10-pdf-processing)
11. [PPTX (Presentations)](#11-pptx-presentations)
12. [Skill Creator](#12-skill-creator)
13. [Slack GIF Creator](#13-slack-gif-creator)
14. [Theme Factory](#14-theme-factory)
15. [Web Artifacts Builder](#15-web-artifacts-builder)
16. [Webapp Testing](#16-webapp-testing)
17. [XLSX (Excel Processing)](#17-xlsx-excel-processing)
18. [UI/UX Pro Max](#18-uiux-pro-max)
19. [Brainstorming](#19-brainstorming)
20. [Dispatching Parallel Agents](#20-dispatching-parallel-agents)
21. [Executing Plans](#21-executing-plans)
22. [Finishing a Development Branch](#22-finishing-a-development-branch)
23. [Receiving Code Review](#23-receiving-code-review)
24. [Requesting Code Review](#24-requesting-code-review)
25. [Subagent Driven Development](#25-subagent-driven-development)
26. [Systematic Debugging](#26-systematic-debugging)
27. [Test Driven Development (TDD)](#27-test-driven-development-tdd)
28. [Using Git Worktrees](#28-using-git-worktrees)
29. [Using Superpowers](#29-using-superpowers)
30. [Verification Before Completion](#30-verification-before-completion)
31. [Writing Plans](#31-writing-plans)
32. [Writing Skills](#32-writing-skills)
33. [Planning with Files](#33-planning-with-files)
34. [BDI Mental States](#34-bdi-mental-states)
35. [Memory Systems](#35-memory-systems)
36. [Filesystem Context](#36-filesystem-context)
37. [Context Fundamentals](#37-context-fundamentals)
38. [Context Optimization](#38-context-optimization)
39. [Context Compression](#39-context-compression)
40. [Context Degradation](#40-context-degradation)
41. [Multi-Agent Patterns](#41-multi-agent-patterns)
42. [Hosted Agents](#42-hosted-agents)
43. [Tool Design](#43-tool-design)
44. [Project Development](#44-project-development)
45. [Evaluation (Basic)](#45-evaluation-basic)
46. [Advanced Evaluation](#46-advanced-evaluation)

---

### 1. Algorithmic Art

**Invocation**: `@[algorithmic-art]` or `/algorithmic-art`

**Description**:
Focuses on code-based generative art creation. It uses the p5.js library to create unique visual experiences through controlled randomness and mathematical algorithms, rather than simply copying existing art.

**Core Capabilities**:
- **Create Algorithmic Philosophy**: Define unique aesthetic concepts for generative art (e.g., "Organic Turbulence", "Quantum Harmonics").
- **Generate Interactive Art**: Create HTML widgets containing parameter controls and seed navigation, supporting real-time exploration and variant generation.
- **Professional Craftsmanship**: Emphasize fine-tuning, color harmony, and algorithmic depth.

**Use Case**:
> **User**: "Please create a generative art background named 'Digital Pulse' for a tech conference, reflecting data flow and connectivity."
>
> **Skill Response**:
> 1. Create a "Digital Pulse" algorithmic philosophy document defining visual rules (particle flow, network connections, neon colors).
> 2. Generate an interactive HTML piece with adjustable parameters like "Flow Speed" and "Connection Density".

---

### 2. Brand Guidelines

**Invocation**: `@[brand-guidelines]` or `/brand-guidelines`

**Description**:
Provides Anthropic's official brand visual identity guidelines to ensure generated documents, presentations, or designs comply with brand standards.

**Core Capabilities**:
- **Color Specifications**: Provides official color palettes (Dark background #141413, accent color #d97757, etc.).
- **Typography Specifications**: Guides the use of Poppins (headings) and Lora (body) fonts.
- **Style Application**: Applies brand elements to various Artifacts.

**Use Case**:
> **User**: "Help me beautify this slide deck using Anthropic's brand style."
>
> **Skill Response**:
> Applies official color schemes (Warm Dark or Light mode), adjusts fonts to Poppins/Lora, and standardizes chart colors.

---

### 3. Canvas Design

**Invocation**: `@[canvas-design]` or `/canvas-design`

**Description**:
Used for creating high-quality static visual designs (posters, art pieces, covers). Emphasizes minimalism, typography design, and visual philosophy.

**Core Capabilities**:
- **Design Philosophy Creation**: Define a visual language (e.g., "Brutalist Joy", "Geometric Silence").
- **Canvas Creation**: Generate high-precision design work in PDF or PNG format.
- **Font Management**: Support for loading custom fonts to enhance typographic quality.

**Use Case**:
> **User**: "Design a minimalist poster about the 'City of the Future'."
>
> **Skill Response**:
> 1. Conceptualize the "Concrete Future" design philosophy (emphasizing negative space, brutalist lines).
> 2. Generate a poster PDF containing architectural geometries and fine typography.

---

### 4. Doc Co-authoring

**Invocation**: `@[doc-coauthoring]` or `/doc-coauthoring`

**Description**:
Assists users in writing high-quality documents (e.g., PRDs, design docs, proposals) through a structured guidance process.

**Core Capabilities**:
- **Context Collection**: Uncover user intent and background information through targeted questions.
- **Structured Drafting**: Brainstorm, filter, and write section by section.
- **Reader Perspective Testing**: Review the document from a reader's perspective to identify blind spots.

**Use Case**:
> **User**: "I need to write a PRD for a new feature."
>
> **Skill Response**:
> 1. Guide the user in answering questions about target users, core features, and constraints.
> 2. Propose a PRD structure (Background, Goals, Solution, Metrics).
> 3. Assist in writing and refining content chapter by chapter.

---

### 5. DOCX (Word Processing)

**Invocation**: `@[docx]` or `/docx`

**Description**:
Handles the creation, editing, and analysis of Word documents. Supports complex Track Changes modes and underlying XML editing.

**Core Capabilities**:
- **Document Reading**: Extract text or convert to Markdown for analysis.
- **Redlining**: Plan and implement batch revisions (Track Changes), suitable for contract or thesis modifications.
- **OOXML Editing**: Directly manipulate underlying XML to handle complex formatting.
- **New Document Creation**: Build documents from scratch using `docx-js`.

**Use Case**:
> **User**: "Review this contract `contract.docx`, change all '30-day' terms to '60 days', and enable Track Changes."
>
> **Skill Response**:
> 1. Read the document and locate all "30-day" mentions.
> 2. Use underlying scripts to batch-replace text and mark `<w:ins>` (insert) and `<w:del>` (delete) tags.
> 3. Generate a new document with revision history.

---

### 6. Frontend Design

**Invocation**: `@[frontend-design]` or `/frontend-design`

**Description**:
Builds frontend interfaces with unique aesthetics and production-grade quality. Avoids generic AI aesthetics, pursuing unique visual styles.

**Core Capabilities**:
- **Aesthetic Design**: Select unique themes (e.g., "Retro Futurism", "Magazine Layout style").
- **Code Implementation**: Generate React/HTML/CSS code with delicate animations and interactions.
- **Visual Differentiation**: Use non-standard fonts, unique layouts, and color schemes.

**Use Case**:
> **User**: "Create a landing page for a new coffee brand."
>
> **Skill Response**:
> Design a page with deep brown and cream tones, combined with serif fonts and parallax scrolling effects, reflecting premium artisanal quality.

---

### 7. Internal Comms

**Invocation**: `@[internal-comms]` or `/internal-comms`

**Description**:
Drafts internal communication materials following corporate standards, such as weekly reports, announcements, FAQs, etc.

**Core Capabilities**:
- **Template Application**: Includes standard formats like 3P (Progress, Plans, Problems), Newsletters, etc.
- **Style Adaptation**: Ensures a professional tone that is clear and consistent with company culture.

**Use Case**:
> **User**: "Write an internal announcement about system maintenance next week."
>
> **Skill Response**:
> Uses a standard announcement template including time, impact scope, recommended actions, and contact info, with a formal yet considerate tone.

---

### 8. NotebookLM (Knowledge Base Q&A)

**Invocation**: `@[notebooklm]` or `/notebooklm`

**Description**:
Directly queries Google NotebookLM notebooks to obtain definitive answers grounded in documentation with citations. Effectively reduces hallucinations through browser-automated knowledge base interaction.

**Core Capabilities**:
- **Knowledge Retrieval**: Extract precise information from user-uploaded document sources (PDF, text, etc.).
- **Citation Sourcing**: Provides clear citations from the original text for the answers.
- **Persistent Authentication**: Manages browser sessions to maintain login status.

**Use Case**:
> **User**: "Based on our RAG technical white paper, explain the retrieval re-ranking strategy."
>
> **Skill Response**:
> 1. Automatically connect to the "RAG Research" notebook in NotebookLM.
> 2. Input the query and obtain a cited answer.
> 3. Return: "According to page 12 of the white paper, Strategy A is superior to B..." [Source 1]

---

### 9. MCP Builder (MCP Server Construction)

**Invocation**: `@[mcp-builder]` or `/mcp-builder`

**Description**:
Guides users in building Model Context Protocol (MCP) servers, enabling LLMs to connect with external data or tools.

**Core Capabilities**:
- **Architecture Planning**: Determine Resources, Tools, and Prompts.
- **Code Scaffolding**: Provide implementation guidance using Python (FastMCP) or TypeScript SDK.
- **Testing & Evaluation**: Generate test cases to verify MCP services.

**Use Case**:
> **User**: "I want to create an MCP server that can check weather data."
>
> **Skill Response**:
> 1. Plan the input/output schema for the `get_weather` tool.
> 2. Provide a complete code implementation based on the Python SDK.
> 3. Generate instructions for testing the server.

---

### 10. PDF Processing

**Invocation**: `@[pdf]` or `/pdf`

**Description**:
A comprehensive PDF processing toolkit supporting reading, generation, merging, splitting, and form filling.

**Core Capabilities**:
- **Content Extraction**: Extract text and tables (preserving layout).
- **File Operations**: Merge, split, and rotate pages.
- **PDF Generation**: Generate complex PDFs from code using ReportLab.
- **Image Conversion**: PDF to Image or Image to PDF.

**Use Case**:
> **User**: "Merge these three reports into one and add a watermark to every page."
>
> **Skill Response**:
> 1. Merge files using `pypdf`.
> 2. Create a watermark page and overlay it onto every page.
> 3. Output the final file.

---

### 11. PPTX (Presentations)

**Invocation**: `@[pptx]` or `/pptx`

**Description**:
Creates and edits PowerPoint presentations. Supports generation from outlines, template application, and underlying modifications.

**Core Capabilities**:
- **HTML to PPTX**: Convert HTML/CSS designs into native PPTX slides (supporting complex layouts).
- **Template Filling**: Replace text and images based on existing PPTX templates.
- **OOXML Editing**: Unpack PPTX to modify underlying XML (e.g., master slides, deep styles).

**Use Case**:
> **User**: "Generate a 10-slide presentation based on this Markdown outline."
>
> **Skill Response**:
> 1. Plan content and illustrations for each slide.
> 2. Render each slide's layout using `html2pptx` technology stack.
> 3. Generate the final .pptx file.

---

### 12. Skill Creator

**Invocation**: `@[skill-creator]` or `/skill-creator`

**Description**:
Guides users in creating high-quality Antigravity Skills.

**Core Capabilities**:
- **Structure Initialization**: Create standard `.agent/resources` and `.agent/workflows` structures.
- **Best Practices**: Provide Workflow writing guides and design patterns.

**Use Case**:
> **User**: "I want to create a Skill for automatically analyzing financial reports."
>
> **Skill Response**:
> Assist in creating the `financial-analyst` skill directory, planning the `analyze_report.py` script, and writing the workflow file.

---

### 13. Slack GIF Creator

**Invocation**: `@[slack-gif-creator]` or `/slack-gif-creator`

**Description**:
Creates animated GIFs optimized for Slack stickers.

**Core Capabilities**:
- **Parameter Optimization**: Control 128x128 size, frame rate, and color count to meet Slack limits.
- **Animation Tools**: Provide Python drawing tools (PIL) to create custom animations (shaking, rotating, explosion effects).

**Use Case**:
> **User**: "Make a 'Party Parrot' style nodding animation GIF."
>
> **Skill Response**:
> Draw frame-by-frame animation using Python and export as a GIF with Slack-optimized parameters.

---

### 14. Theme Factory

**Invocation**: `@[theme-factory]` or `/theme-factory`

**Description**:
Applies professional design themes to Artifacts (PPTs, docs, web pages).

**Core Capabilities**:
- **Theme Library**: Provides 10+ preset themes (e.g., "Deep Sea", "Sunset", "Minimalist").
- **Theme Generation**: Generate new color and font combinations based on descriptions.

**Use Case**:
> **User**: "Change this PPT to a 'Cyberpunk' style."
>
> **Skill Response**:
> Generate a theme configuration with neon colors and dark backgrounds, and apply it to the PPT generation process.

---

### 15. Web Artifacts Builder

**Invocation**: `@[web-artifacts-builder]` or `/web-artifacts-builder`

**Description**:
Builds complex, multi-file React web applications supporting Tailwind CSS and shadcn/ui.

**Core Capabilities**:
- **Project Scaffolding**: Initialize complete projects containing Vite, React, and Tailwind.
- **Component Library Integration**: Pre-install shadcn/ui components.
- **Single-file Bundling**: Bundle the entire app into a single HTML file for easy sharing and previewing.

**Use Case**:
> **User**: "Create an interactive report app with a dashboard and data visualization."
>
> **Skill Response**:
> 1. Initialize a React project.
> 2. Build the interface using shadcn/ui and integrate Recharts.
> 3. Bundle it as `dashboard.html` for delivery.

---

### 16. Webapp Testing

**Invocation**: `@[webapp-testing]` or `/webapp-testing`

**Description**:
Uses Playwright for automated testing and debugging of local web applications.

**Core Capabilities**:
- **Automated Testing**: Write Python scripts to simulate user actions (clicks, inputs).
- **State Verification**: Take screenshots, inspect DOM elements, and verify network requests.
- **Server Management**: Automatically start and manage local development servers.

**Use Case**:
> **User**: "Test my login page to confirm that incorrect passwords trigger an error."
>
> **Skill Response**:
> Write a Playwright script, start the local service, simulate a failed login, and take a screenshot to verify the error message.

---

### 17. XLSX (Excel Processing)

**Invocation**: `@[xlsx]` or `/xlsx`

**Description**:
Professional Excel processing supporting complex formulas, formatting preservation, and financial model construction.

**Core Capabilities**:
- **Data Analysis**: Clean and analyze data using Pandas.
- **Model Building**: Construct complex spreadsheets with formulas and formatting using openpyxl.
- **Formula Recalculation**: Ensure precise formula updates using the LibreOffice engine.
- **Financial Standards**: Follow investment banking formatting standards (blue text for inputs, black for formulas).

**Use Case**:
> **User**: "Help me build a DCF valuation model with 5-year projections and sensitivity analysis."
>
> **Skill Response**:
> 1. Build assumption and projection sheets.
> 2. Write Excel formulas to link cells (avoiding hard-coded numbers).
> 3. Apply standard financial model formatting and color coding.
> 4. Verify model results using recalculation scripts.

---

### 18. UI/UX Pro Max

**Invocation**: `@[ui-ux-pro-max]` or `/ui-ux-pro-max`

**Description**:
A powerful UI/UX design intelligence database and search engine covering 50+ design styles, 21+ color schemes, font pairings, and best practices across various tech stacks (React, Vue, Tailwind, etc.).

**Core Capabilities**:
- **Style Search**: Retrieve detailed characteristics and implementation parameters for specific styles (e.g., Glassmorphism, Brutalism).
- **Asset Recommendations**: Provide color, font, and chart suggestions for specific industries (e.g., Fintech, SaaS).
- **Tech Stack Guides**: Obtain implementation specifications for specific tech stacks (e.g., HTML-Tailwind, React).

**Use Case**:
> **User**: "I'm designing a clean, professional dashboard for a healthcare app."
>
> **Skill Response**:
> 1. Search "healthcare" for color (typically blue/cyan) and font recommendations.
> 2. Retrieve "clean professional" layout and style suggestions.
> 3. Provide specific Tailwind CSS implementation parameters (shadows, rounded corners).

---

### 19. Brainstorming

**Invocation**: `@[brainstorming]` or `/brainstorming`

**Description**:
A **mandatory** skill to use before any creative work (building components, adding features). Clarifies user intent, requirements, and design constraints through dialogue.

**Core Capabilities**:
- **Requirement Clarification**: Uncover implicit requirements through multiple-choice questions or targeted inquiries.
- **Solution Exploration**: Propose 2-3 different implementation paths before coding.
- **Guiding Principle**: Refuse blind coding - "Measure twice, cut once."

**Use Case**:
> **User**: "I want to add an AI feature to my Todo app."
>
> **Skill Response**:
> 1. Ask for specific scenarios (Auto-generating tasks? Smart sorting? Voice input?).
> 2. Propose three integration schemes: Local LLM, Cloud API, or Browser-side model.
> 3. Assist in defining the MVP scope.

---

### 20. Dispatching Parallel Agents

**Invocation**: `@[dispatching-parallel-agents]` or `/dispatching-parallel-agents`

**Description**:
Dispatches multiple agents to handle tasks in parallel when faced with 2 or more independent, stateless tasks.

**Use Case**:
> **User**: "Write Dockerfiles for the Python backend and React frontend of this project simultaneously; they don't depend on each other."
>
> **Skill Response**:
> 1. Start Agent A to analyze the backend `requirements.txt` and write a `Dockerfile`.
> 2. Start Agent B to analyze the frontend `package.json` and write a `Dockerfile`.
> 3. Aggregate outputs and report completion.

---

### 21. Executing Plans

**Invocation**: `@[executing-plans]` or `/executing-plans`

**Description**:
Used to execute pre-written Implementation Plans. Guides execution step-by-step with checkpoints at critical nodes.

**Use Case**:
> **User**: "Start executing the 'Database Layer Refactoring' plan we just created."
>
> **Skill Response**:
> 1. Read `implementation_plan.md`.
> 2. Prompt that `db.py` will be modified in Step 1.
> 3. Execute modification and run verification.
> 4. Ask if user wants to proceed to Step 2.

---

### 22. Finishing a Development Branch

**Invocation**: `@[finishing-a-development-branch]` or `/finishing-a-development-branch`

**Description**:
Guides branch cleanup after feature completion and testing. Offers merge strategies, PR description generation, and branch deletion suggestions.

**Use Case**:
> **User**: "Feature development is done, tests passed, ready to merge."
>
> **Skill Response**:
> 1. Check for uncommitted changes.
> 2. Recommend Squash Merge to keep the main branch clean.
> 3. Generate a PR description draft with key change points.
> 4. Suggest deleting local and remote `feature/login` branches.

---

### 23. Receiving Code Review

**Invocation**: `@[receiving-code-review]` or `/receiving-code-review`

**Description**:
Helps users process code review feedback. Instead of blind implementation, it evaluates feedback, flags unreasonable suggestions, or seeks clarification on vague points.

**Use Case**:
> **User**: "A colleague reviewed and said this function is too long and needs splitting, but splitting would break context. Help me handle this."
>
> **Skill Response**:
> 1. Analyze code and feedback.
> 2. Suggest response: Explain potential side effects of splitting and propose alternatives (e.g., detailed comments or folding regions).
> 3. Or: Acknowledge the feedback is reasonable and demonstrate how to safely extract a sub-function.

---

### 24. Requesting Code Review

**Invocation**: `@[requesting-code-review]` or `/requesting-code-review`

**Description**:
Performs self-review before code submission. Verifies requirements, tests, and documentation, generating high-quality PR descriptions.

**Use Case**:
> **User**: "About to submit code, help me with a final check."
>
> **Skill Response**:
> 1. Run linting and test suites.
> 2. Check if `README.md` is updated with new configuration items.
> 3. Generate a review request with a "Change Summary" and "Test Coverage".

---

### 25. Subagent Driven Development

**Invocation**: `@[subagent-driven-development]` or `/subagent-driven-development`

**Description**:
Splits complex plans into independent subtasks and uses Subagents (like Browser Subagent) for independent execution, keeping the main session context clean.

**Use Case**:
> **User**: "Per the plan, check the Ant Design website for the latest Table component API and update our component."
>
> **Skill Response**:
> 1. Launch Browser Subagent to find Table API on the official site.
> 2. Return API changes (e.g., changes in `columns` property) to the main Agent.
> 3. Main Agent modifies local code based on the data.

---

### 26. Systematic Debugging

**Invocation**: `@[systematic-debugging]` or `/systematic-debugging`

**Description**:
**Antigravity Core Debugging Methodology**. Guesses are strictly forbidden.
1. **Root Cause Analysis**: Identify the root cause first.
2. **Pattern Analysis**: Compare with similar working code.
3. **Hypothesis Verification**: Propose hypothesis -> Minimal testing -> Verify.
4. **Fix Implementation**: Only implement a fix after root cause is confirmed.

**Use Case**:
> **User**: "The production API occasionally reports 502 errors; not sure why."
>
> **Skill Response**:
> 1. **Refuse** attempts to restart or modify config blindly.
> 2. Guide user to collect logs (Phase 1: Evidence Collection).
> 3. Identify errors clustered in specific timeframes; hypothesize "Database Connection Pool Exhaustion" (Phase 3: Hypothesis).
> 4. Write a script to verify connection peaks, then adjust pool parameters (Phase 4: Fix).

---

### 27. Test Driven Development (TDD)

**Invocation**: `@[test-driven-development]` or `/test-driven-development`

**Description**:
**Antigravity Core Development Pattern**.
1. **Red**: Write a failing test (Reproduction script or Unit test).
2. **Green**: Write the minimum code to make the test pass.
3. **Refactor**: Optimize code structure.

**Use Case**:
> **User**: "Help me write a function to parse this special date format."
>
> **Skill Response**:
> 1. Create `test_date_parser.py` with passing and failing cases (Red).
> 2. Write simple regex parsing logic to ensure tests pass (Green).
> 3. Optimize regex performance and handle boundary cases (Refactor).

---

### 28. Using Git Worktrees

**Invocation**: `@[using-git-worktrees]` or `/using-git-worktrees`

**Description**:
Create isolated Git Worktrees for new features or bug fixes without disturbing the current workspace (Checkout).

**Use Case**:
> **User**: "I'm halfway through development, but there's an urgent bug on Prod. I don't want to stash my current changes."
>
> **Skill Response**:
> 1. Use `git worktree add ../hotfix-branch` to create a new directory.
> 2. Fix the bug and commit in the new directory.
> 3. Remove the Worktree and return to the original directory to continue development.

---

### 29. Using Superpowers

**Invocation**: `@[using-superpowers]` or `/using-superpowers`

**Description**:
A Meta-Skill. Helps users discover available Skills and how to use them correctly at the start of a session. Guides users to "Think about the Skill before acting."

**Use Case**:
> **User**: "I want to make a PPT; which tool is best?"
>
> **Skill Response**:
> Recommend `@[pptx]` for structure, `@[theme-factory]` for design themes, or `@[brand-guidelines]` if brand identity is needed.

---

### 30. Verification Before Completion

**Invocation**: `@[verification-before-completion]` or `/verification-before-completion`

**Description**:
The final line of defense before claiming "Task Complete." Enforces verification commands (Tests, Builds, Lint) and requires substantial evidence of success (Logs, Screenshots).

**Use Case**:
> **User**: "I think this bug is fixed."
>
> **Skill Response**:
> 1. Run the reproduction script to confirm "Success".
> 2. Run the full test suite to ensure no regressions.
> 3. Only reply "Task Complete" once green checkmarks are seen.

---

### 31. Writing Plans

**Invocation**: `@[writing-plans]` or `/writing-plans`

**Description**:
Write a detailed Implementation Plan before touching any code. Includes: Goal description, User Review Points, Detailed Change List, and Verification Plan.

**Use Case**:
> **User**: "We need to migrate the database from SQLite to MySQL."
>
> **Skill Response**:
> 1. Create `implementation_plan.md`.
> 2. Plan steps: Schema export, Data migration script, App config modification.
> 3. List specific files and verification methods (e.g., data consistency checks) for each step.
> 4. Wait for user confirmation before starting execution.

---

### 32. Writing Skills

**Invocation**: `@[writing-skills]` or `/writing-skills`

**Description**:
Assists in writing or modifying Skills. Provides best practices, templates, and testing methods for Antigravity Skills.

**Use Case**:
> **User**: "I want to write a new Skill for automatically optimizing SQL queries."
>
> **Skill Response**:
> 1. Plan Skill structure (Workflow + Python Script).
> 2. Write the `explain_analyzer.py` script.
> 3. Create `.agent/workflows/sql-optimizer.md` defining triggers and parameters.

---

### 33. Planning with Files

**Invocation**: `@[planning-with-files]` or `/planning-with-files`

**Description**:
Implements a Manus-like task planning mode using `task_plan.md`, `findings.md`, and `progress.md` as persistent "disk memory" to bypass Context Window limits.

**Core Capabilities**:
- **Persistent Memory**: Write key decisions, findings, and progress to files rather than leaving them in dialogue history.
- **Task Phasing**: Enforce breaking complex tasks into Phases and marking them as complete.
- **Error Learning**: Record encountered errors and tried solutions in the plan file to avoid repeating mistakes.

**Use Case**:
> **User**: "I want to research migrating our Django project to FastAPI; this involves many file changes and investigation."
>
> **Skill Response**:
> 1. Initialize `task_plan.md` (defining investigation, prototype, migration, testing phases).
> 2. Initialize `findings.md` (to record API differences between Django and FastAPI).
> 3. Initialize `progress.md` (to record operation logs).

---

### 34. BDI Mental States

**Invocation**: `@[bdi-mental-states]` or `/bdi-mental-states`

**Description**:
Simulates the Belief-Desire-Intention (BDI) model. Enables agents to perform reasoning and decision-making more like humans, rather than simple request-response.

**Core Capabilities**:
- **Belief Modeling**: Transform information into structured beliefs (RDF/Knowledge Graphs).
- **Intention Generation**: Generate specific action intentions based on desires and beliefs.
- **Dynamic Tuning**: Real-time updates of mental states based on new information.

**Use Case**:
> **User**: "Simulate the mental activity of a rational buyer considering an EV."
>
> **Skill Response**:
> 1. Establish initial beliefs ("Rising fuel prices", "Environmental impact is important").
> 2. Generate desires ("Reduce travel costs", "Minimize carbon footprint").
> 3. Form intentions ("Research Model 3 and BYD Han").

---

### 35. Memory Systems

**Invocation**: `@[memory-systems]` or `/memory-systems`

**Description**:
Builds a persistent long-term memory system for Agents, surpassing context limits for cross-session information storage and retrieval.

**Core Capabilities**:
- **Knowledge Graphs**: Build graph memory of entity relationships.
- **Entity Tracking**: Continuously track key entities (e.g., user preferences, project status).
- **Cross-session Persistence**: Save key info into databases or file systems.

**Use Case**:
> **User**: "Remember my previous project preferences?"
>
> **Skill Response**:
> Retrieve from memory (e.g., "Prefers React", "Dislikes Tailwind") and apply to current task.

---

### 36. Filesystem Context

**Invocation**: `@[filesystem-context]` or `/filesystem-context`

**Description**:
Leverages the filesystem as extended context storage. Suitable for processing massive info constrained by Token windows.

**Core Capabilities**:
- **Context Offloading**: Automatically write less-frequent info to files.
- **Dynamic Loading**: Retrieve and load into the window on demand.
- **Scratchpad Management**: Maintain the Agent's "Draft Paper" and "Notebook."

**Use Case**:
> **User**: "We need to analyze these 50 documents, but they're too long to fit."
>
> **Skill Response**:
> Suggest a filesystem summary strategy: generate summaries into the `summaries/` directory, reading details only when necessary.

---

### 37. Context Fundamentals

**Invocation**: `@[context-fundamentals]` or `/context-fundamentals`

**Description**:
A foundational tool for understanding LLM context mechanisms. Helps users understand "Why the model forgot" or "Why it's not following instructions."

**Core Capabilities**:
- **Window Analysis**: Explain current context window utilization.
- **Attention Mechanisms**: Visualize or explain possible attention distributions.
- **Prompt Debugging**: Diagnose if Prompt structure causes attention drift.

**Use Case**:
> **User**: "The model ignores instructions in the middle of my Prompt."
>
> **Skill Response**:
> 1. Analyze Primacy/Recency Effects.
> 2. Suggest moving critical instructions to the end (Recency).
> 3. Use XML tags to reinforce instruction boundaries.

---

### 38. Context Optimization

**Invocation**: `@[context-optimization]` or `/context-optimization`

**Description**:
Focuses on reducing Token consumption and improving processing efficiency.

**Core Capabilities**:
- **KV-Cache Optimization**: Design cache-friendly Prompt structures.
- **Partitioning Strategy**: Split long tasks into multiple independent small context tasks.
- **Budget Management**: Set Token budgets and cleanup strategies for long dialogues.

**Use Case**:
> **User**: "This dialogue is too long; API costs are high and it's getting slow."
>
> **Skill Response**:
> 1. Detect duplicate System Prompts; suggest Context Caching (if supported).
> 2. Identify and remove redundant data blocks (e.g., old code files).
> 3. Enable a rolling window strategy, keeping only recent N turns.

---

### 39. Context Compression

**Invocation**: `@[context-compression]` or `/context-compression`

**Description**:
Compression techniques for ultra-long context, significantly reducing Tokens while retaining key info.

**Core Capabilities**:
- **Summary Generation**: Recursively summarize long text.
- **Information Extraction**: Extract key KV pairs from unstructured text.
- **Semantic Compression**: Rewrite verbose content with more compact expressions.

**Use Case**:
> **User**: "Summarize this 100,000-word paper, keeping only core arguments and data as background."
>
> **Skill Response**:
> 1. Perform `compress` operation using recursive summarization.
> 2. Replace original text with structured high-density summary (90% Token reduction).
> 3. Ensure subsequent Q&A remains grounded in these core facts.

---

### 40. Context Degradation

**Invocation**: `@[context-degradation]` or `/context-degradation`

**Description**:
Specially handles "Lost-in-the-Middle" issues in long contexts.

**Core Capabilities**:
- **Degradation Diagnosis**: Detect if the model is hallucinating or ignoring instructions.
- **Critical Info Reset**: Periodically restate critical instructions (System Prompt reinforcement).
- **Context Refresh**: Guide users to open a new session to restore intelligence.

**Use Case**:
> **User**: "The Agent has become 'dumb'; it forgot the variable names I defined at the start."
>
> **Skill Response**:
> 1. Diagnose that context has reached 180k with uneven attention distribution.
> 2. Suggest "Context Refresh": Summarize current progress and generate a new System Prompt.
> 3. Guide user to start a new session with this Snapshot to restore reasoning.

---

### 41. Multi-Agent Patterns

**Invocation**: `@[multi-agent-patterns]` or `/multi-agent-patterns`

**Description**:
Designs and implements advanced Multi-Agent collaboration systems.

**Core Capabilities**:
- **Supervisor Pattern**: One master Agent coordinating multiple subordinate Agents.
- **Swarm Pattern**: Multiple peer Agents self-organizing for collaboration.
- **Handoffs**: Define context and task handoff protocols between Agents.

**Use Case**:
> **User**: "Design an Agent system for a software development team."
>
> **Skill Response**:
> Design a workflow with PM, Dev, and QA roles, defining task distribution (PM) and verification (QA).

---

### 42. Hosted Agents

**Invocation**: `@[hosted-agents]` or `/hosted-agents`

**Description**:
Builds Agents that can run long-term in the background or on a server, detached from the current dialogue box.

**Core Capabilities**:
- **Sandbox Environments**: Deploy Agents in Modal or Docker.
- **Continuous Running**: Implement Agents for loop execution or scheduled tasks.
- **API Encapsulation**: Wrap Agent capabilities as HTTP APIs.

**Use Case**:
> **User**: "I need a bot to monitor GitHub Issues and reply automatically, running 24/7."
>
> **Skill Response**:
> 1. Write Agent logic (Listen to webhooks -> Analyze issue -> Comment).
> 2. Package it using Modal or Docker.
> 3. Deploy to a cloud server as an independent Service.

---

### 43. Tool Design

**Invocation**: `@[tool-design]` or `/tool-design`

**Description**:
Expert guide for designing high-quality Agent tools (Function Calling).

**Core Capabilities**:
- **Interface Definition**: Write clear, unambiguous JSON Schemas.
- **Fault-tolerant Design**: Design robust error handling and feedback mechanisms.
- **Granularity Control**: Balance a tool's atomicity and ease of use.

**Use Case**:
> **User**: "I want to add a database query tool for the Agent; what's the best design?"
>
> **Skill Response**:
> 1. Warning: Do not provide direct `execute_sql` permissions (dangerous and hallucination-prone).
> 2. Suggest: Design semantic tools like `get_user_by_email(email)` or `search_orders(query)`.
> 3. Provide JSON Schema definitions and Pydantic models.

---

### 44. Project Development

**Invocation**: `@[project-development]` or `/project-development`

**Description**:
End-to-end guide for developing LLM-native applications.

**Core Capabilities**:
- **Task Fit**: Evaluate if a task is suitable for LLM + Agent solutions.
- **Tech Selection**: Choose models (Claude vs. GPT vs. Local), databases, and frameworks.
- **Cost Estimation**: Estimate Token consumption and latency.

**Use Case**:
> **User**: "I want to use an LLM for a legal contract review system. Where do I start?"
>
> **Skill Response**:
> 1. Step 1: Task-Fit evaluation (confirming legal clause review is within model capacity).
> 2. Step 2: Architecture design (RAG for statutes + GPT-4 for logic review).
> 3. Step 3: PoC prototype verification plan.

---

### 45. Evaluation (Basic)

**Invocation**: `@[evaluation]` or `/evaluation`

**Description**:
Establishes a foundational evaluation system for Agent systems.

**Core Capabilities**:
- **Test Set Construction**: Generate Golden Datasets.
- **Metric Definition**: Define Accuracy, Recall, Hallucination rates, etc.
- **Automated Execution**: Batch-run test cases.

**Use Case**:
> **User**: "How do I know if my Prompt change made the Agent better or worse?"
>
> **Skill Response**:
> 1. Create a CSV dataset with 50 typical user questions and standard answers.
> 2. Define metrics (Accuracy, JSON format correctness).
> 3. Run the `evaluation` script to compare score changes (+5% or -10%).

---

### 46. Advanced Evaluation

**Invocation**: `@[advanced-evaluation]` or `/advanced-evaluation`

**Description**:
Implements deeper, model-based evaluation methods.

**Core Capabilities**:
- **LLM-as-a-Judge**: Use powerful models (e.g., Claude 3.5 Sonnet) to evaluate weaker model outputs.
- **Pairwise Comparison**: Simulate human preference testing (Elo rating).
- **Bias Analysis**: Detect potential biases in model outputs.

**Use Case**:
> **User**: "I need to evaluate if generated marketing copy is creative; that's hard to judge with code."
>
> **Skill Response**:
> 1. Set up an LLM-as-a-Judge pipeline with Claude 3.5 Sonnet as the judge.
> 2. Provide evaluation dimensions (Creativity, Logic, Fluency) and scoring rubrics (1-5 points).
> 3. Have the judge score and comment on the smaller model's output.
