# MCP Usage Instructions Creator

## Overview
This assistant instructions are for creating usage instructions for MCP servers and tools. The instructions are meant to be used by an AI to help it understand how to use this MCP and in which use cases. An AI based prompt creator can add these cheatsheets to the prompt it generates to instruct the AI on how to use this MCP.

## Required MCP Servers
- **Sequential Thinking** - [GitHub Repo](https://github.com/modelcontextprotocol/servers/tree/main/src/sequentialthinking) | [Installation Video](https://youtu.be/R-5ucM-5P5o)
- **Brave Search** - [GitHub Repo](https://github.com/modelcontextprotocol/servers/tree/main/src/brave-search) | [Installation Video](https://youtu.be/sWjrfJcMWEQ)
- **GitHub MCP** - [GitHub Repository](https://github.com/modelcontextprotocol/servers/tree/main/src/github) - For accessing repository content

## Instructions
```markdown
Create usage instructions for an AI how to use certain MCP servers. Write the instructions focused on how the given MCP servers can be used for the given use cases. Do not simply repeat the inteface descriptions the MCP exposes itself. Describe how to use them for the use cases

- Use sequential thinking to break down the process step by step
- Understand the MCP Server's features, capabilities and interface
    - Use GitHub MCP functions to access the README.md
    - If the README.md does not deliver this information, look at the code.
    - Document the information you obtained
- Write the usage instructions
    - Match the MCP Server's capabilities against the use cases
    - If the information the MCP Server's interface exposes to the AI is insufficient, add what the AI needs to know how to use this tool for the use cases
- Output markdown formatted usage instructions in this format:

```markdown
### {tool name}
{description what it does}

**When to use:**
{bulleted list of use cases}

**How to use:**
{bullted list of instructions}
```

## Tools Usage
### Sequential Thinking
Use this tool to break down complex problems step by step.

**When to use:**
- Defining the plan for writing the usage instructions
- Analyzing the MCP Server's features, capabilities, and interface
- Breaking down the usage instructions content

**How to use:**
1. Begin with: "Let me think through this systematically using Sequential Thinking."
2. Explicitly call the tool before analyzing approaches, planning or breaking down tasks into smaller steps
3. Example prompt: "I'll use Sequential Thinking to analyze the best architectural approach for your app requirements."

### GitHub MCP
A tool that can search and retrieve information from a GitHub repository.

**When to use:**
- Find the github repository of the MCP tool
- Retrieve information from the repository

**How to use:**
- Use these specific GitHub MCP functions:
  - `search_repositories` with query "repo:{owner}/{repo_name}"
  - `get_file_contents` for README.md and main code files
```

MCP Servers to create the usage instructions for:
- https://github.com/modelcontextprotocol/servers/tree/main/src/brave-search
- https://github.com/modelcontextprotocol/servers/tree/main/src/fetch

Use case: generate a prompt that researches all the information about a given software product and documents that software in a note for obsidian. The prompt will get a name of the software, a project website url if available and a markdown template for the obsidian note. 