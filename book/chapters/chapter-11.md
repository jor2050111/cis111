# Chapter 11: Cybersecurity Risk, Identity Theft, and Incident Response

A help desk gets three calls about locked accounts. A finance worker sees
a payment that no one approved. A server begins sending data to an
unknown site. Each clue may be one part of the same attack.

A sound response does more than stop a bad file. The team must protect
people, keep proof, restore service, meet notice duties, and learn why the
controls failed. This chapter gives you records and tests for that work.

## Module Overview 🧭

* **Estimated time:** 5-6 hours (reading + practice + Skills Lab)
* **Prerequisites:** Chapters 1-10
* **Deliverables:** Try It Yourself activities, Quick Checks, Skills Lab 11A

## Learning Objectives 🎯

By the end of this chapter, you will be able to:

* **MLO-11.1 (Analyze):** Analyze identity theft and security incidents through asset, threat, weakness, harm, and proof records
* **MLO-11.2 (Evaluate):** Evaluate cyber risk and response choices with the CIA Security Triad and NIST CSF 2.0
* **MLO-11.3 (Create):** Create a security policy and incident plan with roles, controls, evidence, notice, and recovery tests

### This chapter aligns with the following Course Learning Outcomes

* **CLO XIV.** Analyze the major identity theft issues.
* **CLO XV.** Evaluate Information Technology security breaches and risk assessments.
* **CLO XVI.** Formulate security policies within Information Technology.
* **CLO XVIII.** Develop prevention, detection, and responses to Information Technology security attacks.

---

## 11.1 Map the Asset, Event, and CIA Harm

Security starts with what must stay safe and useful. A control has no
clear value until the team names the asset and harm.

The **CIA Security Triad** groups three core goals:

* **Confidentiality:** Data is seen only by people and systems with the right to see it.
* **Integrity:** Data and systems stay correct, complete, and free from unapproved change.
* **Availability:** Approved users can reach the data and service when they need it.

One event can harm all three. Ransomware may copy files first, change
them, and then lock the system. The copy harms confidentiality. The
change harms integrity. The lock harms availability.

Do not frame each control as a trade against another goal. MFA can guard
confidentiality and integrity with little effect on access when recovery
is well designed. Backups can help integrity and availability. The team
should test all three goals and the people who rely on them.

### Separate Threat, Weakness, and Exploit

A **threat** is a source or event that may cause harm. A storm, thief,
careless change, bad update, or failed disk can be a threat.

A **vulnerability** is a weakness that a threat can use. An old server,
shared account, open storage bucket, weak process, or missing backup can
be a weakness.

An **exploit** is a method or code that uses a weakness. An **incident**
is an event that puts security at risk or breaks a security rule.

This order matters. "Phishing is the risk" is too broad. A better record
may say:

* Threat event: a false help-desk message asks for a password
* Weakness: the account has no MFA and the sign-in page has no warning
* Exploit path: the attacker uses the stolen password from a new device
* Harm: the attacker reads student aid files and sends more false mail

The team can now choose controls at more than one point.

### Use a Seven-Line Incident Map

1. **Asset and owner:** Name the data, device, service, or process at risk.
2. **Event:** State what happened or may happen.
3. **Threat source:** Name the person, process, fault, or event that may cause harm.
4. **Weakness and path:** Show how the event reaches the asset.
5. **CIA harm:** Mark confidentiality, integrity, and availability effects.
6. **People and mission:** Name who is harmed and which work may stop.
7. **Proof and control:** List the logs, alerts, files, people, and controls needed.

The map can hold an open question. Write "unknown" when the proof does
not support a claim. Do not turn a guess into an attack story.

### Match Controls to the Attack Path

Common controls work at different points:

| Attack path | Prevent or limit | Detect | Recover |
| --- | --- | --- | --- |
| Stolen password | MFA, password manager, least privilege | New-device and risky sign-in alerts | Reset sessions and review account use |
| Harmful file | Safe mail controls, app limits, staff practice | Endpoint and mail alerts | Isolate host and restore a known-good copy |
| Unpatched flaw | Asset list, patch process, network limit | Scan and exploit alerts | Fix, test, and watch for return |
| Ransomware | MFA, segmenting, allow lists, offline backup | File-change and command alerts | Contain, rebuild, restore, and verify |
| Service flood | Capacity, rate limits, service design | Traffic and service-health alerts | Filter traffic and shift service |

