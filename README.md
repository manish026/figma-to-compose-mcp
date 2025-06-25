# figma-to-compose-mcp

> Generate pixel-perfect Jetpack Compose UI from Figma — with Copilot, Claude, or any MCP-supported client.

---

## 🚀 What is this?

This is an MCP server designed for Android developers that converts Figma design nodes into **Jetpack Compose** code.  
It works seamlessly with **GitHub Copilot**, **Claude**, and other tools that support MCP protocol.

## ✨ Features

- ⚡️ Instant Jetpack Compose code from your Figma design
- 🧠 Natural language support
- 🎯 Works with Copilot, Claude, or any MCP-compatible AI
- 💻 CLI alias for quick access

---

## 🧩 Requirements

- Python 3.13+
- [uv](https://github.com/astral-sh/uv) (a faster Python package installer)

---

## 🔧 Installation

To install uv (skip this step if it’s already installed):
```
pip install uv
```

Install the MCP server with:

```bash
uvx figma-to-compose-mcp
```

⚙️ Configuration

In your clients mcp.json add
```
{
  "servers": {
    "figmaToCompose": {
      "command": "uvx",
      "args": ["figma-to-compose-mcp"],
      "env": {
        "FIGMA_TOKEN": "YOUR_FIGMA_TOKEN"
      }
    }
  }
}
```

🖇️ Usage

Option 1: Natural Language (Copilot, Claude, etc.)

Just ask:

```
"Generate a Jetpack Compose layout for this Figma node: https://www.figma.com/file/..."
```

Option 2: CLI Alias (Quick + Lazy Devs 😎)

```
jc YOUR_FIGMA_NODE_URL
```

🙌 Acknowledgements

Built with ❤️ for Android devs who just want to code, not pixel-push.
