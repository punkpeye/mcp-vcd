# mcp-vcd

A model context protocol (MCP) server for value change dump (VCD) waveforms.

https://github.com/user-attachments/assets/9d1a6a64-de22-4b5a-a597-685c663c9c79

# Tools

- `get-signal`: Provide all changes of the specified signal name to the model's context. This is useful for large waveform files with many signals where you cannot fit the entire VCD file into the model's context window.

# Installation

`uv pip install --system mcp-vcd`

And add the following to your `claude_desktop_config.json`:

```json
"mcpServers": {
  "mcp-vcd": {
    "command": "uv",
    "args": [
      "run",
      "mcp-vcd"
    ]
  }
}
```
See [Anthropic's MCP documentation](https://modelcontextprotocol.io/quickstart/user) for more info.
