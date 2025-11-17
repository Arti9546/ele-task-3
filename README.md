 Task 3: Basic Vulnerability Scan on Local System

## Task Objective
The objective of this task was to perform a basic **vulnerability assessment** on a local machine using a professional-grade free tool. This exercise demonstrates proficiency in identifying common security weaknesses, understanding vulnerability severity, and researching mitigation strategies.

## 🛠 Tool Used
* **Nessus Essentials:** Used to perform the credentialed vulnerability scan.

 Scan Details

| Setting | Configuration |
| :--- | :--- |
| **Tool** | Nessus Essentials (Tenable) |
| **Scan Type** | Basic Network Scan (Authenticated/Credentialed) |
| **Target** | `localhost` or Local Machine IP (`192.168.X.X`) |
| **Credentials** | Provided to Nessus to allow deep, accurate checking (e.g., checking patch levels, registry, and configuration files). |
| **Scan Duration** | [Insert your actual scan time, e.g., 45 minutes] |

## 📊 Key Findings and Analysis

The scan identified several vulnerabilities related to operating system patches, service misconfigurations, and software versions.

### Top 3 Critical Vulnerabilities Identified

(***Note:*** *Replace the placeholders below with actual, summarized findings from your Nessus scan report.*)

#### 1. Outdated Operating System Kernel / Missing Patch (Critical)
* **Vulnerability Name:** [e.g., Microsoft Windows GDI Remote Code Execution Vulnerability]
* **Nessus ID (Plugin ID):** [e.g., 160000]
* **Severity:** **Critical / High**
* **Description:** The host is missing a recent security update that patches a flaw allowing an attacker to execute arbitrary code with elevated privileges.
* **Mitigation:** Immediately install the latest cumulative security update package for the operating system.

#### 2. Unsecured FTP Service Configuration (High)
* **Vulnerability Name:** [e.g., FTP Service Allows Anonymous Login]
* **Nessus ID (Plugin ID):** [e.g., 11213]
* **Severity:** **High**
* **Description:** An FTP service was detected running with anonymous access enabled, potentially allowing unauthenticated users to read or write files to the server directory.
* **Mitigation:** Disable the anonymous FTP account or restrict access to specific authenticated users only.

#### 3. Deprecated Software Version (Medium)
* **Vulnerability Name:** [e.g., Mozilla Firefox End-of-Life Version Detection]
* **Nessus ID (Plugin ID):** [e.g., 51192]
* **Severity:** **Medium**
* **Description:** A piece of installed third-party software (e.g., a browser or media player) is running an older version known to contain multiple, documented minor security flaws.
* **Mitigation:** Update the software to the latest stable version provided by the vendor.

---

## 📸 Screenshots (Evidence)

The following screenshots confirm the completion of the task and demonstrate the results gathered by Nessus:

* * * 
---

## 🎓 Key Concepts and Learnings

* **Vulnerability vs. Exploit:** Learned that a **vulnerability** is a flaw, and an **exploit** is the tool used to take advantage of that flaw. Nessus identifies the flaws.
* **Authenticated Scan:** Using credentials provides a much **deeper and more accurate** assessment than a non-authenticated scan, as it can check internal configurations, patch levels, and registry keys.
* **Prioritization:** The severity levels (Critical, High, Medium) are crucial for prioritizing remediation efforts, focusing on the flaws that pose the most immediate risk (like Remote Code Execution).
* **Mitigation Focus:** The most common mitigation involves applying vendor-supplied **patches** or correcting **misconfigurations** of existing services.# ele-task-3
