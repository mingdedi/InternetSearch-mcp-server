# Internetsearch-mcp-server
An MCP Server for Internet Search  
Based on the Bocha Search API  
Requires the use of Bocha AI's search service key. For specific documentation, please refer to the [Bocha Development Documentation](https://bocha-ai.feishu.cn/wiki/HmtOw1z6vik14Fkdu5uc9VaInBb).

**Usage Instructions**  
1、Clone the Repository
```bash
git clone https://github.com/mingdedi/Internetsearch-mcp-server.git
```
2、Set Up the Environment Using uv
```bash
pip install uv
uv venv
./.venv/Scripts/activate.bat
uv sync
```
3、Add Configuration in the Configuration File  
Add the following configuration in a similar format:
```json
{
  "mcpServers": {
    "Internetsearch-mcp-server": {
      "description": "Internetsearch-mcp-server",
      "command": "uv",
      "args": [
        "--directory",
        "/path/Internetsearch-mcp-server",
        "run",
        "Internet_search.py"
      ],
      "env": {
        "BOCHAAI_API_KEY": "sk-123456789412345678312323456789e"
      }
    }
  }
}
```

**Note**  
The key in the BOCHAAI_API_KEY is merely an example.   
If you need an actual usable key, please visit [BoCha AI](https://bochaai.com/)