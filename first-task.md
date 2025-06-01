Scalable Error Logging Service - Full-Stack JS Solution

### **Task: Describe the Architecture of an Error Logging Service**

**Overview**

You need to prepare a document describing how you would design an error logging service from scratch. Explain which technologies you would choose for the client library (SDK), backend API, database, web dashboard, and DevOps solution, and justify why these choices are optimal. Additionally, compile a list of questions you would ask the client to better understand the project requirements and expectations.

### **Functional Requirements:**

1. **Client SDK** that developers integrate into their applications to capture and send error logs.
2. **API Backend** that receives, processes, and stores logs from client applications.
3. **Web Dashboard** for developers to view, search, and analyze logged errors.
4. **Real-time Alerts** via email notifications on critical errors.
5. **DevOps solution** for scalable deployment, monitoring, and log storage optimization.

### **Additional Task: Developer Questions for the Platform Owner**

As a developer, formulate key questions for the platform owner to clarify requirements and expectations.

### **What You Need to Do:**

- **Describe the application architecture** (SDK, Backend, Database, Web (React) Dashboard, DevOps).
- **Justify your choice of technologies** (why they are suitable for this project).
- **Explain key decisions** (real-time processing, log retention policies, API rate limits, security, DevOps processes).
- **Formulate relevant questions** from a developer's perspective to better understand the project requirements.

====================== SOLUTION =========================

1. Client SDK

I'll use:
JS/TS and Distribute as NPM package.
Purpose:
Capture Frontend (React) and backend (Node.js) errors
Sending logs with context about logs, etc user info, timestamp, environment, stack trace

TypeScript will help with scalable because it gives us safety and IDE support.
It must be small bundle size and async logging
Easy for install for example @error/logger

2. API Backend

Web Framework - Node.js + Express. Because it have high performance and widely using in full-stack JS apps

Realtime Alerts - [Socket.io](https://socket.io/) and we
