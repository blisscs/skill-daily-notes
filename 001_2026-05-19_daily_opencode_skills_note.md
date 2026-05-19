# 🚀 Daily Study Note #001: Mastering opencode Skills with Visuals

## **📌 Introduction: Why Skills Matter**
Imagine you're working in opencode and find yourself repeating the same tasks:
- Searching for files.
- Editing configurations.
- Running commands.

**Skills are your superpower!** They automate these tasks so you can focus on what matters.

Today, you'll learn:
✅ What skills are and how they work.
✅ How to **invoke and use** skills in your workflow.
✅ How to **explore and experiment** with skills hands-on.
✅ How skills compare to **Claude Code** and **Codex** equivalents.

---

## **🔍 Key Concepts: Skills vs. Agents**

### **📊 Comparison Table**
| **Feature**       | **Skills**                          | **Agents**                          |
|-------------------|-------------------------------------|-------------------------------------|
| **Purpose**       | Task-specific (e.g., "Edit config"). | General-purpose (e.g., "Teach me"). |
| **Scope**         | Narrow (e.g., "List agents").      | Broad (e.g., "Help me learn Python"). |
| **Invocation**     | `skill <skill-name>`                | Triggered by user requests.          |
| **Example**       | `customize-opencode`                | `Teacher Agent`                     |

---

## **🌐 Comparison: opencode vs Claude Code vs Codex**

### **📊 Skills Feature Comparison**

| **Feature**        | **opencode**                          | **Claude Code**                      | **Codex**                          |
|--------------------|---------------------------------------|--------------------------------------|------------------------------------|
| **Skill System**   | ✅ `skill <name>` - Built-in skill loader | ❌ No native skill system            | ❌ No native skill system          |
| **Agent System**   | ✅ Multiple specialized agents         | ✅ "Agents" via prompts              | ✅ Limited agent functionality     |
| **Config File**    | ✅ `AGENTS.md` - Define custom agents | ⚠️ Via system prompts only          | ⚠️ Via system prompts only        |
| **Task Automation**| ✅ Skills automate repetitive tasks   | ⚠️ Manual prompt engineering         | ⚠️ Manual prompt engineering       |
| **Built-in Skills**| ✅ `customize-opencode`, `teacher`, etc. | ❌ None                              | ❌ None                            |

### **🔑 Key Differences**

#### **opencode Skills**
```bash
# Invoke a skill
skill teacher

# List available skills
skill --help
```
- **Built-in**: Comes with ready-to-use skills
- **AGENTS.md**: Define custom skills locally
- **Automation**: Skills automate specific tasks

#### **Claude Code**
```bash
# No native skill system
# Use custom prompts instead
# Create "role" prompts like:
Claude, act as a Python expert...
```
- **No skill tool**: Must use prompt engineering
- **Custom prompts**: Create reusable prompt templates
- **Manual**: Must remind Claude of your context each time

#### **Codex**
```bash
# No native skill system
# Similar to Claude Code - use prompts
Codex, help me with DevOps tasks...
```
- **No skill tool**: Uses prompt-based workflows
- **Limited**: Less focused on agent/skill customization

---

## **🎯 How Skills Work: A Visual Guide**

### **📈 Flowchart: Skill Execution in opencode**
```
┌─────────────┐     ┌─────────────┐     ┌─────────────┐     ┌─────────────┐
│             │     │             │     │             │     │             │
│  User       │────▶│  opencode   │────▶│  Skill      │────▶│  Tools      │
│  Request    │     │  Identifies │     │  Activated  │     │  Executed   │
│             │     │  Task       │     │             │     │             │
└─────────────┘     └─────────────┘     └─────────────┘     └─────────────┘
                                                                  │
                                                                  ▼
                                                           ┌─────────────┐
                                                           │             │
                                                           │  Output     │
                                                           │  Returned   │
                                                           │             │
                                                           └─────────────┘
```

### **📈 Equivalent in Claude Code (Manual Process)**
```
┌─────────────┐     ┌─────────────┐     ┌─────────────┐     ┌─────────────┐
│             │     │             │     │             │     │             │
│  User       │────▶│  Claude     │────▶│  You        │────▶│  Claude     │
│  Request    │     │  Receives   │     │  Remind     │     │  Executes   │
│             │     │  Prompt     │     │  Context    │     │  Task       │
└─────────────┘     └─────────────┘     └─────────────┘     └─────────────┘
                         │
                         │ Must re-explain context each time!
                         ▼
              ⚠️ No persistent skill memory
```

---

## **🛠 Hands-On Example: Using the `customize-opencode` Skill**

### **📝 Step-by-Step Guide**
1. **Locate the Skill**
   - Open `AGENTS.md` in project root `./AGENTS.md`.
   - Find the `customize-opencode` skill.

