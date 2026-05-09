# n8n Cloud — Step-by-Step Guide

> **Platform:** n8n Cloud (hosted at `app.n8n.cloud`)  
> **Version:** Cloud-managed (no installation required)  
> **Docs:** [docs.n8n.io](https://docs.n8n.io)

---

## Table of Contents

1. [Getting Started — Account Setup](#1-getting-started--account-setup)
2. [Understanding the n8n Interface](#2-understanding-the-n8n-interface)
3. [Creating Your First Workflow](#3-creating-your-first-workflow)
4. [Working with Nodes](#4-working-with-nodes)
5. [Triggers — Starting a Workflow](#5-triggers--starting-a-workflow)
6. [Setting Up Credentials](#6-setting-up-credentials)
7. [Using Expressions & Variables](#7-using-expressions--variables)
8. [Testing & Debugging](#8-testing--debugging)
9. [Activating & Scheduling Workflows](#9-activating--scheduling-workflows)
10. [Using AI Nodes](#10-using-ai-nodes)
11. [Managing Workflows](#11-managing-workflows)
12. [Tips & Best Practices](#12-tips--best-practices)

---

## 1. Getting Started — Account Setup

### Step 1: Create Your Account

1. Go to [https://app.n8n.cloud/register](https://app.n8n.cloud/register).
2. Enter your **email address** and create a **password**, or sign up with Google.
3. Verify your email via the confirmation link sent to your inbox.

### Step 2: Choose a Plan

1. After verifying your email, you will be prompted to select a plan.
2. A **free trial** is available — no credit card required initially.
3. Paid plans (Starter, Pro, Enterprise) unlock more executions, workflows, and advanced features.

### Step 3: Name Your Instance

1. Enter a name for your n8n workspace (e.g., `my-company`).
2. Your cloud instance URL will be: `https://<your-name>.app.n8n.cloud`
3. Click **Create** — your instance will be ready in seconds.

---

## 2. Understanding the n8n Interface

Once logged in, you'll land on the **main dashboard**. Here's an overview of key areas:

| Area | Description |
|------|-------------|
| **Left Sidebar** | Navigation: Workflows, Credentials, Variables, Executions, Settings |
| **Workflow Canvas** | The visual editor where you build automations |
| **Node Panel** | Opens when you add or click a node to configure it |
| **Top Bar** | Save, activate/deactivate toggle, execute, and workflow name |
| **Executions Tab** | Logs of all past workflow runs with input/output data |

### Key Concepts

- **Workflow** — A sequence of automated steps (nodes) connected together.
- **Node** — A single action or integration (e.g., send an email, query a database).
- **Trigger** — A special node that starts the workflow (e.g., a webhook, a schedule).
- **Credential** — Saved authentication details for third-party services.
- **Execution** — A single run of a workflow.

---

## 3. Creating Your First Workflow

### Step 1: Open the Workflow Editor

1. From the sidebar, click **Workflows**.
2. Click the **+ New Workflow** button (top right).
3. A blank canvas opens — this is your workflow editor.

### Step 2: Rename Your Workflow

1. Click the default name (e.g., "My Workflow") at the top of the canvas.
2. Type a descriptive name like `Send Daily Report` and press **Enter**.

### Step 3: Add a Trigger Node

1. Click the **+** button in the center of the canvas, or click **Add first step**.
2. The **node panel** slides open on the right.
3. Search for a trigger (e.g., `Schedule`, `Webhook`, `Gmail Trigger`).
4. Click the trigger node to add it to the canvas.

### Step 4: Add Action Nodes

1. Click the **+** button that appears on the right edge of your trigger node.
2. Search for an action (e.g., `Slack`, `Google Sheets`, `HTTP Request`).
3. Select a node and configure it in the right-hand panel.
4. Connect additional nodes by clicking the **+** connector on each node.

### Step 5: Save the Workflow

1. Click **Save** (top right) or press `Ctrl + S` / `Cmd + S`.

---

## 4. Working with Nodes

### Configuring a Node

1. Click any node on the canvas to open its settings panel.
2. Fill in the required fields (e.g., API endpoint, message text, filter conditions).
3. Use the **Input** tab (left side of panel) to see what data is coming in.
4. Use the **Output** tab to preview what the node will produce.

### Node Types

| Type | Examples |
|------|---------|
| **Trigger** | Schedule, Webhook, Gmail Trigger, Slack Trigger |
| **Action / Regular** | Send Email, HTTP Request, Google Sheets, Notion |
| **Transform** | Set, Merge, Split In Batches, Code |
| **Flow Control** | IF, Switch, Wait, Stop and Error |
| **AI** | AI Agent, OpenAI, Anthropic, Chat Model, Vector Store |

### Connecting Nodes

- Drag from the **right handle** of one node to the **left handle** of another.
- Use **IF** nodes to create conditional branching (true/false paths).
- Use **Merge** nodes to combine multiple branches back together.

### Deleting / Duplicating a Node

- **Right-click** a node to access options: Duplicate, Delete, Rename, Disable.
- Disabled nodes are skipped during execution (useful for testing).

---

## 5. Triggers — Starting a Workflow

Triggers define *when* and *how* a workflow starts. Common triggers on n8n Cloud:

### Schedule Trigger (Cron)

1. Add a **Schedule Trigger** node.
2. Set the interval: Every X minutes, hours, days, or a custom cron expression.
3. Example cron for every day at 8 AM: `0 8 * * *`

### Webhook Trigger

1. Add a **Webhook** node.
2. Copy the **Webhook URL** generated by n8n.
3. Paste this URL into the external service (e.g., GitHub, Stripe, your app).
4. Choose the HTTP method: `GET`, `POST`, `PUT`, etc.
5. Click **Listen for Test Event** to capture a sample payload.

### App Trigger (e.g., Gmail, Slack)

1. Add the app-specific trigger node (e.g., `Gmail Trigger`).
2. Connect credentials (see Section 6).
3. Set filters (e.g., "only trigger on emails with label X").
4. Use **Poll** mode (checks periodically) or **Instant** (real-time webhook) depending on the app.

### Manual Trigger

1. Add a **Manual Trigger** node.
2. Used during development — runs the workflow only when you click **Test workflow**.

---

## 6. Setting Up Credentials

Credentials store your API keys, OAuth tokens, and passwords securely.

### Step 1: Open Credentials

1. Click the **Credentials** option in the left sidebar, or
2. When configuring a node, click the **Credential** dropdown and select **Create New**.

### Step 2: Add a New Credential

1. Click **+ Add Credential**.
2. Search for the service (e.g., `OpenAI`, `Slack`, `Google Sheets`).
3. Follow the on-screen prompts — most services offer two options:
   - **OAuth2** — Click "Connect" and log in via a pop-up (simplest option).
   - **API Key** — Paste the key from the service's developer/settings page.

### Step 3: Assign Credential to a Node

1. Open the node that needs authentication.
2. In the **Credential** field, select the credential you just created.
3. The node will now use that credential for all API calls.

> **Tip:** Credentials are encrypted at rest and never exposed in logs or output data.

---

## 7. Using Expressions & Variables

Expressions let you pass dynamic data between nodes using the `{{ }}` syntax.

### Referencing Previous Node Output

To use data from a previous node:

```
{{ $json.fieldName }}
```

Example — pass an email from a Gmail trigger to a Slack message:

```
New email from: {{ $json.from }}
Subject: {{ $json.subject }}
```

### Useful Built-in Variables

| Variable | Description |
|----------|-------------|
| `$json` | The output data of the current/previous node |
| `$node["Node Name"].json` | Data from a specific named node |
| `$now` | Current timestamp (ISO 8601) |
| `$today` | Today's date |
| `$runIndex` | The current item index in a batch |
| `$workflow.id` | The ID of the current workflow |

### Using the Expression Editor

1. Click any input field in a node.
2. Click the **= (expression)** toggle icon that appears on the right of the field.
3. Type your expression in the editor that opens.
4. A live preview of the resolved value appears below the editor.

---

## 8. Testing & Debugging

### Test a Single Node

1. Click a node on the canvas.
2. Click **Test step** (play button inside the node panel).
3. Check the **Output** tab to see the result.

### Test the Full Workflow

1. Make sure your first node is a **Manual Trigger** (or has test data available).
2. Click **Test workflow** in the top bar.
3. Each node lights up green (success) or red (error) as it runs.
4. Click any node to inspect its input and output data.

### Re-running with Pinned Data

1. After a test run, click a node and find the output data.
2. Click the **pin icon** to pin this data.
3. Pinned data is reused for subsequent test runs without re-triggering the source.
4. Useful to avoid hitting external APIs repeatedly during development.

### Viewing Errors

1. A red node indicates an error.
2. Click the node → check the **Output** tab for the error message.
3. Common issues: wrong credentials, missing required fields, API rate limits.

### Execution Logs

1. Go to **Executions** in the left sidebar.
2. See a list of all runs: timestamp, status (success/error/waiting), duration.
3. Click any execution to inspect each node's input/output data step by step.

---

## 9. Activating & Scheduling Workflows

### Activate a Workflow

1. Once your workflow is tested and ready, click the **Inactive** toggle in the top-right corner.
2. It turns green — the workflow is now **Active**.
3. Active workflows run automatically based on their trigger.

> **Note:** You must **save** the workflow before activating it.

### Deactivate a Workflow

1. Click the green **Active** toggle to turn it back to **Inactive**.
2. The workflow stops running automatically.

### Monitor Upcoming Executions (Schedule Trigger)

1. With a Schedule Trigger active, check the **Executions** tab to see past runs.
2. The next run time is shown in the trigger node settings.

---

## 10. Using AI Nodes

n8n Cloud has native support for building AI-powered workflows and agents.

### Setting Up an AI Agent

1. Add an **AI Agent** node to your canvas.
2. Connect a **Chat Model** node (e.g., `OpenAI Chat Model`, `Anthropic Chat Model`).
3. Connect a **Memory** node (e.g., `Window Buffer Memory`) to retain conversation context.
4. Optionally attach **Tool** nodes (e.g., `HTTP Request Tool`, `Calculator`, `Wikipedia`).

### Common AI Nodes

| Node | Purpose |
|------|---------|
| **AI Agent** | Orchestrates reasoning and tool use |
| **OpenAI Chat Model** | Connects to GPT-4o, GPT-4, etc. |
| **Anthropic Chat Model** | Connects to Claude models |
| **Embeddings OpenAI** | Generates vector embeddings |
| **Vector Store (Pinecone, Qdrant)** | Stores and retrieves embeddings for RAG |
| **Document Loader** | Loads text/PDF content for AI processing |
| **Summarization Chain** | Summarizes long text using an LLM |

### Passing User Input to an AI Node

1. Use a **Chat Trigger** to receive user messages.
2. Connect it to an **AI Agent** node.
3. The agent processes the message and responds automatically.

---

## 11. Managing Workflows

### Duplicate a Workflow

1. Go to **Workflows** in the sidebar.
2. Hover over a workflow and click the **three-dot menu (⋮)**.
3. Select **Duplicate**.

### Export a Workflow (JSON)

1. Open the workflow editor.
2. Click the **three-dot menu (⋮)** in the top bar → **Download**.
3. A `.json` file is saved to your computer — useful for backup or sharing.

### Import a Workflow

1. From the **Workflows** list, click **+ New Workflow**.
2. Click the **three-dot menu (⋮)** → **Import from File** or **Import from URL**.
3. Browse and select a `.json` workflow file.

### Folders & Organization

1. In the Workflows list, click **+ New Folder** to group workflows.
2. Drag workflows into folders or right-click → Move to Folder.

### Sharing & Collaboration (Pro/Enterprise)

1. Click **Share** in the workflow editor.
2. Invite team members by email.
3. Set permissions: **Viewer** (can see/run) or **Editor** (can modify).

---

## 12. Tips & Best Practices

### Naming Conventions

- Use descriptive names: `Send Invoice Reminder - Monthly` instead of `Workflow 1`.
- Prefix workflows by team or function: `[Sales] Lead Enrichment`, `[IT] Ticket Auto-Close`.

### Error Handling

- Add an **Error Trigger** workflow to catch failures across all workflows.
- Use **Stop and Error** nodes to intentionally halt with a clear message.
- Enable **Retry on Fail** in critical nodes (available in node settings).

### Performance

- Use **Split In Batches** when processing large lists (e.g., 1000+ records) to avoid timeouts.
- Use the **Wait** node to add deliberate delays between API calls and avoid rate limiting.

### Security

- Never hardcode API keys in node fields — always use **Credentials**.
- Use **Variables** (left sidebar → Variables) for environment-level configuration that can be reused across workflows.
- Restrict workflow access using **RBAC** roles (Enterprise plan).

### Using Templates

1. Click **Templates** in the left sidebar or visit [n8n.io/workflows](https://n8n.io/workflows).
2. Browse 8,500+ pre-built workflow templates.
3. Click **Use for free** → the workflow opens directly in your editor.
4. Adjust credentials and configuration to match your setup.

---

## Useful Links

| Resource | URL |
|----------|-----|
| n8n Cloud Login | https://app.n8n.cloud/login |
| Official Documentation | https://docs.n8n.io |
| Workflow Templates | https://n8n.io/workflows |
| Community Forum | https://community.n8n.io |
| Discord | https://discord.gg/n8n |
| YouTube Channel | https://www.youtube.com/c/n8n-io |
| Release Notes | https://docs.n8n.io/release-notes/ |

---

*Last updated: May 2026*
