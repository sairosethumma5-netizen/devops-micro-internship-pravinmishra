# Assignment 4 — Building Your AI Team

Part of the DevOps Micro Internship (DMI) Cohort with Agentic AI

---

## Purpose

In this assignment, you will build and configure a set of specialized AI subagents inside your project. You will learn how different models and tool permissions define agent behavior, and you will trigger two real agent delegations to analyze security and cost aspects of your Terraform infrastructure.

---

# Task 1 — Create the Agents Folder and Add Files

## Goal

Create the `.claude/agents/` directory and add all required agent files.

### Evidence

#### Screenshot 1 — VS Code sidebar showing `.claude/agents/` with all 3 files

<img width="1598" height="687" alt="WhatsApp Image 2026-10-03 at 4 00 03 PM" src="https://github.com/user-attachments/assets/e0975350-256d-4109-bb9e-8fcefa422e3b" />


---

# Task 2 — Compare the Agent Configurations

## Goal

Analyze the configuration differences between the three agents and demonstrate understanding of model and tool selection.

### Written Answers

#### 1. Why does the cost optimizer use Haiku instead of Sonnet?

The cost optimizer uses Haiku instead of Sonnet because Haiku is designed for faster and cheaper tasks while still being capable enough for routine optimization work.

💰 Lower cost — Haiku generally costs less per request than Sonnet.
⚡ Faster responses — useful when the optimizer performs many small checks.
🔧 Simple/repetitive tasks — cost optimization often involves analyzing straightforward resource or configuration data.
🧠 Sonnet is reserved for complex reasoning — tasks requiring deeper analysis can justify the higher cost.

---

#### 2. Why does the security auditor NOT have Write in its tools list?

The security auditor does not have Write in its tools list because it should be read-only.

🔍 It only needs to inspect files, configurations, and code.
🛡️ Removing Write prevents it from accidentally changing or deleting project files.
🔒 This follows the principle of least privilege: give an agent only the permissions required for its task.
✅ The auditor can report security issues and recommendations, while a developer or deployment skill can make the actual changes.

---

#### 3. Why does the tf-writer use `inherit` instead of a specific model?

The tf-writer uses inherit so it inherits the model configuration from the parent Claude Code session instead of forcing a specific model.

This is useful because:

🔄 Flexible: It automatically uses whatever model the user/session has selected.
⚙️ Consistent: The skill works with the same model configuration as the rest of the workflow.
💰 Cost control: You can change the model at the session level without modifying the skill.
🛠️ Reusable: The skill isn't tied to a particular model such as Haiku or Sonnet.

---

### Evidence

#### Screenshot 2 — `security-auditor.md` frontmatter showing model and tools configuration

<img width="1458" height="634" alt="WhatsApp Image 2026-10-03 at 4 00 10 PM" src="https://github.com/user-attachments/assets/7ffc04d5-6c9c-4d36-87a8-12e5774e792b" />


---

#### Screenshot 3 — `cost-optimizer.md` frontmatter showing the model and tools configuration

<img width="1530" height="674" alt="WhatsApp Image 2026-10-03 at 4 00 17 PM" src="https://github.com/user-attachments/assets/e5385fb6-2685-4ea9-a223-5a2396844945" />


---

# Task 3 — Run the Security Auditor

## Goal

Trigger the security auditor agent and analyze the generated security report for your Terraform infrastructure.

### Evidence

#### Screenshot 4 — The delegation message showing Claude launched the security-auditor

<img width="1600" height="611" alt="WhatsApp Image 2026-10-03 at 4 00 28 PM" src="https://github.com/user-attachments/assets/cad2d70c-621d-4a62-96a0-a5aedf3ddffa" />


---

#### Screenshot 5 — Security audit report output

<img width="1600" height="642" alt="WhatsApp Image 2026-10-03 at 4 00 28 PM (1)" src="https://github.com/user-attachments/assets/83307a2d-5796-49c4-9cdb-cab9cf55b2ad" />
.

---

# Task 4 — Run the Cost Optimizer

## Goal

Trigger the cost optimizer agent and review the generated cost optimization report.

### Evidence

#### Screenshot 6 — The full cost optimization report

<img width="1600" height="767" alt="WhatsApp Image 2026-10-03 at 4 00 28 PM (2)" src="https://github.com/user-attachments/assets/af16060b-dfce-4e39-a115-9651c5f1b350" />


---

# Task 5 — Share Your AI Team Achievement on LinkedIn

## Goal

Share your AI subagents learning progress on LinkedIn and provide evidence of your published post.

### LinkedIn Post

Use the LinkedIn post template provided in the assignment guideline.

Make sure your published post includes:

- Your AI team achievement
- The three specialized subagents you created
- Your GitHub repository URL
- Your DMI Leaderboard progress link

### Evidence

#### Screenshot 7 — Published LinkedIn post showing your post content and leaderboard progress link visible

<img width="1352" height="676" alt="image" src="https://github.com/user-attachments/assets/92d21c93-9242-4357-a41c-752030f095e4" />


---

# Submission Instructions

- Ensure all agent files are committed in `.claude/agents/`
- Complete all written answers in your GitHub Repo
- Push final changes to your forked GitHub repository

---

## GitHub Repository URL

Paste your forked repository URL here:

https://github.com/sairosethumma5-netizen/Ultimate-Agentic-DevOps-with-Claude-Code
https://github.com/sairosethumma5-netizen/devops-micro-internship-pravinmishra

---

# Completion Checklist

- [ ] `.claude/agents/` folder contains all 3 agent files
- [ ] Screenshot 2 shows correct `security-auditor.md` configuration
- [ ] Screenshot 3 shows correct `cost-optimizer.md` configuration
- [ ] All 3 written answers completed 
- [ ] Security auditor executed successfully
- [ ] Cost optimizer executed successfully
- [ ] Security report is visible with findings
- [ ] Cost report is visible with recommendations
- [ ] All required screenshots added
- [ ] GitHub repo updated with agents


---

## 📌 About DMI & CloudAdvisory

DevOps Micro Internship (DMI) is a project-based DevOps program run by Pravin Mishra (The CloudAdvisory) focused on real-world execution, systems thinking, and career readiness.

It helps learners build strong DevOps foundations with hands-on experience.

---

## 📌 Resources

- 🌐 DMI Official Website: https://dmi.pravinmishra.com?utm_source=github&utm_medium=readme  
- 🎓 University: https://university.pravinmishra.com?utm_source=github&utm_medium=readme  
- 💬 Discord Community: https://discord.pravinmishra.com?utm_source=github&utm_medium=readme  
- 📝 Blog: https://dmi.pravinmishra.com/blog?utm_source=github&utm_medium=readme  
- ▶️ YouTube Playlist: https://www.youtube.com/playlist?list=PLFeSNDtI4Cho  
- 🔗 Pravin Mishra (LinkedIn): https://www.linkedin.com/in/pravin-mishra-aws-trainer/  
- 🏢 CloudAdvisory (LinkedIn): https://www.linkedin.com/company/thecloudadvisory/

---

*This submission is part of DevOps Micro Internship (DMI) — Agentic AI Track.*
