# Build Your First MCP Server: Leave Management
This AI tool helps an HR with leave management related tasks. The codebase here 
is for MCP server that interacts with mock leave database and responds to MCP client queries

# Setup steps
1. Install Claude Desktop
2. You can use docker container for Ubuntu Linux
     ## Commands
      IMAGE_NAME="ke5haav/claude-desktop-builder:latest"
      DEB_FILE="claude-desktop_0.12.55_amd64.deb"
      
      # Run the script (or execute commands step-by-step)
      docker pull $IMAGE_NAME && \
      docker create --name claude-temp $IMAGE_NAME && \
      docker cp claude-temp:/home/appuser/claude-desktop-debian/$DEB_FILE . && \
      sudo dpkg -i $DEB_FILE && \
      sudo apt-get -f install -y && \
      rm $DEB_FILE && \
      echo "Done. Run: claude-desktop"

4. install mcp using `pip install mcp`
5. Install uv by running `pip install uv`
6. Run `uv init my-first-mcp-server` to create a project directory
7. Run `uv add "mcp[cli]"` to add mcp cli in your project
8. Few folks may get type errors for which you can run `pip install --upgrade typer` to upgrade typer library to its latest version
9. Write code in main.py for leave management server
10. Install this server inside Claude desktop by running `uv run mcp install main.py` in the project directory
11. Kill any running instance of Claude from Task Manager. Restart Claude Desktop
12. In Claude desktop, now you will see tools from this server

@All rights reserved. Codebasics Inc. LearnerX Pvt Ltd. 


