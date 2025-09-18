# Forked from PRD PowerBomb, altered rules for preference

![PRD PowerBomb](README.png)

A comprehensive Product Requirements Document (PRD) management system for coding with LLMs. As seen on "How I AI" with Claire Vo: https://youtu.be/_fD1PwltbuE?si=ZsbrZZmUA_UqziSm

## Overview

PRD PowerBomb is designed to streamline the product development process by providing structured workflows for creating, reviewing, and executing product requirements documents with LLM coding agents.

## Features

- **PRD Creation & Management**: Structured workflows for creating and managing product requirements documents
- **AI-Powered Review**: Automated review processes with quality assurance
- **Linear Integration**: Seamless integration with Linear for project tracking
- **Code Quality Standards**: Built-in rules for maintaining high code quality
- **Swift Development Support**: Specialized rules for iOS/Swift development
- **Rubber Duck Debugging**: AI-assisted debugging workflows

## Project Structure

```
prd-powerbomb/
├── .cursor/
│   └── rules/           # Cursor AI rules for project workflows
├── README.md            # This file
└── .git/               # Git repository
```

## Cursor Rules

This project uses custom Cursor AI rules to enhance development workflows. 

- **01-communication-rules.mdc**: Communication guidelines and standards
- **02-prd-create.mdc**: Converts ideas/feature requests into hybrid PRD/tech spec documents
- **03-prd-review.mdc**: Converts PRD into phased checklist with git safety measures
- **04-prd-execute.mdc**: Execution guidelines and implementation workflows
- **05-prd-refactor.mdc**: Breaks down unmanageable codebases into smaller, maintainable chunks
- **06-prd-rubberduck.mdc**: AI-assisted debugging when LLM gets stuck, useful for learning
- **07-code-quality.mdc**: Prevents bad AI-generated code patterns and "AI slop"

## Getting Started

1. Clone the repository:
   ```bash
   git clone https://github.com/itsmeterrylin/prd-powerbomb.git
   cd prd-powerbomb
   ```

2. The project is ready to use with Cursor AI rules already configured. It is also usable with other coding agents such as Claude Code or Codex by simply @ the specific rule files.

## Usage

### Setup Phase
1. **Create Documentation**: Start by creating markdown files documenting your:
   - **Backend architecture** (APIs, databases, services)
   - **Frontend structure** (components, routing, state management)
   - **Project overview** (tech stack, deployment, environment)

2. **Reference in Rules**: Use these documentation files as reference guides in your Cursor rules for context-aware AI assistance.

### Development Workflow
When you have a new feature idea or requirement:

1. **Create PRD**: Use `02-prd-create.mdc` to generate a structured Product Requirements Document. Input is an idea or feature request, which gets broken down into problem statements and core components to create a hybrid PRD/tech spec document.

2. **Review PRD**: Run the PRD through `03-prd-review.mdc` for validation and quality checks. Input is a PRD document from the previous rule - this rule primarily converts it into a phased checklist. This is the pre-flight checklist before your LLM goes off and codes. The LLM is specifically instructed to pause after each phase when there's a git commit and some self-QA was done. 

## Tasks

### [Phase] (1.0) - [Category]
- [ ] 1.0 `git commit -m "[Layer]: [Brief description of goal for this phase]"`
- [ ] 1.1 [Specific task description]
- [ ] 1.2 [Specific task description]
- [ ] 1.3 [Specific task description]
- [ ] 1.4 [Specific QA validation command/test]
- [ ] 1.5 [Pause for user confirmation before next phase]


3. **Execute**: When ready to implement, use `04-prd-execute.mdc` to guide the development process

### Additional Tools
- **Refactoring**: Use `05-prd-refactor.mdc` for code improvements. This is for when the codebase gets unmanageable or you have long files that run up context windows with an LLM. This rule helps take an existing codebase and break it down into smaller, more maintainable chunks.

- **Debugging**: Use `07-rubberduck.mdc` for AI-assisted debugging. This is for when the LLM gets stuck, and you need to rubber duck the problem to get past something. Also useful for your own learning if you are new to coding.

- **Code Quality**: Follow `08-code-quality.mdc` standards. LLMs can generate very bad code such as nested logic with 9 layers deep. This rule is to avoid scenarios like that with very bad AI slop.

The Cursor rules provide AI assistance for:
- Creating structured PRDs
- Reviewing and validating requirements
- Executing development tasks
- Refactoring code
- Integrating with Linear
- Maintaining code quality
- Swift development best practices

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Commit and push to your branch
5. Create a pull request

## License

This project is open source and available under the [MIT License](LICENSE).

## Contact

- GitHub: [@itsmeterrylin](https://github.com/itsmeterrylin)
- Project: [PRD PowerBomb](https://github.com/itsmeterrylin/prd-powerbomb)

---

*Built with ❤️ for better product development workflows*
