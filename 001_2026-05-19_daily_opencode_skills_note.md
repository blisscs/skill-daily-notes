# 🚀 Daily Study Note: Mastering opencode Skills with Visuals

---

## **📌 Introduction: Why Skills Matter**
Imagine you're working in opencode and find yourself repeating the same tasks:
- Searching for files.
- Editing configurations.
- Running commands.

**Skills are your superpower!** They automate these tasks so you can focus on what matters.

Today, you’ll learn:
✅ What skills are and how they work.
✅ How to **invoke and use** skills in your workflow.
✅ How to **explore and experiment** with skills hands-on.

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

## **🎯 How Skills Work: A Visual Guide**

### **📈 Flowchart: Skill Execution**
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

---

## **🛠 Hands-On Example: Using the `customize-opencode` Skill**

### **📝 Step-by-Step Guide**
1. **Locate the Skill**
   - Open `AGENTS.md` in `~/.config/opencode/`.
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

## **🎨 Visual Aid: Skill Workflow in Action**

### **🖼 Example: `customize-opencode` Skill**
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
2. Find the `grill-me` skill.
3. Answer:
   - What does it do?
   - When would you use it?

### **🔹 Exercise 2: Use the `grill-me` Skill**
1. Invoke the skill:
   ```bash
   skill grill-me
   ```
2. Ask it to stress-test a plan:
   ```text
   I want to build a Python script to organize files. Grill me!
   ```
3. Observe how it challenges your plan.

### **💡 Hint**
Use `skill --help` if you’re stuck.

---

## **📌 Key Takeaways**
1. **Skills automate tasks**: Save time by automating repetitive actions.
2. **Agents vs. Skills**: Agents are general-purpose; skills are task-specific.
3. **Invoke skills easily**: Use `skill <skill-name>`.
4. **Check `AGENTS.md`**: Always refer to this file for available skills.
5. **Experiment**: Try invoking skills to see their power!

---

## **🚀 Further Exploration**
- **Create a custom skill**: Automate a task you repeat often.
- **Explore other skills**: Try `expert-investment` or `teacher`.
- **Read the docs**: Visit opencode’s documentation for more examples.

---
**Reflection**: What’s one task in your workflow that could be automated with a skill? 🤔
---

## 📋 Continue Tomorrow (Quick Resume)

### 📁 Reference File
- **AGENTS.md**: `~/.config/opencode/AGENTS.md`

### 📝 Quick Resume Notes
- **Topic**: Skills (invoking, exploring, creating)
- **Last Exercise**: Used `grill-me` skill to stress-test a plan
- **Next Step**: 
  1. Open `AGENTS.md` and explore other available skills (e.g., `expert-investment`, `teacher`)
  2. Try creating a custom skill for a task you repeat often
  3. Experiment with `skill customize-opencode` for agent configuration

### 🔑 Quick Commands
```bash
# List available skills
skill --help

# Invoke a skill
skill <skill-name>

# Open AGENTS.md
open ~/.config/opencode/AGENTS.md
```

### ⏭️ Tomorrow's Goal
Learn how to **create a custom skill** and understand the skill structure in `AGENTS.md`.
