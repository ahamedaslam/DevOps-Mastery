# Module 01 – Best Practices

---

## Best Practices

### 1. Always Automate Repetitive Tasks

If a task is performed repeatedly, try to automate it instead of doing it manually.

**Example:**

Instead of manually building and deploying the application every time, use a CI/CD pipeline.

---

### 2. Work as One Team

Developers and Operations engineers should work together instead of working separately.

Good communication helps reduce deployment issues.

---

### 3. Use Version Control

Always store your source code in a version control system like Git.

Benefits:

- Track changes
- Restore previous versions
- Work with multiple developers
- Review code changes

---

### 4. Test Before Deployment

Always run automated tests before deploying an application.

This helps detect issues early.

---

### 5. Deploy Small Changes Frequently

Instead of releasing a huge update after several months, release smaller updates more often.

Benefits:

- Easier debugging
- Faster feedback
- Lower deployment risk

---

### 6. Monitor Applications After Deployment

Deployment is not the end.

Always monitor:

- Application health
- Performance
- Errors
- Logs

This helps identify and fix issues quickly.

---

### 7. Learn from Failures

Every deployment failure is an opportunity to improve.

Analyze the root cause and update the process to prevent the same issue in the future.

---

## Best Practices for Our Project

For our **AI TaskManager MultiTenant** project, we will follow these practices:

✔ Store source code in GitHub

✔ Build the application automatically

✔ Run unit tests before deployment

✔ Use Docker for consistency

✔ Automate deployment using CI/CD

✔ Monitor the application after deployment