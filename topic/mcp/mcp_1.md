
## MCP - Model Context Protocol 

- [Model Context Protocol Servers](#MCP-Servers-1)
- [Python-sdk](#python-sdk-1)


#

## Anthropic - Original MCP BLOG -- 
- #### relevant quotes from - 
- https://www.anthropic.com/news/model-context-protocol
-  Yet even the most sophisticated models are constrained by their isolation from data—trapped behind information silos and legacy systems. 
#
- Model Context Protocol 

The Model Context Protocol is an open standard that enables developers to build secure, two-way connections between their data sources and AI-powered tools. The architecture is straightforward: developers can either expose their data through MCP servers or build AI applications (MCP clients) that connect to these servers.

#
##### Model Context Protocol Servers
<p id="MCP-Servers-1">
...
</p>

- https://github.com/modelcontextprotocol/servers

#

###### Python SDK 
<p id="python-sdk-1">
...
</p>
- https://github.com/modelcontextprotocol/python-sdk

#
### install uv - 

- https://docs.astral.sh/uv/#highlights

#

```bash
dhankar@dhankar-1:~/.../mcp_1$ curl -LsSf https://astral.sh/uv/install.sh | sh
downloading uv 0.7.12 x86_64-unknown-linux-gnu
no checksums to verify
installing to /home/dhankar/.local/bin
  uv
  uvx
everything's installed!
dhankar@dhankar-1:~/.../mcp_1$ 

```
#
- https://docs.astral.sh/uv/guides/install-python/#reinstalling-python

```bash
dhankar@dhankar-1:~/.../mcp_1$ uv python install
Installed Python 3.13.4 in 4.00s
 + cpython-3.13.4-linux-x86_64-gnu
dhankar@dhankar-1:~/.../mcp_1$
dhankar@dhankar-1:~/.../mcp_1$ uv init mcp-server-demo
Initialized project `mcp-server-demo` at `/home/dhankar/temp/04_25/mcp_1/mcp-server-demo`
dhankar@dhankar-1:~/.../mcp_1$ 
dhankar@dhankar-1:~/.../mcp_1$ cd mcp-server-demo/
dhankar@dhankar-1:~/.../mcp-server-demo$ ls -lahtr
total 28K
-rw-rw-r-- 1 dhankar dhankar    0 Jun  7 20:07 README.md
-rw-rw-r-- 1 dhankar dhankar    5 Jun  7 20:07 .python-version
-rw-rw-r-- 1 dhankar dhankar  161 Jun  7 20:07 pyproject.toml
-rw-rw-r-- 1 dhankar dhankar   93 Jun  7 20:07 main.py
-rw-rw-r-- 1 dhankar dhankar  109 Jun  7 20:07 .gitignore
drwxrwxr-x 7 dhankar dhankar 4.0K Jun  7 20:07 .git
drwxrwxr-x 3 dhankar dhankar 4.0K Jun  7 20:07 ..
drwxrwxr-x 3 dhankar dhankar 4.0K Jun  7 20:07 .
dhankar@dhankar-1:~/.../mcp-server-demo$ 

```

#

uv init mcp-server-demo
cd mcp-server-demo





- [Omni Response](#omni-response-1)
- [Gemini Response](#gemini-response-1)
- [DeepSeek Response](#deepseek-response-1)

