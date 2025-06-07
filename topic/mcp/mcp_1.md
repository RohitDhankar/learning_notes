
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

##### Yes -- fast 

```bash
dhankar@dhankar-1:~/.../mcp-server-demo$ uv add "mcp[cli]"
Using CPython 3.13.4
Creating virtual environment at: .venv
Resolved 29 packages in 362ms
Prepared 27 packages in 710ms
Installed 27 packages in 29ms
 + annotated-types==0.7.0
 + anyio==4.9.0
 + certifi==2025.4.26
 + click==8.2.1
 + h11==0.16.0
 + httpcore==1.0.9
 + httpx==0.28.1
 + httpx-sse==0.4.0
 + idna==3.10
 + markdown-it-py==3.0.0
 + mcp==1.9.3
 + mdurl==0.1.2
 + pydantic==2.11.5
 + pydantic-core==2.33.2
 + pydantic-settings==2.9.1
 + pygments==2.19.1
 + python-dotenv==1.1.0
 + python-multipart==0.0.20
 + rich==14.0.0
 + shellingham==1.5.4
 + sniffio==1.3.1
 + sse-starlette==2.3.6
 + starlette==0.47.0
 + typer==0.16.0
 + typing-extensions==4.14.0
 + typing-inspection==0.4.1
 + uvicorn==0.34.3
dhankar@dhankar-1:~/.../mcp-server-demo$ 

```
#
#### Running the standalone MCP development tools
- To run the mcp command with uv:

```bash

dhankar@dhankar-1:~/.../mcp-server-demo$ uv run mcp
                                                                                                                                              
 Usage: mcp [OPTIONS] COMMAND [ARGS]...                                                                                                       
                                                                                                                                              
 MCP development tools                                                                                                                        
                                                                                                                                              
                                                                                                                                              
╭─ Options ──────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
│ --help          Show this message and exit.                                                                                                │
╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
╭─ Commands ─────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
│ version   Show the MCP version.                                                                                                            │
│ dev       Run a MCP server with the MCP Inspector.                                                                                         │
│ run       Run a MCP server.                                                                                                                │
│ install   Install a MCP server in the Claude desktop app.                                                                                  │
╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
Usage: mcp [OPTIONS] COMMAND [ARGS]...
Try 'mcp --help' for help.
╭─ Error ────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╮
│                                                                                                                                            │
╰────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────────╯
dhankar@dhankar-1:~/.../mcp-server-demo$ 
```


uv init mcp-server-demo
cd mcp-server-demo





- [Omni Response](#omni-response-1)
- [Gemini Response](#gemini-response-1)
- [DeepSeek Response](#deepseek-response-1)

