# Adding an MCP server

MCP (Model Context Protocol) is a standard way to plug tools and data sources into an agent. In this case we use one to let the agent read PDF and PowerPoint files directly, instead of relying on text versions.

> Your organisation decides which MCP servers are allowed. If adding a server fails, the policy may not allow it. Ask the data academy team.

## Example: MarkItDown

[MarkItDown](https://github.com/microsoft/markitdown) is an open-source Microsoft tool that converts PDF, Word, PowerPoint and Excel files to markdown. Its MCP server gives the agent a tool to read those files.

**Requirements:** Python 3.10 or later on your laptop.

### 1. Install the server

```bash
pip install markitdown-mcp
```

### 2. Add it to Copilot

**From the terminal** (Copilot CLI):

```bash
copilot mcp add markitdown -- markitdown-mcp
```

**Or by editing the configuration file** `~/.copilot/mcp-config.json`:

```json
{
  "mcpServers": {
    "markitdown": {
      "type": "stdio",
      "command": "markitdown-mcp",
      "args": [],
      "tools": ["*"]
    }
  }
}
```

**In the Copilot app:** open the MCP server settings and add the same server. The app uses the same Copilot configuration as the CLI.

### 3. Use it

Start a new session and ask, for example:

*"Use the markitdown tool to read sources/bcbs239.pdf and list the titles of all principles."*

To let a custom agent use the server, add it to the agent's tools. For example, add `'markitdown/*'` to the `tools:` list in the agent's frontmatter.

## Check before you trust it

- Ask the agent which tool it used. Did it really read the file, or did it answer from memory?
- Spot-check one quote against the original PDF.