No control makes risk zero. A strong plan uses layers so one miss does
not end the defense.

**Worked incident map:** A small clinic cannot open its schedule. A note
on one server asks for payment. The firewall shows a large upload the
night before. A backup job failed for six days.

The schedule, patient data, server, and backup are separate assets. The
event may involve data theft and ransomware. The upload is proof of
traffic, not proof of which files left. The failed backup raises the
recovery harm.

The team should isolate systems under its plan, preserve the right logs,
set an incident lead, and check the scope. It should not promise that no
data left or that the backup will work until tests support those claims.

### Try It Yourself 11.1: Map a Shared Account 🛠️

**Predict:** Five staff members share one admin account. A setting is
changed, but no one admits doing it. Which CIA goal faces the most harm?

**Run:** Complete all seven lines of the incident map. Add least-
privilege, named-account, log, MFA, and recovery controls.

**Explain:** In 1-2 sentences, name the first control to change and the
proof it would add.

### Quick Check 11.1 ✅

1. Define confidentiality, integrity, and availability. *(Understand)*

2. Distinguish a threat, vulnerability, exploit, and incident. *(Apply)*

3. How can one ransomware event harm all three CIA goals? *(Analyze)*

---

## 11.2 Trace Identity Theft and Lawful Access

**Identity theft** occurs when someone uses another person's data
without permission to commit fraud or gain a benefit. The harm can reach
money, health records, taxes, work, housing, or a person's legal record.

**Personally identifiable information (PII)** is data that can identify
or be linked to a person. A name alone may pose little risk. A name with
a birth date, Social Security number, account, and password can support
far more harm.

### Link the Data to the Misuse

Common forms include:

* **Financial identity theft:** The thief opens an account, takes a loan, or spends from an account.
* **Tax identity theft:** The thief files a false return or claim with another person's data.
* **Medical identity theft:** The thief gets care, drugs, or benefits under another person's name.
* **Criminal identity theft:** The thief gives another person's identity to police or a court.
* **Synthetic identity theft:** The thief joins real and false data to form a new identity.
* **Child identity theft:** The thief uses a child's data, which may go unchecked for years.

Do not write "PII was exposed" and stop. Ask which fields were involved,
whether they were plain or protected, who gained access, and what misuse
those fields can support.

Use a six-line identity harm map:

1. **Data:** List each field, account, document, or token involved.
2. **Access:** State who may have obtained it and how.
3. **Misuse:** Link the data to a plausible form of fraud or harm.
4. **Warning sign:** Name what the person or firm should watch for.
5. **Containment:** Stop more access, use, or spread.
6. **Recovery:** Name the report, freeze, dispute, record fix, or support step.

The FTC's [IdentityTheft.gov recovery tool](https://www.identitytheft.gov/steps)
creates a report and a plan based on the person's case. A fraud alert and
a credit freeze are not the same. The right step depends on the harm.

### Build Prevention at Two Levels

People can use unique passwords, a password manager, MFA, account alerts,
credit reports, and credit freezes. They can also verify a request
through a known contact path.

Firms control much of the risk. They can:

* Collect less data and erase it when the purpose ends
* Use MFA and least privilege
* Encrypt data in storage and transit
* Split high-risk duties and log access
* Patch systems and test backups
* Give people a fast way to report a false message
* Plan notices and support before an incident

Training alone is not a full control. A well-made false page can fool a
careful person. The system should limit what one stolen password can do.

### Read the CFAA after Van Buren

The **Computer Fraud and Abuse Act (CFAA)** is a federal computer crime
law. It covers several acts involving protected computers, such as some
forms of access without authorization, fraud, damage, and password
traffic. Each charge has its own elements.

In *Van Buren v. United States*, the Supreme Court held that a person
does not "exceed authorized access" merely by getting data that the
person could access for an improper purpose. The clause reaches data in
parts of a computer that are off limits to that person.

