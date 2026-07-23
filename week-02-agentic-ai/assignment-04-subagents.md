# Assignment 4 — Building Your AI Team

Part of the DevOps Micro Internship (DMI) Cohort 3 with Agentic AI

---

## Purpose

In this assignment, you will build and configure a set of specialized AI subagents inside your project. You will learn how different models and tool permissions define agent behavior, and you will trigger two real agent delegations to analyze security and cost aspects of your Terraform infrastructure.

---

# Task 1 — Create the Agents Folder and Add Files

## Goal

Create the `.claude/agents/` directory and add all required agent files.

### Evidence

#### Screenshot 1 — VS Code sidebar showing `.claude/agents/` with all 3 files

![alt text](assignment-briefs/Q4_screenshot_1.jpg).

---

# Task 2 — Compare the Agent Configurations

## Goal

Analyze the configuration differences between the three agents and demonstrate understanding of model and tool selection.

### Written Answers

#### 1. Why does the cost optimizer use Haiku instead of Sonnet?

A cost optimizer uses Claude Haiku instead of Sonnet primarily because it is designed for maximum efficiency in mechanical, well-defined tasks. 
A cost optimizer defaults to Haiku rather than Sonnet for specific reasons: 
•	Drastically Lower Pricing: 
•	Optimized for Simpler Tasks. 
•	Speed and Throughput: 


---

#### 2. Why does the security auditor NOT have Write in its tools list?

- Why does the security auditor NOT have Write in its tools list?

Security auditors lack "Write" capabilities to maintain strict impartiality, data integrity, and compliance. This limitation is by design to ensure they cannot alter system files or logs, preventing conflicts of interest and guaranteeing that their audit trails remain verifiable, tamper-proof, and completely objective.

---

#### 3. Why does the tf-writer use `inherit` instead of a specific model?

- Why does the tf-writer use `inherit` instead of a specific model?

   The tf-writer (or similar logging agents) uses inherit instead of a specific model to decouple the agent's behavior from any single architecture. This allows it to adapt dynamically to whichever model or pipeline is passed to it, making the code more flexible, modular, and easier to scale.

---

### Evidence

#### Screenshot 2 — `security-auditor.md` frontmatter showing model and tools configuration

![alt text](assignment-briefs/Question4_screenshot_2.jpg).

---

#### Screenshot 3 — `cost-optimizer.md` frontmatter showing the model and tools configuration

![alt text](assignment-briefs/Question4_screenshot_3.jpg).

---

# Task 3 — Run the Security Auditor

## Goal

Trigger the security auditor agent and analyze the generated security report for your Terraform infrastructure.

### Evidence

#### Screenshot 4 — The delegation message showing Claude launched the security-auditor

![alt text](assignment-briefs/Q4_subagents_screenshot_4.jpg).

---

#### Screenshot 5 — Security audit report output

![alt text](assignment-briefs/Q4_subagents_screenshot_5.jpg).

---

# Task 4 — Run the Cost Optimizer

## Goal

Trigger the cost optimizer agent and review the generated cost optimization report.

### Evidence

#### Screenshot 6 — The full cost optimization report

![alt text](assignment-briefs/Question4_screenshot_6.jpg).

---

# Submission Instructions

- Ensure all agent files are committed in `.claude/agents/`
- Complete all written answers in your GitHub Repo
- Push final changes to your forked GitHub repository

---

## GitHub Repository URL

Paste your forked repository URL here:

`https://github.com/richmondusoh/Ultimate-Agentic-DevOps-with-Claude-Code.git`

---

# Completion Checklist

- [✅] `.claude/agents/` folder contains all 3 agent files
- [✅] Screenshot 2 shows correct `security-auditor.md` configuration
- [✅] Screenshot 3 shows correct `cost-optimizer.md` configuration
- [✅] All 3 written answers completed 
- [✅] Security auditor executed successfully
- [✅] Cost optimizer executed successfully
- [✅] Security report is visible with findings
- [✅] Cost report is visible with recommendations
- [✅] All required screenshots added
- [✅] GitHub repo updated with agents

---

## 📌 About DMI & CloudAdvisory

DevOps Micro Internship (DMI) is a project-based DevOps program run by Pravin Mishra (The CloudAdvisory) focused on real-world execution, systems thinking, and career readiness.

It helps learners build strong DevOps foundations with hands-on experience.

---

## 📌 Resources

- 🌐 DMI Official Website: https://pravinmishra.com/dmi  
- 🎓 DevOps for Beginners (Udemy): https://www.udemy.com/course/devops-for-beginners-docker-k8s-cloud-cicd-4-projects/  
- 🎓 Agentic AI DevOps with Claude Code: https://www.udemy.com/course/ultimate-agentic-ai-devops-with-claude-code/  
- 🎓 DevOps with Claude Code: Terraform, EKS, ArgoCD & Helm: https://www.udemy.com/course/devops-with-claude-code-terraform-eks-argocd-helm/  
- ▶️ YouTube Playlist: https://www.youtube.com/playlist?list=PLFeSNDtI4Cho  
- 🔗 Pravin Mishra (LinkedIn): https://www.linkedin.com/in/pravin-mishra-aws-trainer/  
- 🏢 CloudAdvisory (LinkedIn): https://www.linkedin.com/company/thecloudadvisory/

---

*This submission is part of DevOps Micro Internship (DMI) Cohort 3 — Agentic AI Track.*