# Build Your First MCP Server: Leave Management
This AI tool helps an HR with leave management related tasks. The codebase here 
is for MCP server that interacts with mock leave database and responds to MCP client queries

# Setup steps
1. Install Claude Desktop
2. install mcp using `pip install mcp`
3. Install uv by running `pip install uv`
4. Run `uv init my-first-mcp-server` to create a project directory
5. Run `uv add "mcp[cli]"` to add mcp cli in your project
6. Few folks may get type errors for which you can run `pip install --upgrade typer` to upgrade typer library to its latest version
7. Write code in main.py for leave management server
8. Install this server inside Claude desktop by running `uv run mcp install main.py` in the project directory
9. Kill any running instance of Claude from Task Manager. Restart Claude Desktop
10. In Claude desktop, now you will see tools from this server

@All rights reserved. Codebasics Inc. LearnerX Pvt Ltd. 

