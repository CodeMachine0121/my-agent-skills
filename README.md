# My Agent Skills

A collection of specialized skills that extend Claude Code's capabilities with focused workflows and domain-specific knowledge.

## Overview

This repository contains custom skills designed to enhance Claude's ability to assist with software engineering tasks. Each skill encapsulates best practices, workflow patterns, and structured approaches to solving specific categories of problems.

## Skills Included

### 1. **UI/UX Pro Max** 📐
**File:** `skills/ui-ux-pro-max/`

Comprehensive UI/UX design intelligence with searchable databases of:
- 50+ UI design styles (glassmorphism, minimalism, brutalism, neumorphism, etc.)
- 21 color palettes organized by product type
- 50 font pairings with Google Fonts integration
- 20+ chart types for data visualization
- 8 tech stacks (React, Next.js, Vue, Svelte, SwiftUI, React Native, Flutter, Tailwind)
- UX guidelines and best practices

**Key Features:**
- Python-based search system for design recommendations
- Pre-calculated product/industry recommendations
- Stack-specific implementation guidelines
- Professional UI checklist with common pitfalls
- Pre-delivery verification checklist

**Technology:** Python 3, CSV-based data storage

**Source:** Custom-developed skill system

---

### 2. **Systematic Debugging** 🐛
**File:** `skills/systematic-debugging/`

A disciplined 4-phase approach to finding and fixing bugs without guessing or patching symptoms.

**Four Phases:**
1. **Root Cause Investigation** - Read errors, reproduce consistently, check changes, gather evidence
2. **Pattern Analysis** - Find working examples, identify differences
3. **Hypothesis & Testing** - Form testable theory, validate with minimal changes
4. **Implementation** - Create failing test, implement fix, verify

**Supporting Techniques:**
- Root cause tracing through call stacks
- Defense-in-depth validation patterns
- Condition-based waiting (replacing arbitrary timeouts)

**Key Principles:**
- NO FIXES WITHOUT ROOT CAUSE FIRST
- Scientific method for debugging
- Architectural problem detection (after 3+ failed fixes)

**Technology:** Markdown-based guides with TypeScript examples

**Source:** Custom-developed debugging methodology

---

### 3. **Writing Skills** 🛠️
**File:** `skills/writing-skills/`

Guide for creating effective, production-ready skills for Claude Code. Covers:
- Skill structure and format
- Workflow design patterns
- Data organization
- Testing and validation

**Technology:** Markdown documentation

**Source:** Custom skill development framework

---

### 4. **Writing Plans** 📋
**File:** `skills/writing-plans/`

Systematic approach to planning software implementations before coding:
- Requirements analysis
- Architecture design
- Multi-step task decomposition
- Progress tracking

**Technology:** Markdown-based planning templates

**Source:** Custom planning methodology

---

### 5. **Subagent-Driven Development** 🤖
**File:** `skills/subagent-driven-development/`

Framework for decomposing complex tasks into parallel sub-tasks, delegating work to specialized agents:
- Task decomposition patterns
- Agent capability matching
- Parallel execution coordination
- Result synthesis

**Technology:** Markdown-based workflow guides

**Source:** Custom agent orchestration methodology

---

### 6. **Component Refactoring** ♻️
**File:** `skills/component-refactoring/`

Specialized approach for refactoring high-complexity React components:
- Complexity analysis (thresholds: >50 complexity, >300 lines)
- Code splitting strategies
- Hook extraction patterns
- Performance optimization

**Target Stack:** React/Next.js frontend

**Technology:** Markdown guides with React examples

**Source:** Custom React optimization methodology

---

### 7. **TDD (Test-Driven Development)** ✅
**File:** `skills/tdd/`

Test-driven development expert guide implementing RED-GREEN-REFACTOR cycle:
- Writing failing tests first
- Minimal implementation
- Refactoring with confidence

**Language:** Traditional Chinese documentation

**Technology:** Markdown testing methodology

**Source:** Custom TDD framework

---

### 8. **DDD (Domain-Driven Design)** 🏛️
**File:** `skills/ddd/`

Domain-Driven Design methodology for complex software architecture:
- Ubiquitous language
- Bounded contexts
- Entity and value object design
- Aggregate patterns

**Technology:** Markdown-based design patterns

**Source:** Custom DDD methodology

---

### 9. **Brainstorming** 💡
**File:** `skills/brainstorming/`

Structured creative problem-solving before implementation:
- Requirements exploration
- Design space analysis
- Option generation and evaluation
- Trade-off analysis

**Technology:** Markdown workflow guide

**Source:** Custom ideation methodology

---

## Project Structure

