# Rules Library for Cursor IDE

A comprehensive library of development rules and documentation guidelines for projects using the Cursor IDE, featuring enterprise-grade privacy, security, and responsible AI implementation standards.

## Quick Start

1. Review the [Documentation Guidelines](docs/rules/documentation.mdc) for how to document and journal your work with **mandatory date verification**.
2. Familiarize yourself with all [Project Rules](#rules-overview) before contributing code.
3. Check the [Project Journal](docs/prompt-journal.md) for recent milestones and context.
4. Use the [Chat Interaction Rules](docs/rules/chat.mdc) when working with Cursor AI.
5. Follow the [Git Rules](docs/rules/git.mdc) for version control, commit, and branching best practices.
6. **NEW**: Implement [Privacy & Security Rules](docs/rules/privacy-security.mdc) for secure development practices.
7. **NEW**: Apply [Responsible AI Rules](docs/rules/responsible-ai.mdc) based on Microsoft HAX Guidelines for ethical AI development.

## Recent Updates (2025-06-14)

- ✅ **Critical Date Accuracy Fix**: Implemented mandatory date verification for all documentation
- 🔒 **Privacy & Security Rules**: Comprehensive security guidelines with auto-attachment for all relevant file types
- 🤖 **Responsible AI Rules**: Complete Microsoft HAX Toolkit implementation with 18 guidelines and pattern catalog
- 📋 **Enhanced Documentation**: Mandatory date verification process to prevent timestamp errors
- 🎯 **Auto-Attachment**: Smart file type targeting for automatic rule application

## Usage

To integrate this rules library into your own Cursor project:

1. **Copy the Rules and Documentation**
   - Copy the rules you want from `docs/rules/` directory and paste them into your project's `.cursor/rules/`.
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
   - **CRITICAL**: Always verify current date before creating documentation entries
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
│   │   └── 2025-06-14-responsible-ai-implementation.md
│   ├── prompt-journal.md    # Chronological project journal
│   ├── responsible-ai-outline.md # Microsoft HAX pattern catalog
│   └── rules/               # Rule definitions and documentation
│       ├── chat.mdc         # Chat interaction rules
│       ├── documentation.mdc# Documentation guidelines with date verification
│       ├── fastapi.mdc      # FastAPI implementation rules
│       ├── git.mdc          # Git version control and branching rules
│       ├── journal.mdc      # Project journal guidelines
│       ├── nextjs.mdc       # Next.js implementation rules
│       ├── privacy-security.mdc # Privacy and security guidelines (NEW)
│       ├── responsible-ai.mdc   # Responsible AI implementation rules (NEW)
│       └── rule-analytics.mdc   # Analytics tracking rules
```

## Rules Overview

### Core Documentation & Process Rules
- **[Documentation Rules](docs/rules/documentation.mdc):** How to document, journal, and cross-reference work with **mandatory date verification**.
- **[Journal Rules](docs/rules/journal.mdc):** Structure and standards for the project journal.
- **[Chat Rules](docs/rules/chat.mdc):** How to interact with Cursor AI and format responses.
- **[Git Rules](docs/rules/git.mdc):** Version control, commit, and branching best practices.
- **[Analytics Rules](docs/rules/rule-analytics.mdc):** How rule usage is tracked and analyzed.

### Security & Ethics Rules
- **[Privacy & Security Rules](docs/rules/privacy-security.mdc):** 🔒 Comprehensive privacy and security guidelines with auto-attachment for all code, config, and infrastructure files.
- **[Responsible AI Rules](docs/rules/responsible-ai.mdc):** 🤖 Complete Microsoft HAX Toolkit implementation with 18 guidelines for ethical AI development.

### Technology-Specific Rules
- **[FastAPI Rules](docs/rules/fastapi.mdc):** Best practices for Python API development.
- **[Next.js Rules](docs/rules/nextjs.mdc):** Best practices for fullstack development with Next.js.

## Key Features

### 🔒 **Enterprise Security**
- File system access control and violation detection
- Third-party dependency security validation
- Sensitive data handling and API key management
- Global installation alerts and consent mechanisms

### 🤖 **Responsible AI Implementation**
- Microsoft HAX Guidelines (18 patterns) for ethical AI
- Proactive UI pattern implementation with auto-attachment
- Misleading AI practice detection and prevention
- Educational approach for complex AI implementations

### 📋 **Accurate Documentation**
- Mandatory date verification for all entries
- Chronological project journaling with verified timestamps
- Technical analysis logs with proper dating
- Cross-referenced documentation system

### 🎯 **Smart Auto-Attachment**
- Automatic rule application based on file types
- Technology-specific guidance and patterns
- Comprehensive coverage across development stack
- Performance-optimized targeting

## Getting Started with New Features

### Privacy & Security
1. Review the comprehensive security guidelines in `docs/rules/privacy-security.mdc`
2. Implement file system access controls and violation detection
3. Follow third-party dependency security criteria
4. Use proper sensitive data handling practices

### Responsible AI
1. Study the Microsoft HAX pattern catalog in `docs/responsible-ai-outline.md`
2. Apply the 18 guidelines from `docs/rules/responsible-ai.mdc`
3. Implement proactive UI patterns for AI features
4. Follow educational approach for complex AI implementations

### Documentation Accuracy
1. **ALWAYS** run `date` command before creating documentation
2. Use verified timestamps in all journal entries and logs
3. Follow the enhanced documentation standards
4. Maintain accurate chronological records

## Rule File Headers (.mdc Format)

### Privacy & Security Rule Header
```yaml
---
description: Privacy and Security Guidelines for AI Agent Operations
globs: **/*.{js,jsx,ts,tsx,py,java,go,rs,php,rb,cs,cpp,c,h,hpp,scala,kt,swift,dart,elm,clj,cljs,hs,ml,fs,ex,exs,erl,pl,lua,jl,nim,zig,v,cr,d,pas,ada,cob,f90,f95,f03,f08,for,m,mm,r,html,htm,css,scss,sass,less,styl,vue,svelte,json,yaml,yml,toml,xml,ini,conf,cfg,env,properties,sql,proto,thrift,graphql,ipynb,pyx,pxd,pxi,md,mdx,rst,txt,dockerfile,makefile,cmake,package.json,requirements.txt,pipfile,gemfile,pom.xml,build.gradle,cargo.toml,composer.json,setup.py,pyproject.toml,poetry.lock,yarn.lock,package-lock.json,pnpm-lock.yaml,go.mod,go.sum},**/*{.config.js,.config.ts},**/webpack.config.*,**/vite.config.*,**/next.config.*,**/nuxt.config.*,**/vue.config.*,**/angular.json,**/tsconfig.json,**/jsconfig.json,**/eslint.*,**/prettier.*,**/babel.*,**/rollup.*,**/gulpfile.*,**/gruntfile.*,**/*.env*,**/docker-compose.{yml,yaml},**/cmakelists.txt
alwaysApply: true
autoAttach: true
---
```

### Responsible AI Rule Header
```yaml
---
description: Responsible AI Implementation Rules based on Microsoft HAX Guidelines
globs: **/*.{js,jsx,ts,tsx,py,java,go,rs,php,rb,cs,cpp,c,h,hpp,scala,kt,swift,dart,elm,clj,cljs,hs,ml,fs,ex,exs,erl,pl,lua,jl,nim,zig,v,cr,d,pas,ada,cob,f90,f95,f03,f08,for,m,mm,r,html,htm,css,scss,sass,less,styl,vue,svelte,json,yaml,yml,toml,xml,ini,conf,cfg,env,properties,sql,proto,thrift,graphql,ipynb,pyx,pxd,pxi,md,mdx,rst,txt,dockerfile,makefile,cmake,package.json,requirements.txt,pipfile,gemfile,pom.xml,build.gradle,cargo.toml,composer.json,setup.py,pyproject.toml,poetry.lock,yarn.lock,package-lock.json,pnpm-lock.yaml,go.mod,go.sum},**/*{.config.js,.config.ts},**/webpack.config.*,**/vite.config.*,**/next.config.*,**/nuxt.config.*,**/vue.config.*,**/angular.json,**/tsconfig.json,**/jsconfig.json,**/eslint.*,**/prettier.*,**/babel.*,**/rollup.*,**/gulpfile.*,**/gruntfile.*,**/*.env*,**/docker-compose.{yml,yaml},**/cmakelists.txt
alwaysApply: true
autoAttach: true
---
```

### Key Features of Auto-Attachment Headers
- **Comprehensive File Coverage**: 70+ file extensions across all major programming languages
- **Smart Targeting**: Automatic application based on file type relevance
- **Always Apply**: `alwaysApply: true` ensures consistent rule enforcement
- **Auto Attach**: `autoAttach: true` enables automatic rule attachment
- **Technology Agnostic**: Covers frontend, backend, mobile, data science, and infrastructure files

For detailed information, see the respective files in `docs/rules/`.

---

**Last Updated**: 2025-06-14  
**Version**: 2.0  
**New Features**: Privacy & Security Rules, Responsible AI Rules, Mandatory Date Verification 