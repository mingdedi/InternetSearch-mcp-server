# Internetsearch-mcp-server
一个用于联网搜索的MCP服务器

如何使用
1、将仓库git clone
```bash
git clone https://github.com/mingdedi/Internetsearch-mcp-server.git
```
2、使用uv重建环境
```bash
pip install uv
uv venv
./.venv/Scripts/activate.bat
uv sync
```
3、在配置文件中添加，类似格式如下
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
      ]
    }
  }
}
```

Usage Instructions
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
      ]
    }
  }
}
```