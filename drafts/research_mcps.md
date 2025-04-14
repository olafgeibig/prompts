## Research
I need to evaluate search providers that offer MCP servers. I need a good internet search for my complex prompts that use MCP servers to do complex tasks and I want to decide for a good search service. These prompts will be executed with top notch smart models with reasoning capabilities. There are two different kinds of approaches to search now

a. Classic. Traditional web search where then the prompted AI would have to look at the search result and then fetch and read the pages that seem to be interesting. 
b. AI powered.  Search services that already compile an answer out of a seacrh result with their own AI-researcher. To get the needed level of details the prompted LLM probably still needs to fetch the pages that are quoted by the service answer.

1. Compare regarding quality, rate limits and also cost. 
2. Look the features of the mcp-servers by reading the README from their github
3. Investigate the pros and cons of using classic search vs AI-search

### The contenders and their MCP servers 
AI search
- firecrawl.dev: https://github.com/mendableai/firecrawl-mcp-server
- tavily: https://github.com/tavily-ai/tavily-mcp
- exa search: https://github.com/exa-labs/exa-mcp-server
- perplexity: https://github.com/ppl-ai/modelcontextprotocol

Classic search: 
- Brave: https://github.com/modelcontextprotocol/servers/tree/main/src/brave-search
- Google Search: https://github.com/adenot/mcp-google-search
- serper.dev: https://github.com/NightTrek/Serper-search-mcp

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