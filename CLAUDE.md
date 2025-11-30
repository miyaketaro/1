# CLAUDE.md

This file provides guidance for AI assistants (like Claude) when working with this repository.

## Project Overview

> **Note:** This is a new repository. Update this section with project details as it evolves.

- **Project Name:** [Project Name]
- **Description:** [Brief description of what this project does]
- **Primary Language:** [e.g., TypeScript, Python, Go]
- **Framework:** [e.g., React, Django, Express]

## Repository Structure

```
/
├── src/                    # Source code
├── tests/                  # Test files
├── docs/                   # Documentation
├── scripts/                # Build and utility scripts
├── .github/                # GitHub workflows and templates
└── CLAUDE.md               # This file - AI assistant guidance
```

> Update this structure as the project grows.

## Development Workflow

### Getting Started

```bash
# Clone the repository
git clone <repository-url>
cd <project-directory>

# Install dependencies
# npm install        # for Node.js projects
# pip install -r requirements.txt  # for Python projects

# Run the project
# npm start / npm run dev
# python main.py
```

### Common Commands

| Command | Description |
|---------|-------------|
| `npm install` / `pip install -r requirements.txt` | Install dependencies |
| `npm test` / `pytest` | Run tests |
| `npm run build` | Build for production |
| `npm run lint` | Run linter |
| `npm run format` | Format code |

> Update these commands based on the actual project setup.

## Code Conventions

### General Guidelines

1. **Keep changes focused** - Make minimal, targeted changes that address the specific task
2. **Follow existing patterns** - Match the style and conventions already in the codebase
3. **Write self-documenting code** - Use clear variable/function names; add comments only when logic isn't obvious
4. **Avoid over-engineering** - Don't add features, abstractions, or "improvements" beyond what's requested

### File Organization

- Group related files together in logical directories
- Keep file sizes manageable (consider splitting files over 300-400 lines)
- Use consistent naming conventions (kebab-case, camelCase, etc. as per project standards)

### Code Style

- Follow the project's linter configuration
- Use consistent indentation (spaces vs tabs as configured)
- Keep lines under 100-120 characters when possible
- Remove unused imports and dead code

## Testing Guidelines

### Running Tests

```bash
# Run all tests
npm test  # or pytest, go test, etc.

# Run specific test file
npm test -- path/to/test.spec.ts

# Run with coverage
npm test -- --coverage
```

### Writing Tests

1. Write tests for new functionality
2. Update tests when modifying existing code
3. Ensure all tests pass before committing
4. Aim for meaningful coverage, not 100% coverage

## Git Conventions

### Branch Naming

- `feature/` - New features
- `fix/` - Bug fixes
- `refactor/` - Code refactoring
- `docs/` - Documentation updates
- `test/` - Test additions/updates

### Commit Messages

Write clear, concise commit messages:
- Use present tense ("Add feature" not "Added feature")
- Keep the first line under 72 characters
- Reference issue numbers when applicable

Example:
```
Add user authentication endpoint

- Implement JWT token generation
- Add password hashing utility
- Create login/logout routes

Fixes #123
```

### Pull Requests

- Provide a clear description of changes
- Link related issues
- Include test plan or testing notes
- Request appropriate reviewers

## Important Notes for AI Assistants

### Before Making Changes

1. **Read before editing** - Always read and understand files before modifying them
2. **Check dependencies** - Understand how changes might affect other parts of the codebase
3. **Verify assumptions** - Don't assume file contents; read them first

### When Writing Code

1. **Match existing style** - Follow patterns already established in the codebase
2. **Avoid introducing vulnerabilities** - Be mindful of security (XSS, injection, etc.)
3. **Keep it simple** - Prefer straightforward solutions over clever ones
4. **Don't add unnecessary dependencies** - Use existing libraries when possible

### After Making Changes

1. **Run tests** - Ensure all tests pass
2. **Check for lint errors** - Run the linter if configured
3. **Verify the build** - Ensure the project builds successfully
4. **Test manually** - When applicable, verify changes work as expected

## Configuration Files

| File | Purpose |
|------|---------|
| `package.json` / `pyproject.toml` | Project dependencies and scripts |
| `.eslintrc` / `.flake8` | Linter configuration |
| `.prettierrc` / `black.toml` | Code formatter settings |
| `tsconfig.json` / `setup.cfg` | Language/build configuration |
| `.env.example` | Environment variable template |
| `.gitignore` | Git ignore patterns |

## Environment Variables

> List important environment variables here as the project develops.

| Variable | Description | Required |
|----------|-------------|----------|
| `NODE_ENV` | Environment (development/production) | Yes |
| `DATABASE_URL` | Database connection string | Yes |
| `API_KEY` | External API key | No |

## Troubleshooting

### Common Issues

> Document common issues and solutions as they arise.

1. **Issue:** [Description]
   - **Solution:** [How to fix]

2. **Issue:** [Description]
   - **Solution:** [How to fix]

## Writing Guidelines (matsumoto Style)

記事やドキュメントを執筆する際のルールです。

### 構成・段落

- 1段落は1〜3文まで、ほぼ毎文で改行
- 段落間には空行を入れる
- 記事は800〜1500文字程度を目安に

### 文体

- 「です・ます」調で統一
- 読者への問いかけを含める
- 問いかけの末尾には必ず「？」をつける（例：「〜ありませんか？」「〜ですよね？」）

### リード文の書き方

各セクションの冒頭には、以下を意識したリード文を入れる：

1. **なぜその話をするのか** - セクションの意義や目的を示す
2. **体験・考察**（適宜） - 筆者の経験や気づきを入れて具体性を持たせる
   - すべてに入れる必要はない
   - 読者がイメージしやすくなると判断した場合に入れる

### 避けるべきこと

- 絵文字・顔文字の使用
- 「超〜」「めっちゃ」などカジュアルすぎる表現
- 抽象的な説明だけで終わる（必ず具体例を添える）
- 読者への問いかけがない一方的な説明

## Work Process Rules

### フィードバックの反映

構成や内容についてフィードバックを受けた場合：

1. **具体的な修正** - 指摘された箇所を修正する
2. **抽象化** - フィードバックから汎用的な学びを抽出する
3. **ルールへの反映** - 抽象化した学びをCLAUDE.mdの該当セクションに追記する

これにより、同じ指摘を繰り返し受けることを防ぎ、継続的に品質を向上させる。

## Resources

- [Project Documentation](./docs/)
- [Contributing Guidelines](./CONTRIBUTING.md)
- [API Documentation](./docs/api/)

---

*Last updated: 2025-11-30*
