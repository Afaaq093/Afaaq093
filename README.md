# Afaaq Yaseen

**Offensive Security · Web Application VAPT · Bug Bounty · Red Team**

[LinkedIn](https://www.linkedin.com/in/afaaq-yaseen-23b40a342) · [Medium](https://medium.com/@afaaqyaseen) · [HackerOne](https://hackerone.com/YOUR-H1-USERNAME) · [bugbountyhunter121@gmail.com](mailto:bugbountyhunter121@gmail.com)

---

## Operator Profile

| | |
|---|---|
| **Role** | Penetration Tester Intern, Tech Biz Security |
| **Focus** | Web application VAPT, red teaming, bug bounty |
| **Education** | BSc Computer Science (2026) |
| **Certifications** | CEH · CHFI (training completed) · CPTS (in progress) |
| **Location** | Rawalpindi, Pakistan |
| **Availability** | Open to VAPT and red team roles |

---

## Attacker Mindset

Applications are built on assumptions. My job is to find the ones that break.

```diff
- Assumption: "Users can only access their own records."
+ Test: replay requests across two accounts, swap object IDs, change roles.

- Assumption: "The input filter blocks script injection."
+ Test: context-specific payloads for HTML, attributes, JS, and DOM sinks.

- Assumption: "This endpoint is internal, so it's safe."
+ Test: steer server-side requests toward internal resources (SSRF).

- Assumption: "Error messages help developers, not attackers."
+ Test: trigger errors, collect stack traces, paths, tokens, and metadata.
```

A single low-severity finding is rarely the end. I look at how findings **chain** into real impact:

```
Information disclosure  →  leaked ID format / internal path
        ↓
IDOR                    →  enumerate other users' objects
        ↓
Impact                  →  unauthorized access to sensitive data
```

*(Illustrative example of how I reason about chaining, not a specific engagement.)*

---

## Engagement Approach

| Phase | Objective |
|---|---|
| **1. Recon** | Map the attack surface: subdomains, endpoints, parameters, tech stack, exposed assets |
| **2. Enumeration** | Understand authentication, roles, object references, and trust boundaries |
| **3. Exploitation** | Validate each weakness with a minimal, safe proof of concept |
| **4. Impact analysis** | Demonstrate what an attacker actually gains, in business terms |
| **5. Reporting** | Reproducible steps, severity rationale, and fix guidance developers can act on |

---

## Vulnerability Coverage

`XSS` · `SQL Injection` · `IDOR / Broken Access Control` · `CSRF` · `SSRF` · `XXE` · `Information Disclosure` · `Clickjacking`

---

## Report Standard

Every finding I write follows this structure:

```
Title:         Short, specific, impact-focused
Severity:      Critical / High / Medium / Low, with rationale
Affected:      URL / endpoint / parameter
Description:   What the weakness is and why it exists
Reproduction:  Numbered steps with request/response evidence
Impact:        What an attacker can achieve
Remediation:   Concrete fix, not generic advice
```

---

## Bug Bounty

```
Platforms   HackerOne · OpenBugBounty
Reported    XSS · IDOR · Information Disclosure
Standard    PoC + impact analysis + remediation in every report
Ethics      Responsible disclosure, in-scope testing only
```

---

## Toolkit

`Burp Suite` · `Nmap` · `ffuf` · `sqlmap` · `Nuclei` · `Wireshark` · `Kali Linux` · `Python` · `Git`

---

## Projects

| Project | Description | Status |
|---|---|---|
| `aws-vuln-scanner` | AWS security misconfiguration scanner | Uploading soon |
| `port-scanner` | Port and service detection utility | Uploading soon |
| `ai-vuln-scanner` | AI-assisted vulnerability scanner | In development |

---

## Writeups

Lab and machine writeups covering methodology, exploitation, and remediation: **uploading soon.**

Articles: [medium.com/@afaaqyaseen](https://medium.com/@afaaqyaseen)

---

## Training

PortSwigger Web Security Academy · Hack The Box · TryHackMe · CTFtime

---

<sub>All testing is performed on authorized targets only. No client data or confidential findings are published here.</sub>
