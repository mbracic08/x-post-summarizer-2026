# x-post-summarizer-2026

This repository summarizes a public figure's 2026 X posts using AI.

## Project Description
This project analyzes and summarizes recent posts from a specified public figure on X (formerly Twitter) during 2026. The example analyzed here is the user handle @llm_wizard.

The summary is generated using AI tools that leverage a LangGraph agent combined with GitHub MCP tools for repository operations and the X API v2 for retrieving posts.

## How It Was Built
- Utilizes a LangGraph agent to orchestrate tasks.
- Employs GitHub MCP tools to manage repository creation, file commits, branching, and pull requests.
- Uses the X API v2 to fetch recent posts from the specified user.

## Replicating the Process
To replicate this project, follow these steps:

1. **Set up your X API Bearer Token:**
   - Obtain your Bearer Token from the X developer portal.
   - Set it as an environment variable in your system:
     ```bash
     export X_BEARER_TOKEN='your_bearer_token_here'
     ```

2. **Install Python dependencies:**
   - This project requires the `requests` library.
   - Install it using pip:
     ```bash
     pip install requests
     ```

3. **Run the search script:**
   - Use the provided `x_search.py` script to fetch recent posts:
     ```bash
     python x_search.py <x_handle>
     ```
   - Replace `<x_handle>` with the desired X username (default is `llm_wizard`).

4. **Review the generated summary:**
   - The script outputs a `posts.json` file with the fetched posts.
   - Use AI tools or manual methods to analyze and summarize the data.

---

Feel free to explore and extend this project for other users or additional analysis features.