```
my-agent-skills/
├── README.md                           # This file
├── .git/                               # Git repository
├── .claude/                            # Claude Code configuration
└── skills/                             # Skill definitions
    ├── brainstorming/
    ├── component-refactoring/
    ├── ddd/
    ├── subagent-driven-development/
    ├── systematic-debugging/
    │   ├── SKILL.md                    # Skill metadata and workflow
    │   ├── root-cause-tracing.md       # Supporting technique
    │   ├── defense-in-depth.md         # Supporting technique
    │   ├── condition-based-waiting.md  # Supporting technique
    │   └── test-*.md                   # Usage examples
    ├── tdd/
    │   └── SKILL.md
    ├── ui-ux-pro-max/
    │   ├── SKILL.md                    # Skill metadata and workflow
    │   ├── scripts/
    │   │   ├── core.py                 # Search engine
    │   │   └── search.py               # CLI interface
    │   └── data/                       # Design databases
    │       ├── products.csv
    │       ├── colors.csv
    │       ├── styles.csv
    │       ├── typography.csv
    │       ├── charts.csv
    │       ├── ux-guidelines.csv
    │       ├── landing.csv
    │       └── stacks/
    ├── writing-plans/
    │   └── SKILL.md
    ├── writing-skills/
    │   └── SKILL.md
    └── [other skills]/
```

## How to Use

### Understanding Skill Format

Each skill follows this structure:

1. **SKILL.md** - Contains frontmatter metadata and workflow documentation
   - `name`: Skill identifier
   - `description`: When and how to use this skill
   - Detailed workflow steps and examples

2. **Supporting Files** - Additional documentation, scripts, or data
   - Scripts (Python, TypeScript, etc.)
   - Databases (CSV files with searchable data)
   - Technique guides (detailed methodology)
   - Examples and test cases

### How Claude Uses These Skills

Skills are triggered through the `/skillname` command when they match the user's request. For example:

- User: "Help me debug this issue" → Triggers `systematic-debugging` skill
- User: "Design a landing page" → Triggers `ui-ux-pro-max` skill
- User: "Create a test" → Triggers `superpowers:test-driven-development` skill

### Adding New Skills

To create a new skill:

1. Create a directory: `skills/your-skill-name/`
2. Add `SKILL.md` with metadata and workflow
3. Add supporting documentation, scripts, or data
4. Document clearly with examples
5. Test workflow integration

See `skills/writing-skills/` for detailed guidance on skill creation.

## Data Sources & Attribution

### UI/UX Pro Max Databases

The design intelligence databases come from:

- **Color Palettes:** Industry-standard palettes for SaaS, e-commerce, healthcare, beauty, fintech, and service businesses
- **Typography:** Google Fonts pairings curated for different design aesthetics
- **Styles:** Modern design system trends (glassmorphism, minimalism, brutalism, neumorphism, bento grid, flat design, etc.)
- **UX Guidelines:** Best practices from WCAG, material design, and modern web standards
- **Tech Stack Guides:** Framework-specific patterns from official documentation

### Methodology Sources

- **Systematic Debugging:** Based on scientific debugging methodology and error analysis best practices
- **TDD:** Classic red-green-refactor cycle from Kent Beck's TDD methodology
- **DDD:** Eric Evans' Domain-Driven Design principles
- **Component Refactoring:** React performance optimization patterns from official React docs
- **UI/UX Guidelines:** Professional UI design best practices from design systems and accessibility standards

## Technology Stack

### Languages & Frameworks
- **Python 3** - Search engine for UI/UX databases
- **Markdown** - Skill documentation and workflows
- **TypeScript/JavaScript** - Example code and patterns
- **React** - Frontend component examples

### Data Storage
- **CSV files** - Searchable design databases
- **Markdown** - Workflow documentation and guides

### Tools & Integration
- **Claude Code CLI** - Skill execution framework
- **Git** - Version control

## Version Information

- **Latest Commit:** 0a0c59b - feat: add skills
- **Repository:** Git-enabled
- **Platform:** macOS (Darwin 25.2.0)

## Contributing

To improve or extend these skills:

1. Update relevant skill documentation in `skills/[skill-name]/SKILL.md`
2. Add new techniques or examples to supporting files
3. Expand databases (CSV files) with new entries
4. Test the workflow with real use cases
5. Document changes and sources

## License

These skills are custom-developed tools for the Claude Code ecosystem.

## Related Resources

- **Claude Code Documentation:** Official Claude Code CLI guide
- **Skill Creator Guide:** `skills/writing-skills/SKILL.md`
- **UI/UX Pro Max:** `skills/ui-ux-pro-max/SKILL.md`
- **Systematic Debugging:** `skills/systematic-debugging/SKILL.md`

---

**Last Updated:** 2026-02-11
**Maintained for:** Claude Code / Claude Opus 4.6