The DOJ's current
[CFAA charging policy](https://www.justice.gov/archives/opa/pr/department-justice-announces-new-policy-charging-cases-under-computer-fraud-and-abuse-act)
also states that a terms-of-service breach alone should not support a
federal criminal charge. It directs prosecutors not to charge good-faith
security research as defined in the policy.

That policy is not a broad right to test any system. Scope, consent,
method, harm, notice, and other laws still matter. A researcher should
use a written vulnerability disclosure or safe-harbor rule when one is
available.

Other laws may apply to identity fraud, wire or stored messages, access
devices, and notice after a breach. Do not use "cybercrime law" as one
label. Name the act and the facts.

**Worked identity harm map:** A school learns that a staff mailbox was
open to an attacker for three days. The mail held tax forms, health notes,
and student aid files. The team does not know which messages were read.

The data can support tax, medical, financial, and child identity harm.
The access log, mail rules, downloads, forwarded mail, and sign-in tokens
may help set scope. Lack of a download log does not prove that no one
read a message.

The school should stop the account use, preserve logs, apply its notice
map, and give each affected person steps tied to the data. A broad offer
of credit checks may not fix a false medical record or tax filing.

### Try It Yourself 11.2: Trace a Stolen Student File 🛠️

**Predict:** A stolen file holds names, birth dates, and student ID
numbers, but no Social Security numbers. Does that remove identity risk?

**Run:** Complete the six-line identity harm map. Separate known access
from possible misuse.

**Explain:** In 1-2 sentences, name the best support step and the missing
fact that could change it.

### Quick Check 11.2 ✅

1. Name three forms of identity theft and the data each may use. *(Understand)*

2. How did *Van Buren* limit the CFAA access rule? *(Apply)*

3. Why is security training weak when one stolen password can reach all records? *(Analyze)*

---

## 11.3 Rank Risk and Write Enforceable Policy

A **risk assessment** helps a team choose where to spend time and money.
It does not predict the future with a perfect score.

NIST risk guidance examines threats, weak points, likelihood, and impact.
The team should also record uncertainty. A "high" rating with poor proof
may need more study before a costly choice.

### Build a Nine-Column Risk Register

| Field | Question |
| --- | --- |
| Asset and owner | What must be protected, and who answers for it? |
| Threat event | What could happen? |
| Weakness and path | How could the event reach the asset? |
| Current controls | What now prevents, detects, or limits it? |
| Likelihood | How likely is the event under stated facts? |
| Impact | What harm could reach people, work, money, law, or trust? |
| Proof and uncertainty | Which facts support the rating, and what is unknown? |
| Response and owner | Will the team reduce, share, avoid, or accept the risk? Who acts? |
| Due point and residual risk | When will the action occur, and what risk remains? |

Some teams use numbers. Others use low, medium, and high bands. Either
method needs a clear scale. "Risk equals likelihood times impact" is a
useful shorthand, not a full or universal method.

A team may:

* **Reduce** risk with a control
* **Share** part of the risk through a contract or insurance
* **Avoid** the act that creates the risk
* **Accept** the risk with named authority and review

Insurance does not move all harm. It may pay some costs, but people can
still lose access, privacy, time, or trust.

### Use All Six CSF 2.0 Functions

The [NIST Cybersecurity Framework 2.0](https://www.nist.gov/cyberframework)
organizes outcomes under six functions:

* **Govern:** Set strategy, roles, policy, risk limits, and legal duties.
* **Identify:** Know assets, systems, suppliers, weak points, and risk.
* **Protect:** Apply safeguards and prepare people and systems.
* **Detect:** Find and assess signs of an event.
* **Respond:** Contain harm, act on the cause, and communicate.
* **Recover:** Restore work, confirm safety, and improve the plan.

The functions are concurrent and continuous. They are not six steps that
begin only after an alert.

### Turn Policy into a Testable Control

A **security policy** states rules, roles, and proof for a security goal.
It should be clear enough to enforce and test.

Use this policy record:

1. **Purpose and scope:** State the risk, people, data, systems, and places covered.
2. **Roles:** Name the owner, user, approver, reviewer, and backup.
3. **Required control:** State the act in plain terms.
4. **Technical enforcement:** Name the setting, block, log, test, or alert.
5. **Exception path:** Name who may approve an exception, why, and for how long.
6. **Proof:** State which record shows that the control works.
7. **Failure response:** State the fix, support, and fair result when the rule fails.
8. **Review:** Set an event or date that starts the next review.

A policy that says "use strong passwords" is hard to test. A better rule
can require passphrases, block known weak choices, require MFA, and name
the recovery path. The control should make the safe act easy.

Avoid blame-only policy. If ten people send data through personal mail
to complete a task, the team should ask why the approved tool fails. A
policy can need both a rule and a better work path.

**Worked risk register:** A city keeps one online backup for its permit
system. The backup uses the same admin account and network as the live
server. No restore test has run for eight months.

Ransomware or an admin-account loss could reach both copies. The impact
may include stopped permits, changed records, and loss of public data.
The likelihood rating needs local facts, but the shared path is a clear
weakness.

The city can reduce risk with a separate backup identity, an offline or
isolated copy, alerts, and restore tests. The owner should record what
risk remains and when the next test must pass.

### Try It Yourself 11.3: Rank a Patch Delay 🛠️

**Predict:** A public server has a known flaw. The patch may break one
old app. Should the team wait one month?

**Run:** Fill the nine-column risk register. Compare patch, isolate,
temporary control, app fix, and service pause options.

**Explain:** In 1-2 sentences, choose an action and name the proof needed
before the delay is approved.

### Quick Check 11.3 ✅

1. Name the six NIST CSF 2.0 functions. *(Understand)*

2. Distinguish reducing, sharing, avoiding, and accepting risk. *(Apply)*

3. Why must a security policy name both enforcement and an exception path? *(Evaluate)*

---

## 11.4 Respond, Preserve Proof, and Recover

**Incident response** is planned work to prepare for, find, contain,
remove, report, and recover from a security event.

[NIST SP 800-61 Revision 3](https://csrc.nist.gov/pubs/sp/800/61/r3/final)
connects response to all six CSF 2.0 functions. Govern, Identify, and
Protect reduce the number and impact of incidents. Detect, Respond, and
Recover help the team act when an event occurs.

### Use a Live Response Board

For each incident, keep a board with:

* Incident lead, backup, time, severity, and current state
* Known facts, open questions, and source of each fact
* Affected assets, accounts, people, and services
* Containment acts, owner, approval, time, and result
* Evidence items and storage location
* Legal, privacy, insurer, vendor, law-enforcement, and notice contacts
* Recovery test, business owner, and return-to-service approval
* Next update time and decision

The board separates facts from guesses. It also keeps two teams from
changing the same system in conflict.

### Build a Notice Map Before an Incident

Breach notice duties vary by data, people, place, contract, and sector.
A health plan, school, bank, state agency, and online shop may face
different rules. Deadlines and required recipients also vary.

Build a notice map with:

* Data and system type
* Home or location of affected people
* Contract and sector rules
* Trigger and deadline
* Required regulator, client, insurer, law-enforcement, and person notice
* Approval owner and backup
* Facts needed for the notice

Do not wait for perfect certainty when a deadline has begun. State what
is known, what remains open, and what people can do now. Legal staff
should confirm the rule and wording.

### Preserve Digital Evidence Under a Plan

**Digital forensics** is the use of tested methods to find, collect,
preserve, examine, and report digital facts. It may support response,
discipline, a civil case, or a criminal case.

NIST SP 800-86 warns that its forensic guide is not a full step-by-step
manual or legal advice. The right act depends on the system and case.
Turning off a host may lose memory data. Leaving it online may allow more
harm. The incident lead and qualified analyst must choose under the plan.

Use an evidence log:

1. **Item and source:** Identify the device, file, log, account, or service.
2. **Time and collector:** Record when, how, and by whom it was collected.
3. **Method and tool:** State the command, export, image, or tool version.
4. **Integrity check:** Record a hash or other check when it fits.
5. **Original and working copy:** State which item remains unchanged.
6. **Storage and access:** Record where it is kept and who may reach it.
7. **Transfer:** Record each handoff, time, sender, receiver, and reason.
8. **Limits:** State gaps, clock errors, missing logs, or other weak proof.

The **chain of custody** is the record of evidence control and transfer.
A gap can weaken trust and may affect legal use. It does not support a
simple claim that all evidence is always rejected.

A **forensic image** is a controlled copy made for analysis. Do not make
one on a live system without the role, tool, skill, and plan to do so.
Preserve first through the approved playbook and call the right expert.

### Put AI Security Tools Behind an Action Gate

AI can group alerts, find odd patterns, summarize logs, and draft steps.
Attackers can use AI to scale false messages, clone a voice, or change
malware. Both uses still depend on people, access, tools, and weak points.

Do not let an AI score become proof by itself. Before an automated tool
blocks an account, wipes a host, or stops a service, record:

* The source data and alert
* The action and possible business harm
* The error rate and known blind spots
* The person who may approve or reverse it
* The rollback and evidence plan
* The test that confirms the action worked

Low-risk, easy-to-reverse acts may be automatic. High-impact or hard-to-
reverse acts need a clear approval rule.

**Worked response board:** An AI tool flags a late-shift worker for a
large file copy. It blocks the account. The worker was moving a client
backup under a change ticket, but the tool did not read the shift or
ticket data.

The block may still limit harm while the team checks. A human should
review the ticket, file path, device, volume, and target. If the work was
approved, the team should restore access and add the case to its tests.

The team must also ask why the tool lacked needed context. A person who
works at night should not face a lasting fraud label from one weak score.

### Try It Yourself 11.4: Choose a Containment Step 🛠️

**Predict:** A server sends data to an unknown site, but it runs a key
public service. Should the team unplug it at once?

**Run:** Use the response board, CIA map, and evidence log. Compare full
isolation, network limits, traffic capture, failover, and service pause.

**Explain:** In 1-2 sentences, choose the first step and name who must
approve it.

### Quick Check 11.4 ✅

1. How do all six CSF functions support incident response? *(Understand)*

2. Why can shutting down a host help one goal and harm another? *(Analyze)*

3. Which AI security acts may be automatic, and which need approval? *(Evaluate)*

---

## 11.5 Summary and Retrieval 💡

### Key Concepts

* **Map the asset and harm.** Link each threat, weakness, and path to confidentiality, integrity, availability, people, and proof.

* **Trace identity harm by data field.** Different data supports different fraud, warning signs, and recovery steps.

* **Read the CFAA after *Van Buren*.** Improper purpose alone does not mean a person exceeded approved access to data.

* **Rank risk with stated proof.** Likelihood and impact need a scale, source, uncertainty, owner, action, and residual-risk record.

* **Use all six CSF 2.0 functions.** Govern, Identify, Protect, Detect, Respond, and Recover work together.

* **Write policies that systems can enforce.** State scope, roles, control, exception, proof, response, and review.

* **Preserve proof under a plan.** Keep facts apart from guesses, control access, record transfers, and call qualified staff.

### Key Terms

#### Section 11.1

* CIA Security Triad
* Confidentiality
* Integrity
* Availability
* Threat
* Vulnerability
* Exploit
* Incident
* Ransomware
* Multi-factor authentication (MFA)

#### Section 11.2

* Identity theft
* Personally identifiable information (PII)
* Synthetic identity theft
* Child identity theft
* Computer Fraud and Abuse Act (CFAA)

#### Section 11.3

* Risk assessment
* NIST Cybersecurity Framework
* Security policy
* Principle of least privilege
* Residual risk

#### Section 11.4

* Incident response
* Digital forensics
* Evidence log
* Chain of custody
* Forensic image
* Security Operations Center (SOC)

### Retrieval Practice

Try to answer these from memory before looking back at the chapter.

1. Name the seven lines in the incident map.
2. Name the six NIST CSF 2.0 functions.
3. Name five fields in the evidence log.

---

## 11.6 Skills Lab 11A: The MidState Credential Incident

**Goal:** Analyze an identity and data incident, then create a response plan, policy control, evidence log, and notice record.

**Evidence packet:** `assets/code/chapter-11/incident-response-case.md`, a fictional case and evidence packet created for this textbook.

**Estimated time:** 90-120 minutes

### Case: One False Message, Six Used Accounts

**Fictional case:** MidState Community College has 12,000 students and
800 workers. Its student system holds names, Social Security numbers,
birth dates, aid data, and grades.

A false help-desk message reaches 200 faculty accounts. Thirty-two people
enter a password on the false page. Six accounts then open the student
system. The system holds records for 4,500 students in the affected view.

The logs show that three of the six accounts exported files. The export
names are known, but the school has not checked the row count or fields.
Two accounts sent a false scholarship form to students. The form asks
for bank and tax data.

Faculty accounts do not use MFA. Each faculty member can open the full
student view. Sign-in logs are kept for 30 days. The mail team first
deleted the false messages, then learned that the legal team wanted a
copy. No one recorded which admin ran the deletion.

One backup is online under the same admin account as the student system.
The school has no tested notice map or response role chart. Leaders must
choose the first containment steps and the scope of the student notice.

<!-- markdownlint-disable MD029 -->

### Part 1: Foundation (Aligns with MLO-11.1)

1. Complete the seven-line incident map for the false message, stolen passwords, student-system access, file exports, and scholarship form.
2. Complete the six-line identity harm map. Link each known or possible data field to a form of harm and support step.
3. Separate known facts, sound inferences, and open questions. Name the log or person that could answer each open question.

### Part 2: Application (Aligns with MLO-11.1, MLO-11.2)

4. Build a nine-column risk register for MFA, access scope, mail controls, log retention, evidence handling, and backup separation.
5. Draft two policy records. One must cover MFA and one must cover least privilege or evidence preservation.
6. Create an evidence log for the false message, sign-in logs, student access logs, file exports, and affected account records.

### Part 3: Extension (Aligns with MLO-11.2, MLO-11.3)

7. Build a response board with actions under all six CSF 2.0 functions. Include owner, approval, time, result, and recovery test.
8. Draft a 200-300 word student notice. Separate known access from possible exposure and give steps tied to the data.

<!-- markdownlint-enable MD029 -->

### Questions & Analysis 🤔

1. Which control would have broken the attack path earliest?
2. How should MidState state uncertainty without hiding the risk?

### Rubric: Skills Lab 11A

This lab is graded with the standard
[Skills Lab Rubric](../skills-lab-rubric.md): four criteria at
4 points each, 16 points total. The criteria are Technical Accuracy
and Efficiency, Output Quality, Documentation Quality, and Analysis,
Interpretation, and Response to QUESTION(s).

For CIS111, **Technical Accuracy and Efficiency** means matching each
asset, identity risk, control, response step, and notice claim to the
case proof. **Output Quality** means that the plan, records, and notice
are clear, consistent, evidence-safe, and ready for team use.

### Submission Guidelines

* **Length:** 1,000-1,500 words total across all parts
* **Format:** Submit one PDF named `skills-lab-11a-lastname.pdf`. Use clear headings for each part and label both Questions & Analysis answers.

---

## 11.7 Review Questions 🔄️

1. **Understand:** Explain how one event can harm all three CIA goals.
2. **Apply:** Use the identity harm map for a stolen tax file.
3. **Analyze:** Analyze a patch delay with the nine-column risk register.
4. **Create:** Draft an evidence-safe first response to a server alert.

## Further Reading 📖

* [NIST Cybersecurity Framework 2.0](https://www.nist.gov/cyberframework): NIST organizes risk outcomes under six functions.
* [NIST SP 800-61 Revision 3](https://csrc.nist.gov/pubs/sp/800/61/r3/final): NIST connects incident response to all six CSF 2.0 functions.
* [NIST SP 800-30 Revision 1](https://csrc.nist.gov/pubs/sp/800/30/r1/final): NIST explains threat, weakness, likelihood, impact, and uncertainty in risk assessment.
* [NIST SP 800-86](https://csrc.nist.gov/pubs/sp/800/86/final): NIST explains how forensic work can support incident response.
* [IdentityTheft.gov](https://www.identitytheft.gov/steps): The FTC creates a case-based report and recovery plan.
* [CISA: Recognize and Report Phishing](https://www.cisa.gov/secure-our-world/recognize-and-report-phishing): CISA explains phishing signs and reporting steps.
* [Supreme Court: *Van Buren v. United States*](https://www.supremecourt.gov/opinions/20pdf/19-783_k53l.pdf): The Court explains the CFAA access limit.
* [DOJ CFAA Charging Policy](https://www.justice.gov/archives/opa/pr/department-justice-announces-new-policy-charging-cases-under-computer-fraud-and-abuse-act): DOJ explains current federal charging rules and good-faith research.
* [U.S. Code: CFAA](https://uscode.house.gov/view.xhtml?req=%28title%3A18+section%3A1030%29): The House provides the current statute.

## Looking Ahead ⏩

Chapter 12 turns to professional duty. You will compare codes of ethics,
set an escalation path, and defend a capstone choice with proof.
