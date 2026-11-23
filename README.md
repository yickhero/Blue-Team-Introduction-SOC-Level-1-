# Blue-Team-Introduction-SOC-Level-1-
Here is my note after finishing blue team intruduction module from tryhackme
# Junior Security Analyst Intro

## Daily Duties

1. Detect and prevent a data stealer infection on a coworker's laptop.
2. Analyze and stop a phishing campaign targeting the finance team.
3. Participate in a bigger incident, such as a full-scale ransomware attack.
4. Team up with your teammates to build detection rules and automations.
5. Go beyond cyber and understand how companies operate from the inside.

---

## SOC Roles in Blue Team

### Core Security Teams

* **Red Team:** Offensive security experts, pentesters, or ethical hackers who look for security issues.
* **GRC Team:** Specialists managing policies and ensuring compliance with regulations like PCI DSS.
* **Blue Team:** Defensive security experts like SOC analysts, engineers, or incident responders.

### Incident Response "Firefighters" (CIRT / CSIRT / CERT)

If SOC expertise is not enough or the incident goes out of control, you urgently call the "firefighters" — CIRT, also called CSIRT or CERT. Examples include:

* **JPCERT:** Japan's CERT handling nation-wide breaches.
* **Mandiant:** A private team responding to global cyber incidents.
* **AWS CIRT:** Investigates security incidents of AWS customers.

### Narrow Roles

* **Digital Forensics Analyst:** Uncover hidden threats in disk and memory.
* **Threat Intelligence Analyst:** Gather data about emerging threat groups.
* **AppSec Engineer:** Maintain a secure software development lifecycle.
* **AI Researcher:** Study AI threats and how to defend against them.

### Internal SOC vs. MSSP

| Topic | Internal SOC | MSSP |
| --- | --- | --- |
| **Scenario Example** | You work in a SOC team of the bank and protect the bank's systems. | You work for a global MSSP protecting its sixty customers in Europe. |
| **Working Pace** | You usually have calm shifts without too much time pressure. | Your shift usually starts from a queue of urgent alerts to analyze. |
| **Security Tools** | You work with just a few tools, but need to know them very well. | You have to work with sixty diverse security tools and platforms. |
| **Incident Practice** | You saw and learned from just two major cyber attacks last year. | Every week, you deal with attacks and breaches, and can learn from it. |

---

## Human as Attack Vectors

* Humans are targeted because of the access they can provide — to websites, mailboxes, or databases. Some threat actors hunt for a specific access, while others are not so selective and just breach as many accounts as they can and decide how to use them later.
* In the cyber world, humans are often these naive "gatekeepers" — the weakest link in cyber security and those who help threat actors the most.

### Social Engineering

Social engineering is designed to be:

* **Trustworthy:** The attacker must appear legitimate so the victim trusts them.
* **Emotional:** The attack must trigger feelings like urgency, fear, or curiosity.

### Defending Against Threats

Defending against threats involves two key tasks: **Mitigation** and **Detection**. Mitigation aims to prevent or reduce the chance and impact of attacks. Examples include:

* Anti-phishing solution
* Antivirus/EDR solution
* "Trust but verify" principle
* Security awareness training

---

## System as Attack Vectors

### Supply Chain Attacks

Your PC is home to hundreds of apps, including web browsers, messengers, development, and entertainment software. Every app depends on thousands of libraries. If threat actors manage to breach one of the apps or libraries and push an update to all its users, all of them will be compromised. This technique is called a **supply chain attack**. The most famous examples are the **SolarWinds** and **3CX** breaches, which affected thousands of companies.

### Vulnerabilities, CVEs, and Patching

* Once a vulnerability is made public, it is assigned a **Common Vulnerabilities and Exposures (CVE)** number. From that moment, it's a race: attackers develop exploits while defenders rush to update their systems.
* An answer to a CVE is always a **patch** — an update supplied by the software vendor. Even for zero-days, you'll have to wait for a patch, vigilantly monitor for exploitation traces, and try to survive the stressful period before the patch is released. For example, by:
1. Restricting access to the system to only trusted IPs.
2. Applying temporary measures provided by the vendor.
3. Blocking known attack patterns on IPS or WAF.



### Misconfigurations

A **misconfiguration** isn't a bug in the software, but a mistake in how the system was set up, often by the IT team.