2. **Invoke the Skill**
   ```bash
   skill customize-opencode
   ```

3. **Use the Skill**
   - Ask opencode to **list all agents**:
     ```text
     List all available agents in my opencode setup.
     ```

4. **Verify Output**
   - Example output:
     ```
     Available Agents:
     1. Teacher - Helps create study plans.
     2. Expert Investment - Analyzes markets.
     3. Grill Me - Stress-tests plans.
     ```

---

### **🔄 Equivalent in Claude Code**
Since Claude Code has no native skill system, you must:
```text
"Claude, I want you to act as an opencode configuration expert.
You should help me customize opencode settings.
Now list all available agents in my opencode setup."
```
⚠️ **Problem**: Must repeat context every time!

### **🔄 Equivalent in Codex**
```text
"Codex, act as opencode config expert.
Help me customize opencode.
List all available agents."
```
⚠️ **Same problem**: No persistent skill memory.

---

## **🎨 Visual Aid: Skill Workflow in Action**

### **🖼 opencode Skill Flow**
```
┌───────────────────────┐     ┌───────────────────────┐     ┌───────────────────────┐
│                       │     │                       │     │                       │
│  User Input:          │────▶│  Skill:               │────▶│  Tool: `read`         │
│  "List all agents"    │     │  `customize-opencode` │     │  Fetches agent list   │
│                       │     │                       │     │                       │
└───────────────────────┘     └───────────────────────┘     └───────────────────────┘
                                                                 │
                                                                 ▼
                                                          ┌───────────────────────┐
                                                          │                       │
                                                          │  Output:              │
                                                          │  List of agents       │
                                                          │                       │
                                                          └───────────────────────┘
```

---

## **💡 Interactive Exercise (5-10 Minutes)**

### **🔹 Exercise 1: Explore a Skill**
1. Open `AGENTS.md`.
2. Find the `teacher` skill.
3. Answer:
   - What does it do?
   - When would you use it?

### **🔹 Exercise 2: Use the `teacher` Skill**
1. Invoke the skill:
   ```bash
   skill teacher
   ```
2. Ask it to create a study plan:
   ```text
   I want to learn about advanced Claude Code prompting techniques.
   Compare your plan with what I would do in opencode using skills.
   ```
3. Observe how the skill generates a personalized plan.

### **💡 Hint**
Use `skill --help` if you're stuck.

---

## **📌 Key Takeaways**
1. **Skills automate tasks**: Save time by automating repetitive actions.
2. **Agents vs. Skills**: Agents are general-purpose; skills are task-specific.
3. **Invoke skills easily**: Use `skill <skill-name>`.
4. **Check `AGENTS.md`**: Always refer to this file for available skills.
5. **Experiment**: Try invoking skills to see their power!

### **🌐 Cross-Tool Comparison**
| Task                    | **opencode**          | **Claude Code**      | **Codex**          |
|-------------------------|----------------------|---------------------|-------------------|
| Load context            | `skill <name>`      | Manual prompt       | Manual prompt     |
| Define custom workflow | Edit `AGENTS.md`    | Create prompt file | Create prompt file|
| Reusable automation    | ✅ Native            | ❌ Not native       | ❌ Not native     |

---

## **🚀 Further Exploration**
- **Create a custom skill**: Automate a task you repeat often.
- **Explore other skills**: Try `expert-investment` or `teacher`.
- **Compare workflows**: Try the same task in opencode, Claude Code, and Codex to see differences.

---

**Reflection**: What's one task in your workflow that could be automated with a skill? Which tool (opencode, Claude Code, or Codex) do you prefer for this task? 🤔

---

## 📋 Continue Tomorrow (Quick Resume)

### 📁 Reference File
- **AGENTS.md**: `./AGENTS.md` (local in project)

### 📝 Quick Resume Notes
- **Topic**: Skills (invoking, exploring, creating)
- **Comparison**: Learned how opencode skills differ from Claude Code and Codex
- **Last Exercise**: Used `teacher` skill to create a study plan
- **Next Step**:
  1. Open `AGENTS.md` and explore other available skills (e.g., `expert-investment`)
  2. Try creating a custom skill for a task you repeat often
  3. Experiment with `skill customize-opencode` for agent configuration

### 🔑 Quick Commands
```bash
# List available skills
skill --help

# Invoke a skill
skill <skill-name>

# Open AGENTS.md (local)
open ./AGENTS.md
```

### ⏭️ Tomorrow's Goal
Learn how to **create a custom skill** and understand the skill structure in `AGENTS.md`.

---

### 🌐 Important Note for Future Lessons
> When using the **teacher** skill for new topics, always request comparisons with:
> - **Claude Code** workflows
> - **Codex** workflows
>
> This helps you understand which tool is best for different tasks!