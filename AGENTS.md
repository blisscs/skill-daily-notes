# Agent & Skill Configurations for Skill Study

This project uses opencode skills to automate learning workflows.

## Available Skills

### customize-opencode

**File:** `<built-in>`

A skill for customizing opencode's own configuration.

**Usage:** Use ONLY when editing opencode's own configuration: opencode.json, opencode.jsonc, files under .opencode/, or files under ~/.config/opencode/. Also use when creating or fixing opencode agents, subagents, skills, plugins, MCP servers, or permission rules.

---

### teacher

**File:** `<built-in>`

An educational agent that helps create personalized study plans. Capabilities:

- Reads learning topics from provided web links
- Compares new material against your existing knowledge base
- Generates structured study plans with milestones
- Creates study notes and summaries with **comparisons to Claude Code and Codex**
- Tracks learning progress over time

**Usage:** Invoke the teacher agent when you want to learn a new topic. Provide:
1. Web links to resources you want to learn from
2. Description of what you already know about the topic
3. Your learning goals or desired outcomes
4. **Note:** Always include comparisons with Claude Code and Codex workflows

**Special Instructions:**
- When generating study notes, **compare the topic with equivalent approaches in Claude Code and Codex**
- Highlight differences in workflows, syntax, and best practices
- Include examples showing how the same task would be accomplished in each tool

## Custom Skills (To Be Added)

As you learn, add new skills here. Structure:

```markdown
### my-custom-skill

**Description:** What this skill does.

**Usage:** When to use this skill.
```

---

## Agent Behavior Preferences

### Notifications
When an agent finishes a task and is waiting for user input, it should notify the user using the appropriate OS notification tool:
- **Linux:** Use `notify-send` (e.g., `notify-send "OpenCode" "Task completed. Waiting for your input."`)
- **macOS:** Use `osascript` (e.g., `osascript -e 'display notification "Task completed. Waiting for your input." with title "OpenCode"'`)
- **Windows:** Use PowerShell (e.g., `powershell -Command "Add-Type -AssemblyName System.Windows.Forms; [System.Windows.Forms.MessageBox]::Show('Task completed. Waiting for your input.', 'OpenCode')"`)

Always prefer native OS notification tools over sound alerts or terminal bells.