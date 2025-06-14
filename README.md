# Rules Library for Cursor IDE

A comprehensive library of development rules and documentation guidelines for projects using the Cursor IDE, featuring enterprise-grade privacy, security, and responsible AI implementation standards.

## Quick Start

1. Review the [Documentation Guidelines](rules/documentation.mdc) for how to document and journal your work.
2. Familiarize yourself with all [Project Rules](#rules-overview) before contributing code.
3. Check the [Project Journal](docs/prompt-journal.md) for recent milestones and context.
4. Use the [Chat Interaction Rules](rules/chat.mdc) when working with Cursor AI.
5. Follow the [Git Rules](rules/git.mdc) for version control, commit, and branching best practices.
6. Implement [Privacy & Security Rules](rules/privacy-security.mdc) for secure development practices.
7. Apply [Responsible AI Rules](rules/responsible-ai.mdc) based on Microsoft HAX Guidelines for ethical AI development.

## Usage

To integrate this rules library into your own Cursor project:

1. **Copy the Rules and Documentation**
   - Copy the rules you want from `rules/` directory and paste them into your project's `.cursor/rules/`.
   - Optionally, copy `docs/prompt-journal.md` and `docs/logs/` if you want to maintain journaling and logs.

2. **Update References**
   - Adjust any project-specific references in the rules files (e.g., file paths, team conventions).
   - Update the `README.md` in your project to reference the rules and documentation as needed.

3. **Adopt the Workflow**
   - Follow the documentation, journaling, and version control practices described in the rules.
   - Use the Chat Interaction Rules when working with Cursor AI.
   - Implement privacy and security practices from the comprehensive security rules.
   - Apply responsible AI guidelines for any AI-enabled features.
   - Track rule usage with the analytics system if desired.

4. **Customize as Needed**
   - Modify or extend the rules to fit your team's workflow or technology stack.
   - Add new `.mdc` files for additional frameworks or processes.

5. **Best Practices**
   - Keep your rules and documentation up to date as your project evolves.
   - Encourage all contributors to review and follow the rules.
   - Regularly review the journal and logs for project history and technical decisions.
   - Implement security and responsible AI practices from day one.

## Project Structure

```
.
├── docs/
│   ├── analytics.md         # Rule usage tracking and analytics
│   ├── logs/                # Detailed analysis and technical logs
│   ├── prompt-journal.md    # Chronological project journal
│   └── responsible-ai-outline.md # Microsoft HAX pattern catalog
├── rules/                   # Rule definitions and documentation
│   ├── chat.mdc            # Chat interaction rules
│   ├── documentation.mdc   # Documentation guidelines with date verification
│   ├── fastapi.mdc         # FastAPI implementation rules
│   ├── git.mdc             # Git version control and branching rules
│   ├── journal.mdc         # Project journal guidelines
│   ├── nextjs.mdc          # Next.js implementation rules
│   ├── privacy-security.mdc # Privacy and security guidelines
│   ├── responsible-ai.mdc  # Responsible AI implementation rules
│   └── rule-analytics.mdc  # Analytics tracking rules
```

## Rules Overview

### Core Documentation & Process Rules
- **[Documentation Rules](rules/documentation.mdc):** How to document, journal, and cross-reference work with mandatory date verification.
- **[Journal Rules](rules/journal.mdc):** Structure and standards for the project journal.
- **[Chat Rules](rules/chat.mdc):** How to interact with Cursor AI and format responses.
- **[Git Rules](rules/git.mdc):** Version control, commit, and branching best practices.
- **[Analytics Rules](rules/rule-analytics.mdc):** How rule usage is tracked and analyzed.

### Privacy, Security & RAI Rules
- **[Privacy & Security Rules](rules/privacy-security.mdc):** 🔒 Comprehensive privacy and security guidelines with auto-attachment for all code, config, and infrastructure files.
- **[Responsible AI Rules](rules/responsible-ai.mdc):** 🤖 Complete Microsoft HAX Toolkit implementation with 18 guidelines for ethical AI development.

### Technology-Specific Rules
- **[FastAPI Rules](rules/fastapi.mdc):** Best practices for Python API development.
- **[Next.js Rules](rules/nextjs.mdc):** Best practices for fullstack development with Next.js.
- ** ADD 'EM IF YOU WANT 'EM**

For detailed information, see the respective files in `rules/`.

---

**Last Updated**: 2025-06-14  
**Version**: 2.0 