# Rules Library for Cursor IDE

A comprehensive library of development rules and documentation guidelines for projects using the Cursor IDE.

## Quick Start

1. Review the [Documentation Guidelines](docs/rules/documentation.mdc) for how to document and journal your work.
2. Familiarize yourself with all [Project Rules](#rules-overview) before contributing code.
3. Check the [Project Journal](docs/prompt-journal.md) for recent milestones and context.
4. Use the [Chat Interaction Rules](docs/rules/chat.mdc) when working with Cursor AI.
5. Follow the [Git Rules](docs/rules/git.mdc) for version control, commit, and branching best practices.

## Usage

To integrate this rules library into your own Cursor project:

1. **Copy the Rules and Documentation**
   - Copy the the rules you want from  `docs/rules/` directory and paste them into your project's `.cursor/rules/`.
   - Optionally, copy `docs/prompt-journal.md` and `docs/logs/` if you want to maintain journaling and logs.

2. **Update References**
   - Adjust any project-specific references in the rules files (e.g., file paths, team conventions).
   - Update the `README.md` in your project to reference the rules and documentation as needed.

3. **Adopt the Workflow**
   - Follow the documentation, journaling, and version control practices described in the rules.
   - Use the Chat Interaction Rules when working with Cursor AI.
   - Track rule usage with the analytics system if desired.

4. **Customize as Needed**
   - Modify or extend the rules to fit your team's workflow or technology stack.
   - Add new `.mdc` files for additional frameworks or processes.

5. **Best Practices**
   - Keep your rules and documentation up to date as your project evolves.
   - Encourage all contributors to review and follow the rules.
   - Regularly review the journal and logs for project history and technical decisions.

## Project Structure

```
.
├── docs/
│   ├── logs/                # Detailed analysis and logs
│   ├── prompt-journal.md    # Chronological project journal
│   └── rules/               # Rule definitions and documentation
│       ├── chat.mdc         # Chat interaction rules
│       ├── documentation.mdc# Documentation guidelines
│       ├── fastapi.mdc      # FastAPI implementation rules
│       ├── git.mdc          # Git version control and branching rules
│       ├── journal.mdc      # Project journal guidelines
│       ├── nextjs.mdc       # Next.js implementation rules
│       └── rule-analytics.mdc # Analytics tracking rules
```

## Rules Overview

- **[Documentation Rules](docs/rules/documentation.mdc):** How to document, journal, and cross-reference work.
- **[Journal Rules](docs/rules/journal.mdc):** Structure and standards for the project journal.
- **[Chat Rules](docs/rules/chat.mdc):** How to interact with Cursor AI and format responses.
- **[FastAPI Rules](docs/rules/fastapi.mdc):** Best practices for Python API development. Sourced from [playbooks.com/rules/fastapi](https://playbooks.com/rules/fastapi)
- **[Next.js Rules](docs/rules/nextjs.mdc):** Best practices for fullstack development with Next.js. Sourced from [playbooks.com/rules/nextjs](https://playbooks.com/rules/nextjs)
- **[Git Rules](docs/rules/git.mdc):** Version control, commit, and branching best practices.
- **[Analytics Rules](docs/rules/rule-analytics.mdc):** How rule usage is tracked and analyzed. Sourced from [playbooks.com/rules/rule-analytics](https://playbooks.com/rules/rule-analytics)

For detailed information, see the respective files in `docs/rules/`. 