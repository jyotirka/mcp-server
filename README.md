*MCP Weather Server*
Documentation Reference: This project follows the official Model Context Protocol (MCP) Quickstart guide to build and integrate the MCP server.
https://modelcontextprotocol.io/quickstart/server#testing-your-server-with-claude-for-desktop
This is a simple MCP (Model Context Protocol) server that exposes weather tools (`get-alerts` and `get-forecast`) to be used by AI agents or custom applications.

*Features*

- Exposes two tools: 
  - `get-alerts`: Returns weather alerts for a given location
  - `get-forecast`: Returns the weather forecast for a given location
- Built using Python
- MCP-compatible: Can be used with Claude or any custom app via HTTP+JSON-RPC

*Steps to Run This Repository on Your System*

Follow the steps below to clone, set up, and run the MCP server:

1. Clone the Repository
   
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
   
2. Install Dependencies
Make sure you have Python installed, then run:

   pip install -r requirements.txt
   
3. Install Claude Desktop
   
Download and install Claude for Desktop from https://modelcontextprotocol.io/quickstart/server#testing-your-server-with-claude-for-desktop.

4. Run the MCP Server
To start the server:

mcp run file_name.py
To run the server with MCP Inspector (helpful for debugging):

mcp dev file_name.py

5. Integrate the Server with Claude Desktop
To let Claude use your server’s tools, run:
mcp install file_name.py

You should see this confirmation in your terminal:
Added server 'weather' to Claude config
Successfully installed weather in Claude app

This means your MCP weather server is successfully integrated with Claude Desktop and ready to use.

VERIFYING THE INTEGRATION

Open Claude for Desktop.

Click on the sidebar menu (top-left corner).

Go to Files > Settings > Developer.

You should see your weather server listed and running.
