# My Claude Code Skills & Config

Personal collection of Claude Code skills and configurations.

## Skills

| Skill | Description | Source |
|-------|-------------|--------|
| planning-with-files | 3-file planning pattern (task_plan.md, findings.md, progress.md) | OthmanAdi |
| ui-ux-pro-max | UI/UX design intelligence with 50 styles, 21 palettes, 50 font pairings | Custom |
| react-best-practices | 40+ React/Next.js performance optimization rules | Vercel Labs |
| web-design-guidelines | 100+ accessibility, performance, and UX rules | Vercel Labs |
| composition-patterns | React component scaling and prop patterns | Vercel Labs |
| react-native-skills | 16 rules for mobile app development | Vercel Labs |
| vercel-deploy-claimable | Instant deployment to Vercel from Claude | Vercel Labs |
| notebooklm-skill | Generate AI podcasts using Google NotebookLM | PleasePrompto |

## Installation on New Computer

### 1. Clone this repo

```bash
git clone https://github.com/SheltonMark/claude_skill.git
```

### 2. Copy skills to global folder

**Windows (PowerShell):**
```powershell
Copy-Item -Recurse .\claude_skill\skills\* $env:USERPROFILE\.claude\skills\
```

**Windows (Git Bash):**
```bash
cp -r claude_skill/skills/* ~/.claude/skills/
```

**macOS/Linux:**
```bash
cp -r claude_skill/skills/* ~/.claude/skills/
```

### 3. Setup MCP Server (markitdown)

```bash
pip install markitdown-mcp
```

Then copy `mcp-config/claude_desktop_config.json` to:
- **Windows:** `%APPDATA%\Claude\claude_desktop_config.json`
- **macOS:** `~/Library/Application Support/Claude/claude_desktop_config.json`

**Note:** Update the Python path in the config file to match your new computer's Python installation.

### 4. Install Plugins (from marketplace)

```bash
# In Claude Code terminal
/plugin install superpowers@claude-plugins-official
/plugin install ralph-wiggum@claude-code-official
```

## Usage

| Tool | How to Use |
|------|------------|
| planning-with-files | `/plan` |
| ui-ux-pro-max | Describe UI/UX needs directly |
| ralph-wiggum | `/ralph-loop`, `/cancel-ralph` |
| markitdown (MCP) | Available in Claude Desktop |

## File Structure

```
claude_skill/
├── skills/
│   ├── planning-with-files/
│   ├── ui-ux-pro-max/
│   ├── react-best-practices/
│   ├── web-design-guidelines/
│   ├── composition-patterns/
│   ├── react-native-skills/
│   ├── vercel-deploy-claimable/
│   └── notebooklm-skill/
├── mcp-config/
│   └── claude_desktop_config.json
└── README.md
```
