# Miyabi - Autonomous Development Plugin

Miyabi is an autonomous development framework that converts GitHub issues into completed pull requests using AI.

## Overview

Miyabi acts as an MCP (Model Context Protocol) server that integrates with Claude Code to provide autonomous development capabilities. It can analyze GitHub issues, generate implementation plans, write code, run tests, and create pull requests automatically.

## Features

- **Autonomous Issue Resolution**: Converts GitHub issues into completed pull requests
- **AI-Powered Code Generation**: Leverages Claude to write high-quality code
- **Test Integration**: Automatically runs tests to verify implementations
- **Pull Request Creation**: Creates PRs with detailed summaries and test plans
- **GitHub Integration**: Seamless integration with GitHub repositories

## Installation

### Prerequisites

- Node.js and npm installed
- GitHub personal access token with appropriate permissions
- Claude Code installed and configured

### Setup

1. Install the Miyabi plugin from the marketplace:
```bash
/plugin marketplace add https://github.com/ShunsukeHayashi/Miyabi.git
/plugin install miyabi
```

2. Configure your GitHub token:
```bash
export GITHUB_TOKEN="your_github_token_here"
```

3. The plugin will be available as an MCP server in your Claude Code session.

## Usage

Once installed, Miyabi provides autonomous development capabilities through the MCP server interface. You can:

1. Reference GitHub issues for automatic resolution
2. Request code generation with automatic testing
3. Create pull requests with AI-generated summaries

## Configuration

The plugin requires the following environment variable:

- `GITHUB_TOKEN`: Your GitHub personal access token with repo access

## Source Code

This plugin wraps the Miyabi framework available at:
https://github.com/ShunsukeHayashi/Miyabi.git

## License

MIT License - See the [source repository](https://github.com/ShunsukeHayashi/Miyabi) for details.

## Support

For issues or questions about this plugin, please visit the [Miyabi repository](https://github.com/ShunsukeHayashi/Miyabi/issues).
