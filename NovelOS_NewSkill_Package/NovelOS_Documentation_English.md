# NovelOS Complete Documentation (English Version)

> Version: v1.0.0　｜　Last Updated: 2026-05-12

---

## Table of Contents

1. [What is NovelOS?](#1-what-is-novelos)
2. [Core Features Overview](#2-core-features-overview)
3. [System Architecture & File Structure](#3-system-architecture--file-structure)
4. [AI Agent Roles (SOP)](#4-ai-agent-roles-sop)
5. [Development Workflow (Phase 0 – Phase 7)](#5-development-workflow-phase-0--phase-7)
6. [All Templates Explained](#6-all-templates-explained)
7. [Project Rules & Prohibitions](#7-project-rules--prohibitions)
8. [Version Control Guidelines](#8-version-control-guidelines)
9. [Quick Start Guide](#9-quick-start-guide)
10. [FAQ](#10-faq)

---

## 1. What is NovelOS?

**NovelOS** is an AI-powered operating system designed specifically for **long-form novel and IP development**.

Its goal is not simply to "generate stories." Instead, it functions like a complete operating system that **manages the entire development lifecycle of a novel universe** — from market research and worldbuilding to character design, foreshadowing layout, chapter writing, quality assurance, and version publishing.

### Why Do You Need NovelOS?

Long-form novel development faces several common pitfalls. NovelOS addresses each one:

| Problem | NovelOS Solution |
|---------|-----------------|
| Worldbuilding inconsistencies (lore-eating) | Lore Database + Version Control |
| Character OOC (Out of Character) | Character Cards + QA Review |
| Unchecked power scaling | Power Scale Manager + No-Free-Upgrade Rule |
| Forgotten or unresolved foreshadowing | Foreshadow Manager Tracking |
| Multi-AI collaboration chaos | Clear AI Agent SOP Division |
| Blind development without market research | Research Phase before any creation |

### Core Design Philosophy

- **Research before creating**: Market research is mandatory before any creative work begins.
- **Layered memory management**: Four memory layers ensure no setting is lost.
- **Strict workflow control**: 7 sequential Phases — no skipping allowed.
- **Clear AI division of labor**: ChatGPT / Gemini / Claude Code / Codex each have defined roles.
- **Enforced version control**: Every modification must leave a traceable record.

---

## 2. Core Features Overview

### 2.1 Market Research System (Research Phase)
- Analyze current popular genres and reader preferences
- Competitive analysis to identify market gaps
- Mythology, history, and science reference material collection
- Viral element and emotional rhythm analysis
- Feasibility assessment report generation

### 2.2 Four-Layer Memory Management System

| Layer | Content | Description |
|-------|---------|-------------|
| Layer 1 | Core Immutable Settings | World rules, main story endings, ability logic foundations |
| Layer 2 | Long-term Character Memory | Personality, relationships, beliefs, weaknesses, destiny |
| Layer 3 | Mid-term Plot Memory | Current arc, subplots, foreshadowing, regional powers |
| Layer 4 | Short-term Chapter Memory | Events, emotions, and battle states from the last 3–5 chapters |

### 2.3 Lore Database (Worldbuilding)
- Background settings, races, and factions
- Geographic and map descriptions
- Historical events and legends
- Technology / Magic / Ability system rules

### 2.4 Character Database
- Standardized character card format
- Personality, desires, fears, and growth arcs
- Ability system with restrictions recorded
- Character relationship network management

### 2.5 Foreshadowing Manager
- Individual tracking file per foreshadow element
- Records first appearance chapter and expected resolution chapter
- Status labels: Unresolved / Partially Resolved / Resolved

### 2.6 Power Scale Manager
- Power level records for each character or faction
- Mandatory registration of ability limits and costs
- Rule mechanism to prevent cost-free power-ups

### 2.7 Emotional Curve Planning
- Chapter-level emotional arc design
- Setting emotional goals for: opening, middle, climax, and ending
- Pacing guidance for writing density adjustments

### 2.8 Timeline Manager
- Sequential logging of major story events
- Prevention of timeline errors and logical contradictions
- Cause-and-effect chain tracking

### 2.9 Version Control & Work Logs
- CHANGELOG.md: Version history records
- WORKLOG.md: Detailed log of every modification
- Semantic Versioning (SemVer) management

### 2.10 QA Quality Assurance Pipeline
- Setting conflict checks
- Character OOC detection
- Timeline contradiction detection
- Power balance auditing

---

## 3. System Architecture & File Structure

### 3.1 Complete Folder Structure

```
NovelOS_Project/
├── Research/                    # Market and genre research (Phase 0)
│   ├── market_trends.md         # Market trend analysis
│   ├── audience_analysis.md     # Audience analysis
│   ├── myth_science_notes.md    # Mythology, history, and science references
│   └── summary.md               # Integrated research summary
│
├── PROJECT_RULES.md             # Core project rules and prohibitions
├── WORKLOG.md                   # Work log (all modification records)
├── CHANGELOG.md                 # Version records
│
├── 00_Project_Rules/            # Extended rules documents
├── 01_Requirements/             # Development requirements and genre descriptions
├── 02_Lore/                     # Lore (worldbuilding) database
│   ├── world_history.md
│   ├── magic_system.md
│   ├── religions.md
│   └── ...
├── 03_Characters/               # Character database
│   ├── [CharacterName].md
│   └── ...
├── 04_Timeline/                 # Timeline files
├── 05_Foreshadow/               # Foreshadowing management
├── 06_PowerScale/               # Power scale control
├── 07_EmotionalCurve/           # Emotional curve planning
├── 08_Chapters/                 # Chapter drafts and final versions
├── 09_QA/                       # QA reports and revision suggestions
├── 10_Worklog/                  # Archived work logs
└── 11_Versions/                 # Historical versions and backups
```

### 3.2 Critical Rules

- `Research/` data **must never be copied directly** into `02_Lore/` or `03_Characters/`
- All setting changes **must be reflected** in WORKLOG.md
- Major changes **must update** CHANGELOG.md and increment the version number

---

## 4. AI Agent Roles (SOP)

NovelOS uses a multi-AI division of labor. Each AI is responsible for distinct phases and functions. Overlap or task substitution is prohibited.

### 4.1 Gemini — Research AI (Phase 0)

**Responsible Phase**: Phase 0 (Market Research)

**Responsibilities**:
1. Survey market trends, analyze popular genres and reader preferences
2. Competitive analysis to identify market gaps and opportunities
3. Collect mythology, history, and science reference materials
4. Analyze viral plot elements and emotional rhythms
5. Produce research reports and store them in the `Research/` directory

**Important Notes**:
- Research results are **for decision-making reference only**; they must not be used directly as story settings
- After completing research, wait for human decision-making before proceeding

---

### 4.2 ChatGPT — PM / Core (Phases 1, 2, 3, 4, 7)

**Responsible Phases**: Phase 1, 2, 3, 4, 7 (Project Management, Worldbuilding, Characters, Planning, Publishing)

**Responsibilities**:
1. Project initialization: build complete folder structure and rules documents
2. Build the lore: create Lore data based on research results and requirements
3. Build characters: create character cards based on requirements and lore
4. Long-form planning: design plot structure, chapter pacing, and foreshadowing plans
5. Maintain the four-layer memory system
6. Final integration and publishing preparation

**Important Notes**:
- ChatGPT **does not write actual chapters**
- All outputs must be recorded in corresponding files following version control standards

---

### 4.3 Claude Code — Main Developer (Phase 5)

**Responsible Phase**: Phase 5 (Chapter Development)

**Responsibilities**:
1. Write novel chapters according to the long-form plan
2. Update `02_Lore/` and `03_Characters/` when settings change during writing
3. Edit chapters as needed, maintaining consistent style and pacing
4. Record all changes in `WORKLOG.md`

**Important Notes**:
- Claude Code **cannot independently add or modify worldbuilding rules**
- If rules are insufficient, notify ChatGPT for additions — **do not speculate or fill in gaps autonomously**

---

### 4.4 Gemini — QA AI (Phase 6)

**Responsible Phase**: Phase 6 (Quality Assurance)

**Responsibilities**:
1. Setting conflict checks: review worldbuilding contradictions, setting conflicts, missed foreshadowing
2. Character OOC review: ensure character behavior aligns with established personalities
3. Timeline verification: confirm logical event order with no temporal inconsistencies
4. Power balance auditing: check for overly rapid power growth or cost-free upgrades
5. Record QA reports and revision suggestions in `09_QA/`

**Important Notes**:
- QA phase is **review and suggestion only — no direct content modification**
- Identified issues must be reported to ChatGPT or Claude Code for resolution

---

### 4.5 Codex — Engineering AI (On-demand across all phases)

**Responsible Phase**: All phases, as needed

**Responsibilities**:
1. Develop checking tools and template generation scripts
2. Automated file structure validation
3. Verify chapter document formatting and Markdown structure

**Important Notes**:
- Codex **does not participate in content generation**
- Output focuses on technical checks and automation tooling

---

## 5. Development Workflow (Phase 0 – Phase 7)

```
Phase 0 → Phase 1 → Phase 2 → Phase 3 → Phase 4 → Phase 5 → Phase 6 → Phase 7
Research   Init    Lore      Characters  Planning   Writing    QA      Publishing
(Gemini) (ChatGPT)(ChatGPT) (ChatGPT) (ChatGPT)  (Claude)  (Gemini) (ChatGPT)
```

### Phase 0: Research Phase

**Purpose**: Analyze market trends and genre feasibility before committing to development.

**Executor**: Gemini (Research AI)

**Main Tasks**:
- Analyze current popular genres and reader preferences
- Research competitor works for strengths, weaknesses, and market gaps
- Collect mythology, history, and science reference materials
- Analyze viral plot elements and emotional rhythms

**Deliverables**:
- `Research/market_trends.md`
- `Research/audience_analysis.md`
- `Research/myth_science_notes.md`
- `Research/summary.md` (integrated report)

**Completion Criteria**:
- Research reports completed
- Creator confirms genre feasibility
- Human decision to "proceed to formal development"

---

### Phase 1: NovelOS Initialization

**Purpose**: Build the project's foundational structure for all subsequent development.

**Executor**: ChatGPT (PM)

**Main Tasks**:
- Create complete folder structure
- Generate `PROJECT_RULES.md`, `WORKLOG.md`, `CHANGELOG.md`
- Initialize Lore Database and Character Database
- Define prohibitions and version control standards

---

### Phase 2: Lore Building (Worldbuilding)

**Purpose**: Establish a complete and internally consistent worldbuilding foundation.

**Executor**: ChatGPT

**Main Tasks**:
- Write background overview, races, and factions
- Build geographic descriptions
- Document historical events and legends
- Define technology/magic ability rules, limitations, and costs

**Storage Location**: `02_Lore/`

---

### Phase 3: Character Building

**Purpose**: Create complete character cards for every major character.

**Executor**: ChatGPT

**Main Tasks**:
- Fill in personality, core desires, fears, and weaknesses
- Design ability systems and growth arcs
- Build character relationship networks
- Document character secrets and foreshadowing links

**Storage Location**: `03_Characters/[CharacterName].md`

---

### Phase 4: Long-form Planning

**Purpose**: Plan plot pacing, major events, foreshadowing layout, and resolution schedule.

**Executor**: ChatGPT

**Main Tasks**:
- Build the timeline (`04_Timeline/`)
- Design the foreshadowing list (`05_Foreshadow/`)
- Plan power growth paths (`06_PowerScale/`)
- Design emotional curves for each arc (`07_EmotionalCurve/`)

---

### Phase 5: Chapter Development

**Purpose**: Write the actual novel chapters based on the long-form plan.

**Executor**: Claude Code (Main Developer)

**Main Tasks**:
- Write chapter drafts
- Maintain consistency with lore and character settings
- Update `WORKLOG.md` after every modification
- Update `CHANGELOG.md` for major changes

**Storage Location**: `08_Chapters/`

---

### Phase 6: QA Quality Assurance

**Purpose**: Ensure chapter quality, preventing setting conflicts and narrative collapse.

**Executor**: Gemini (QA AI)

**Main Tasks**:
- Check for setting conflicts and worldbuilding contradictions
- Audit character behavior for OOC
- Verify timeline logic
- Audit power balance
- Output revision suggestion reports

**Storage Location**: `09_QA/`

---

### Phase 7: Version Sync & Publishing Preparation

**Purpose**: Integrate all revisions, update version records, and prepare for publishing.

**Executor**: ChatGPT

**Main Tasks**:
- Integrate outputs from Claude Code and Gemini QA
- Update version number and version records
- Perform translation tasks
- Prepare publishing format

---

## 6. All Templates Explained

### 6.1 Character Card (CHARACTER_TEMPLATE.md)

**Storage Path**: `03_Characters/[CharacterName].md`

**Field Reference**:

| Field | Description |
|-------|-------------|
| Role / Character Type | Protagonist, supporting character, antagonist, NPC, etc. |
| Initial Personality | Key personality traits (introverted, confident, cunning, brave, etc.) |
| Core Desire | What the character most wants to achieve or obtain |
| Fears & Weaknesses | Inner weaknesses and things the character is afraid of |
| Abilities & Skills | Special powers or skills — **must state limitations and costs** |
| Growth Arc / Evolution Path | Initial → Mid-story → Final form |
| Relationship Network | Relationships with other key characters (rival, ally, master-student, etc.) |
| Secrets & Foreshadowing | Hidden secrets — must have corresponding Foreshadow Manager entries |
| Current Status | Character's state, emotions, and location at the current chapter |
| Inviolable Rules | Core character prohibitions that cannot be changed arbitrarily |

**Important Reminders**:
- Character cards should be created **before the character's first appearance**
- Any updates must be recorded in `WORKLOG.md`

---

### 6.2 Lore Data (LORE_TEMPLATE.md)

**Storage Path**: `02_Lore/[category].md`

**Field Reference**:

| Field | Description |
|-------|-------------|
| Background Overview | The world's overall setting and era |
| Races & Factions | Major races, groups, nations, or organizations |
| Geography & Maps | Important regions, towns, or star systems |
| Historical Events & Legends | Major historical events shaping the current situation |
| Religion & Mythology | Religious systems, beliefs, and mythology |
| Technology / Magic Rules | **Power source, mechanics, limitations, and costs** (required) |
| Evolution & Class System | Character or race evolution tiers and social hierarchy |
| Key Items & Resources | Artifacts, critical resources, or ruins |
| Endgame Foreshadowing | Foreshadowing connected to the main story's conclusion |

**Important Reminders**:
- All lore settings must be reviewed and approved by ChatGPT (PM) before being added
- Any modifications must increment the version number

---

### 6.3 Timeline Management (TIMELINE_TEMPLATE.md)

**Storage Path**: `04_Timeline/[arc or event name].md`

**Field Reference**:

| Field | Description |
|-------|-------------|
| Chapter of Occurrence | The chapter position in the novel |
| Time of Occurrence | Specific date, year, or in-world calendar notation |
| Location | Geographic location or region |
| Characters Involved | List of all major characters present |
| Event Description | Overview of how the event unfolds |
| Immediate Consequences | Direct results of the event |
| Long-term Effects | Lasting impact on the story |
| Potential Conflicts | Possible contradictions with other events (flagged for QA) |

**Important Reminders**:
- Time spans for character travel, recovery, or information transmission must be **logically calculated**
- Complex events can be broken into sub-events that link back to the main event

---

### 6.4 Foreshadowing Management (FORESHADOW_TEMPLATE.md)

**Storage Path**: `05_Foreshadow/[foreshadow name].md`

**Field Reference**:

| Field | Description |
|-------|-------------|
| Foreshadow Type | Main plot / Lore / Character / Emotional / Conspiracy / Endgame |
| First Appearance Chapter | Where the foreshadow is first introduced |
| Characters Involved | List of related characters |
| Content Description | What the foreshadow hints at and how it is planted |
| Expected Resolution Chapter | Projected chapter for reveal (can be updated — must be logged) |
| Current Status | **Unresolved / Partially Resolved / Resolved** |
| Resolution Method | How the foreshadow will be resolved in the story |
| Notes | Connections to other foreshadowing elements |

**Important Reminders**:
- All foreshadowing **must be resolved at an appropriate chapter**
- If the expected resolution chapter changes, update this file and log the change

---

### 6.5 Power Scale Management (POWER_SCALE_TEMPLATE.md)

**Storage Path**: `06_PowerScale/[character or faction name].md`

**Field Reference**:

| Field | Description |
|-------|-------------|
| Current Power Level | Current stage power level (numeric or tier system) |
| Ability Description | Ability characteristics, advantages, and usage |
| Limitations & Costs | **Energy consumption, backlash damage, cooldowns, etc.** (required) |
| Weaknesses | Ways the character can be countered or natural vulnerabilities |
| Defeatable Opponents | Opponents the character can currently overcome |
| Undefeatable Opponents | Opponents the character currently cannot defeat |
| Next Stage Growth Conditions | Requirements for leveling up or evolving |
| Is Growth Too Fast? | Self-audit: is the growth rate reasonable? |

**Important Reminders**:
- Power updates must be **synchronized** with character cards and chapter descriptions
- If QA identifies power imbalance, the relevant chapters must be **rolled back or revised**

---

### 6.6 Emotional Curve (EMOTIONAL_CURVE_TEMPLATE.md)

**Storage Path**: `07_EmotionalCurve/[arc name].md`

**Field Reference**:

| Field | Description |
|-------|-------------|
| Opening | Emotional state at the chapter's start — grabs attention or sets up suspense |
| Middle | Builds pressure or conflict, accumulating tension |
| Climax | Emotional peak — the story's turning point |
| Ending | Resolution or cliffhanger to guide the reader into the next chapter |
| Emotional Target | Choose from: Oppression, Tension, Satisfaction, Despair, Hope, Sadness, Achievement, Reversal, Lingering Resonance |
| Pacing Notes | Guidance on adjusting prose density, dialogue ratio, and battle description |

**Important Reminders**:
- Emotional curves must remain **consistent** with lore, character growth, and power settings
- Do not create emotional peaks by **breaking logical consistency**

---

### 6.7 Research Report (RESEARCH_TEMPLATE.md)

**Storage Path**: `Research/[report name].md`

**Structure**:

**Section 1: Market Trend Analysis**
- Popular genre list with element breakdowns
- Audience preference analysis (with supporting data or case studies)
- Competitive overview (3–5 works: strengths, weaknesses, market gaps)

**Section 2: Mythology / History / Science References**
- Relevant myths and legends with symbolic significance
- Historical events and figures useful for worldbuilding
- Scientific principles for any technology-based world elements

**Section 3: Viral Elements & Emotional Rhythm**
- Plot elements and settings readers particularly enjoy
- Emotional curve analysis of successful works

**Section 4: Conclusions & Recommendations**
- Genre feasibility assessment
- Development direction recommendations (elements to strengthen & pitfalls to avoid)

**Important Reminders**:
- Research results are **for decision-making reference only** — do not write them directly into lore
- After completion, generate `summary.md` as an integrated decision-making document

---

### 6.8 Work Log (WORKLOG_TEMPLATE.md)

**Storage Path**: `WORKLOG.md` (root directory)

**Format**:

```markdown
## [YYYY-MM-DD] Work Item Title (e.g., Update character settings, Fix worldbuilding gap)

- **Responsible Party / AI**: ChatGPT / Claude / Gemini / Codex / Human
- **Version Number**: vX.Y.Z
- **Changes Made**:
  - Brief description of the modification or addition
  - Specific file paths involved
- **Scope of Impact**:
  - Which chapters or settings this change may affect
- **To-Do Items**:
  - Follow-up tasks or items requiring collaboration from other AIs
- **Risks / Notes**:
  - Potential risks from this change, flagged for QA attention
```

**Important Reminders**:
- Always **append** new entries to the end of `WORKLOG.md` — never overwrite previous records
- Major changes must also update `CHANGELOG.md`

---

### 6.9 Version Records (CHANGELOG_TEMPLATE.md)

**Storage Path**: `CHANGELOG.md` (root directory)

**Format**:

```markdown
## vX.Y.Z - YYYY-MM-DD

### Added
- [Added] Description of new features, templates, or settings

### Fixed
- [Fixed] Description of issues resolved and their impact

### Changed
- [Changed] Description of modifications or removals

### Notice
- [Notice] Breaking change warnings that require team-wide sync
```

**Version Number Rules (SemVer)**:
- `vX.0.0` — Major version: large-scale lore restructuring or core rule changes
- `v0.Y.0` — Minor version: new characters, new chapters, new setting modules
- `v0.0.Z` — Patch version: small fixes, typo corrections, format adjustments

---

## 7. Project Rules & Prohibitions

### 7.1 General Principles

1. **Data separation**: Research data goes in `Research/`; official settings go in `02_Lore/` etc. — **never mix them**.
2. **Workflow order**: Research Phase must be complete and genre confirmed before formal development begins. **No skipping steps**.
3. **Version control**: Every major change updates `CHANGELOG.md` and is logged in `WORKLOG.md`.
4. **Work log**: All AIs must **immediately** update `WORKLOG.md` when modifying data. Unlogged changes are considered invalid.

### 7.2 Seven Absolute Prohibitions

| Prohibited Action | Explanation |
|-------------------|-------------|
| No self-filling of unconfirmed settings | Unreviewed settings cannot be added; must go through ChatGPT for confirmation |
| No worldbuilding inconsistencies (lore-eating) | Must not contradict established world rules or prior narrative content |
| No character OOC | Character speech and actions must conform to established personality and growth arc |
| No cost-free power upgrades | Ability growth must have corresponding costs or limitations |
| No unresolved foreshadowing | All foreshadowing must be resolved at an appropriate chapter and logged |
| No missing version records | Major setting changes without a CHANGELOG update are considered invalid |
| No development without completed research | Lore or chapter development cannot begin before Research Phase is complete |

### 7.3 Recommended Best Practices

- **Clear communication**: Use clear documentation and labels when suggesting changes
- **Regular QA**: Run Gemini QA checks after completing each significant milestone
- **Reuse templates**: Always use template files to maintain consistent format
- **Protect core settings**: Only ChatGPT may modify core immutable settings; other AIs must submit a request first

---

## 8. Version Control Guidelines

NovelOS uses **Semantic Versioning (SemVer)**:

```
v[MAJOR].[MINOR].[PATCH]
```

### When to Increment Each Version Segment

| Version Type | When to Increment |
|-------------|-------------------|
| Major (X) | Large-scale lore restructuring, core rule changes, major character setting overhaul |
| Minor (Y) | New character added, new chapter completed, new setting module introduced |
| Patch (Z) | Small fixes, typo corrections, format adjustments |

### Version Update Workflow

1. Identify the nature of the change (Major / Minor / Patch)
2. Update `CHANGELOG.md` (insert new version record at the top)
3. Update `WORKLOG.md` (record version number and change details)
4. Archive to `11_Versions/` as a backup

---

## 9. Quick Start Guide

### Step 1: Create the Project Directory

```
mkdir NovelOS_Project
cd NovelOS_Project
```

Copy all template files from this package into the corresponding directories.

### Step 2: Execute the Research Phase

Input the following prompt in Gemini:
> "Please follow the RESEARCH_TEMPLATE.md to begin market research. Analyze market trends, competitor works, audience preferences, and viral elements for [your genre direction]. Store results in the Research/ directory."

### Step 3: Confirm Genre Feasibility

Read `Research/summary.md` and decide whether to proceed to formal development.

### Step 4: Initialize the Project (Phase 1)

Input the following prompt in ChatGPT:
> "Please use SYSTEM_PROMPT.txt to activate NovelOS. Based on the Research results, initialize the project, build the complete file structure, and generate PROJECT_RULES.md."

### Step 5: Progress Through Each Phase Sequentially

Follow the order Phase 2 → 3 → 4 → 5 → 6 → 7, executing corresponding tasks with the appropriate AI at each stage.

### Step 6: Update the Work Log After Every Modification

No matter how small the change, immediately append a new entry to `WORKLOG.md`.

---

## 10. FAQ

**Q: Can I skip the Research Phase and start creating immediately?**
A: No. PROJECT_RULES.md explicitly prohibits development without completed research. The Research Phase ensures the genre has market potential, preventing wasted effort on an unviable project.

**Q: What if the creator decides not to proceed after the research is done?**
A: The research results are saved in the `Research/` directory. If the project is restarted in the future, the prior research can be referenced directly without repeating the process.

**Q: What if Claude Code discovers a worldbuilding gap during writing? Can it fill it in?**
A: No. Claude Code must notify ChatGPT (PM) to supplement the settings. Claude Code cannot speculate or autonomously fill in unconfirmed worldbuilding rules.

**Q: After QA identifies a problem, who fixes the chapters?**
A: Gemini (QA AI) only produces reports and suggestions. Claude Code handles chapter revisions; major setting changes require ChatGPT confirmation.

**Q: Can foreshadowing ever go unresolved?**
A: No. PROJECT_RULES.md prohibits unresolved foreshadowing. All foreshadowing must be resolved at an appropriate chapter. If a foreshadowing element is confirmed to be dropped, mark it in the Foreshadow file and record the reason.

**Q: How do I decide which version segment to increment?**
A: Follow SemVer conventions: small fixes → Patch (Z), new features or chapters → Minor (Y), major architecture changes → Major (X).

**Q: Can multiple AIs work on the same phase simultaneously?**
A: In general, no — the phases are sequential. However, Codex (Engineering AI) can be invoked at any time across all phases for technical checks and automation. For the main creative phases, always follow the designated AI and phase order.

**Q: What happens if WORKLOG.md is not updated?**
A: According to PROJECT_RULES.md, any modification not recorded in WORKLOG.md is considered invalid. All participating AIs and humans are required to log changes immediately upon making them.

---

*NovelOS v1.0.0 — Keeping long-form novel development structured, ensuring worldbuilding integrity and work quality.*
