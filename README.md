# My Agent Skills

A collection of specialized skills that extend Claude Code's capabilities with focused workflows and domain-specific knowledge.

## Overview

This repository contains custom skills designed to enhance Claude's ability to assist with software engineering tasks. Each skill encapsulates best practices, workflow patterns, and structured approaches to solving specific categories of problems.

## Skills Included

### 1. **UI/UX Pro Max** 📐
**File:** `skills/ui-ux-pro-max/` | **Author:** @jameshsueh

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

**Source:** 🛠️ **Custom-developed by James Hsueh**
- Design trends and best practices curated from industry standards
- UX guidelines synthesized from WCAG, Material Design, and modern web standards
- Comprehensive original implementation with searchable database system

---

### 2. **Systematic Debugging** 🐛
**File:** `skills/systematic-debugging/` | **Author:** @jameshsueh

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

**Source:** 🛠️ **Custom-developed by James Hsueh**
- Original methodology combining software engineering best practices
- Inspired by scientific debugging principles and error analysis techniques
- Comprehensive phase-based workflow with supporting techniques

---

### 3. **Writing Skills** 🛠️
**File:** `skills/writing-skills/` | **Author:** @jameshsueh

Guide for creating effective, production-ready skills for Claude Code. Covers:
- Skill structure and format
- Workflow design patterns
- Data organization
- Testing and validation

**Technology:** Markdown documentation

**Source:** 🛠️ **Custom-developed by James Hsueh**
- Original skill development framework designed for Claude Code ecosystem
- Best practices for skill architecture and workflow design

---

### 4. **Writing Plans** 📋
**File:** `skills/writing-plans/` | **Author:** @jameshsueh

Systematic approach to planning software implementations before coding:
- Requirements analysis
- Architecture design
- Multi-step task decomposition
- Progress tracking

**Technology:** Markdown-based planning templates

**Source:** 🛠️ **Custom-developed by James Hsueh**
- Original planning methodology for software engineering tasks
- Structured approach to architectural planning and design

---

### 5. **Subagent-Driven Development** 🤖
**File:** `skills/subagent-driven-development/` | **Author:** @jameshsueh

Framework for decomposing complex tasks into parallel sub-tasks, delegating work to specialized agents:
- Task decomposition patterns
- Agent capability matching
- Parallel execution coordination
- Result synthesis

**Technology:** Markdown-based workflow guides

**Source:** 🛠️ **Custom-developed by James Hsueh**
- Original agent orchestration framework for Claude Code
- Patterns for parallel task execution and result synthesis

---

### 6. **Component Refactoring** ♻️
**File:** `skills/component-refactoring/` | **Author:** @jameshsueh

Specialized approach for refactoring high-complexity React components:
- Complexity analysis (thresholds: >50 complexity, >300 lines)
- Code splitting strategies
- Hook extraction patterns
- Performance optimization

**Target Stack:** React/Next.js frontend

**Technology:** Markdown guides with React examples

**Source:** 🛠️ **Custom-developed by James Hsueh**
- Original React optimization methodology
- Patterns inspired by React official documentation and community best practices

---

### 7. **TDD (Test-Driven Development)** ✅
**File:** `skills/tdd/` | **Author:** @jameshsueh

Test-driven development expert guide implementing RED-GREEN-REFACTOR cycle:
- Writing failing tests first
- Minimal implementation
- Refactoring with confidence

**Language:** Traditional Chinese documentation

**Technology:** Markdown testing methodology

**Source:** 📚 **Based on established TDD principles**
- Adapted from Kent Beck's Test-Driven Development methodology
- Tailored for Claude Code workflow and Chinese-speaking developers

---

### 8. **DDD (Domain-Driven Design)** 🏛️
**File:** `skills/ddd/` | **Author:** Tech Community

Domain-Driven Design methodology for complex software architecture:
- Ubiquitous language
- Bounded contexts
- Entity and value object design
- Aggregate patterns

**Technology:** Markdown-based design patterns

**Source:** 📚 **Based on established DDD principles**
- Adapted from Eric Evans' Domain-Driven Design book
- Standard patterns from the software architecture community

---

### 9. **Brainstorming** 💡
**File:** `skills/brainstorming/` | **Author:** @jameshsueh

Structured creative problem-solving before implementation:
- Requirements exploration
- Design space analysis
- Option generation and evaluation
- Trade-off analysis

**Technology:** Markdown workflow guide

**Source:** 🛠️ **Custom-developed by James Hsueh**
- Original ideation methodology for software development
- Synthesized from design thinking and creative problem-solving techniques

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

### Custom-Developed by James Hsueh 🛠️

These skills are original creations tailored for Claude Code:

- **UI/UX Pro Max** - Comprehensive design system with curated databases and Python search engine
- **Systematic Debugging** - 4-phase debugging methodology combining science and engineering best practices
- **Writing Skills** - Framework for creating Claude Code skills
- **Writing Plans** - Architecture planning methodology for software development
- **Subagent-Driven Development** - Agent orchestration patterns for parallel task execution
- **Component Refactoring** - React-specific complexity management and optimization
- **Brainstorming** - Creative problem-solving workflow for software design

### Based on Established Principles from the Tech Community 📚

These skills adapt well-known methodologies and best practices:

- **TDD (Test-Driven Development)**
  - Source: Kent Beck's Test-Driven Development methodology
  - Adapted: Tailored for Claude Code workflow

- **DDD (Domain-Driven Design)**
  - Source: Eric Evans' Domain-Driven Design book
  - Adapted: Standard patterns from software architecture community

### Referenced Standards & Best Practices

Throughout the skills, especially in UI/UX Pro Max and component design:

- **Accessibility:** WCAG 2.1 guidelines and standards
- **Design Systems:** Material Design, Tailwind CSS, industry design standards
- **Frontend Frameworks:** Official documentation (React, Vue, Next.js, Svelte, Flutter, SwiftUI)
- **Typography:** Google Fonts library and font pairing research
- **UX Patterns:** Modern web standards and interaction design best practices

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
