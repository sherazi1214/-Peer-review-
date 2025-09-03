# Peer Review Process
### 1. Initial Testing & Documentation

**English:** The first pentester performs testing, collects results, and documents all findings in detail.

**Urdu:** Pehle tester test karta hai aur sari vulnerabilities, evidence aur notes record karta hai taa ke clear documentation ready ho.

### 2. Secondary Review by Another Pentester

**English:** A second penetration tester reviews the initial findings to verify accuracy and check if anything was missed.

**Urdu:** Doosra tester review karta hai taa ke ensure ho ke pehle wale tester ki findings sahi hain aur koi cheez chhuti nahi.

### 3. Cross Verification with Industry Standards

**English:** Findings are compared with known frameworks and standards like OWASP, NIST, or MITRE ATT&CK to validate severity and accuracy.

**Urdu:** Phir vulnerabilities ko industry standards aur frameworks se compare kiya jata hai taa ke severity aur impact ko confirm kiya ja sake.

### 4. Feedback & Improvements

**English:** Reviewers provide feedback for corrections, better documentation, or additional testing if required.

**Urdu:** Reviewer feedback deta hai ke documentation aur testing me kahan improvements ho sakti hain, aur agar zaroori ho to retesting bhi hoti hai.

### 5. Final Validation before Reporting

**English:** Before the official report is delivered to the client, a final check is done to validate all findings, severity ratings, and recommendations.
**Urdu:** Report client ko dene se pehle ek final validation hoti hai taa ke koi galti na rahe aur severity rating sahi ho.

### Tools Used in Peer Review

**Burp Suite Collaborator** → Test web vulnerabilities aur confirm interactions (Roman Urdu: web app flaws verify karne ke liye).

**Nmap & Nessus Reports** → Compare scan results for accuracy (Roman Urdu: network scanning aur vulnerability scanning ka cross-check).

**MITRE ATT&CK Navigator** → Map findings with attacker techniques (Roman Urdu: attack techniques ke sath findings match karna).

**CVSS Calculator** → Standard method to calculate severity score (Roman Urdu: vulnerability ki severity aur impact ko number me score karna).

# Stakeholder Alignment

**English:** Stakeholder alignment means ensuring that all important parties (C-level, security teams, IT teams, legal & compliance) are on the same page regarding penetration testing goals, scope, and reporting.

**Urdu:** Stakeholder alignment ka matlab hai ke sab important log ek hi page pe ho — yani testing ke goals, scope aur reporting sab ko clear samajh aaye.

## Stakeholder Groups

**C-Level Executives** → Focus on business risk, cost, ROI.

**Urdu:** Ye log technical details nahi chahte, unko business impact aur paisay ka risk samajhna hota hai.

**Security Teams** → Focus on vulnerabilities, threats, defenses.

**Urdu:** Security teams detail me findings aur fixes dekhti hain.

**IT Teams** → Focus on systems, configurations, patching.
**Urdu:** IT teams ko batana padta hai ke kaunse systems aur configs vulnerable hain aur kaise fix karna hai.

**Legal & Compliance** → Focus on laws, policies, regulations.
**Urdu:** Legal aur compliance check karte hain ke testing aur findings regulations (GDPR, HIPAA, PCI-DSS) ke mutabiq hain ya nahi.

## How to Align with Stakeholders

Define Testing Goals Clearly

**English:** Set clear objectives (e.g., test web apps, check compliance, identify risks).

**Urdu:** Pehle hi clear goals set karna zaroori hai taa ke sab ko pata ho testing ka purpose kya hai.

### Set Expectations on Scope & Reporting

**English:** Explain what is in-scope vs out-of-scope, and what type of reporting they will receive.

 **Urdu:** Batao ke kaunsa area test hoga aur kaunsa nahi, aur report ka format kaisa hoga.

### Communicate Regularly During Engagement

**English:** Share updates, findings, and issues as testing continues.

**Urdu:** Engagement ke dauran regular communication rakho taa ke surprises na ho.

### Key Communication Strategies

#### Technical vs Non-Technical Language

**English:** Adapt communication — technical detail for security/IT teams, simplified business risk language for executives.

**Urdu:** Audience ke hisaab se language use karo — C-level ko simple risk terms me samjhao, IT ko technical details do.

### Live Demonstrations

**English:** Show real-time exploit or PoC (proof of concept) to make impact clear.

**Urdu:** Kabhi-kabhi live demo dikhana acha hota hai taa ke stakeholders risk ko practically samajh saken.

### Clear Reporting Formats

**English:** Use structured, easy-to-read reports with executive summary + technical detail.

**Urdu:** Report simple aur structured honi chahiye — ek section C-level ke liye, ek detail section IT/security ke liye.

### Easy Exam Recall:

**Who? C-level | Security | IT | Legal/Compliance**

How? Goals → Scope/reporting expectations → Regular communication

Keys? Right language | Live demo | Clear reporting


# Root Cause Analysis (RCA) Process
### 1. Identify the Vulnerability

**English:** Detect the weakness in the system, application, or process.
**Urdu:** Pehla step hai vulnerability ko identify karna — jaise weak password policy ya insecure input field.

### 2. Analyze the Exploitability

**English:** Check how easily the vulnerability can be exploited by an attacker.
**Urdu:** Phir dekhte hain ke attacker kitni asaani se exploit kar sakta hai aur uska potential impact kya hoga.

### 3. Trace the Root Cause

**English:** Find the underlying reason for the vulnerability — whether it’s poor coding, misconfiguration, or weak controls.
**Urdu:** Vulnerability ke asal source ko trace karna zaroori hai, taa ke samajh aaye ye issue kyon aaya (e.g., coding error, policy gap, config mistake).

### 4. Recommend Permanent Fixes

**English:** Suggest long-term solutions to eliminate the root cause and prevent recurrence.
**Urdu:** Last step hai permanent fixes recommend karna taa ke issue dobara na aaye (patching, policy update, training, automation).

## Common Root Causes of Security Flaws
### Root Cause-------------------	Example Vulnerability----------------------------------	Mitigation

Weak Authentication-------	Easy-to-guess passwords, no MFA	----Enforce strong password policies, enable MFA

Lack of Input Validation------	SQL Injection, Cross-Site Scripting (XSS)-----	Implement input sanitization & validation rules

Insecure API Exposure-------	Unauthorized API calls, data leakage--------	Use authentication, rate limiting, secure coding

Misconfigured Security Settings-----	Open ports, overly permissive S3 buckets------	Regular configuration audits, least privilege

## Roman Urdu Explanation:

**Weak Authentication:** Password policy ya MFA na hone ki wajah se system easy hack ho jata hai.

**Lack of Input Validation:** Agar input properly filter nahi hota to attacker malicious code inject kar sakta hai.

**Insecure API Exposure:** APIs agar authentication ke baghair exposed hain to sensitive data leak ho sakta hai.

**Misconfigured Security:** Wrong settings (open ports, wrong permissions) system compromise kar dete hain.

#### Easy Exam Recall Line:

**RCA steps** = Identify → Analyze → Trace → Fix

**Root Causes** = Weak Auth | No Input Validation | Insecure API | Misconfig
