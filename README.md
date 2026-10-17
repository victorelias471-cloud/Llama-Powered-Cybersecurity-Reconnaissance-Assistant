# Llama-Powered Cybersecurity Reconnaissance Assistant

## 📌 Overview
The **Llama-Powered Cybersecurity Reconnaissance Assistant** is a conceptual framework and prototype design for automated network reconnaissance and vulnerability evaluation. Built for early-stage startups, developers, and small organizations, this project bridges the gap between complex command-line security tools and actionable security insights.

By combining open-source network scanning utilities with Meta's **Llama** model family (via Llama Stack), the assistant converts raw terminal log outputs into structured, plain-language executive summaries and risk evaluations.

---

## 🎯 Problem Statement
Small businesses and entry-level security teams often lack the technical expertise or bandwidth to regularly map their attack surfaces. Standard tools produce dense, technical text files that require expert interpretation, leaving organizations exposed to unpatched vulnerabilities and configuration risks.

---

## 🏗 System Architecture & Workflow
1. **Target Input:** User specifies a target domain or IP address within authorized boundaries.
2. **Reconnaissance Execution:** Automated scripts execute lightweight, non-intrusive scans using:
   - **Nmap:** Port discovery and service identification
   - **WHOIS & DNSRecon:** Domain registration and DNS mapping
   - **WhatWeb & cURL:** Web server headers and technology stack detection
   - **Wafw0of:** Web Application Firewall (WAF) detection
3. **Log Processing & LLM Pipeline:** Raw log outputs are formatted and piped into a Llama model.
4. **Insight Generation:** The model returns a human-readable security report highlighting potential exposure points, severities, and suggested mitigation steps.

---

## 🛡 Safety, Guardrails & Boundaries
- **No Exploitation:** The tool strictly performs passive/light active reconnaissance and does **not** execute offensive exploits or automated penetration testing.
- **Human-in-the-Loop:** AI model outputs are treated as preliminary advisories. All security findings must be verified by a qualified analyst before taking remediation actions.
- **Safety Guardrails:** Utilizes **Llama Guard** parameters to enforce strict input/output boundaries and prevent misuse.

---

## 📚 Module Alignment (3MTT × Meta AI Program)
- **Module 2 (Llama Models, Architecture & Tool Calling):** Grounded the technical approach to function calling, orchestrating Llama Stack, and implementing model safety checks.
- **Module 4 (Startup-in-a-Box & Prototyping):** Focused the scope on delivering a clear Minimal Viable Product (MVP) aimed at solving a single high-value security problem.

---

## 📄 License
This repository is shared for educational and portfolio demonstration purposes under the MIT License.