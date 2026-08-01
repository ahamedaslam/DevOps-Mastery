# Module 01 – DevOps Fundamentals

---

# Learning Objectives

By the end of this module, I should understand:

- What DevOps is
- Why DevOps exists
- Problems before DevOps
- Benefits of DevOps
- Azure DevOps Services
- CI/CD overview

---

# Overview

Before learning DevOps in detail, let's answer four basic questions.

## What is DevOps?

DevOps is a culture and a set of practices that bring the Development and Operations teams together to automate the software delivery process.

**Simple Definition**

> DevOps = Development + Operations + Automation

It is:
- A culture
- A mindset
- A set of practices

It is **not**:
- A programming language
- A software application
- A single tool

---

## Why was DevOps introduced?

Before DevOps, developers and operations teams worked separately.

Developers focused on writing code.

Operations teams focused on deploying and maintaining the application.

This caused many communication problems, manual work, and deployment failures.

Companies introduced DevOps to improve collaboration and automate software delivery.

---

## What problems does DevOps solve?

DevOps solves many common software delivery problems, such as:

- Manual deployments
- Human errors
- Slow software releases
- Poor communication between teams
- Environment differences
- Difficult debugging
- Long release cycles
- Frequent deployment failures

---

## Where is DevOps used?

DevOps is used in almost every modern software company.

Examples include:

- Banking applications
- E-commerce websites
- Healthcare systems
- ERP applications
- Cloud-based applications
- Mobile application backends
- Microservices
- Enterprise applications

Our **AI TaskManager MultiTenant** project will also follow DevOps practices.

---

# Theory

## What is DevOps?

DevOps is a way of working where Developers and Operations teams work together to build, test, deploy, and maintain software faster and with fewer mistakes.

### Key Goals

- Faster software delivery
- Automation
- Collaboration
- Continuous feedback
- Reliability
- Better software quality

---

## Real-World Example

Imagine you are working in a company.

You develop a new feature.

Example:

**Task Reminder Feature**

You finish coding.

Now the application must be deployed so users can use it.

### Before DevOps

Developer
│
Write Code
│
Create ZIP File
│
Send ZIP to Operations Team
│
Operations Team
│
Copy Files to Server
│
Restart IIS
│
Check Logs
│
Application Available

If something goes wrong:

Developer:

> "It works on my machine."

Operations:

> "It doesn't work on the server."

Both teams start blaming each other.

### Problems

- Manual work
- Slow deployment
- Human mistakes
- Poor communication
- Difficult debugging

---

### After DevOps

Developer
│
Push Code
│
GitHub
│
Pipeline Starts
│
Build
│
Run Tests
│
Deploy Automatically
│
Users Get New Version

Nobody copies files manually.

Everything is automated.

---

## Why DevOps Exists

Traditional software delivery had several challenges:

- Manual deployments
- Human errors
- Slow releases
- Environment inconsistency
- Developer vs Operations conflicts

DevOps solves these problems through automation and collaboration.

---

## Azure DevOps Services

| Service | Purpose |
|----------|----------|
| Azure Boards | Project planning and work tracking |
| Azure Repos | Source code management using Git |
| Azure Pipelines | Build, test, and deploy applications |
| Azure Test Plans | Manual and exploratory testing |
| Azure Artifacts | Package management (NuGet, npm, Maven, etc.) |


## Popular DevOps Tools

DevOps is a culture, not a tool. Many tools help teams implement DevOps practices.

| Tool | Purpose |
|------|---------|
| Azure DevOps | Complete DevOps platform by Microsoft |
| Jenkins | CI/CD automation server |
| GitHub | Source code management and collaboration |
| GitLab | Source code management and CI/CD |
| Docker | Containerization |
| Kubernetes | Container orchestration |
| Terraform | Infrastructure as Code (IaC) |
| Ansible | Configuration management and automation |