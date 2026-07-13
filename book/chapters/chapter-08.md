# Chapter 8: Regulation, Self-Regulation, and IT Work

A Phoenix software firm launches one app. A customer in California asks
to delete data. A family in France uses the same app. A child creates an
account. The firm also uses an AI tool to rank job applicants.

One product can face several rules at once. Each rule may cover a
different party, person, data type, or act. A good IT worker does not
guess from a law's name. The worker checks scope, date, duty, and proof.

This chapter gives you tools for that work. You will compare law with
self-regulation, assess H-1B and offshore work choices, and apply current
AI rules without treating compliance as the full ethics test.

## Module Overview 🧭

* **Estimated time:** 4-5 hours (reading + practice + Skills Lab)
* **Prerequisites:** Chapters 1-7
* **Deliverables:** Try It Yourself activities, Quick Checks, Skills Lab 8A

## Learning Objectives 🎯

By the end of this chapter, you will be able to:

* **MLO-8.1 (Apply):** Apply a scope map to decide which privacy and AI rules may govern an IT case
* **MLO-8.2 (Analyze):** Analyze whether law, self-regulation, audits, and sanctions create enough accountability
* **MLO-8.3 (Evaluate):** Evaluate an H-1B or offshore work choice for pay, power, voice, and transition harm

### This chapter aligns with the following Course Learning Outcomes

* **CLO X.** Evaluate the influence of government regulations as well as professional self-regulation and sanctions in ethical information technology decision-making.

---

## 8.1 Map the Scope of Data and AI Rules

A law does not cover a system just because the system uses data. Start
with the facts that bring a party, person, or act within the rule.

Use this six-question scope map:

1. **Place:** Where are the firm, user, worker, and data use?
2. **Party:** Is the group a covered business, operator, provider, plan, or other named party?
3. **Person:** Does the rule protect a child, consumer, patient, worker, or person in a set place?
4. **Data and act:** What data is collected, used, sold, shared, ranked, or deleted?
5. **Date:** Which version and start date govern the act?
6. **Duty and proof:** What must the party do, and what record proves it?

The map can show that more than one rule applies. It can also show that a
well-known law does not fit the facts.

### GDPR: Check the Link to the EU

The **General Data Protection Regulation (GDPR)** governs personal data
within its scope. It can apply when a group has an EU establishment. It
can also apply to a group outside the EU when that group offers goods or
services to people in the EU or monitors their behavior there.

An Arizona website does not enter GDPR scope only because a person in
France can open it. The offer, monitoring, or EU establishment facts
matter.

GDPR requires a lawful basis for processing. Consent is one basis, but
it is not the only one. The regulation also sets data principles and
rights. These include data minimization, access, and erasure subject to
limits.

A controller must report some personal data breaches to its oversight
authority within 72 hours after it becomes aware. The rule has a risk
test and content duties. Do not reduce it to "all breaches in 72 hours."
The
[official GDPR text](https://eur-lex.europa.eu/eli/reg/2016/679/oj/eng)
controls the legal analysis.

### CCPA and CPRA: Check the Business Threshold

The **California Consumer Privacy Act (CCPA)**, as amended by the
**California Privacy Rights Act (CPRA)**, gives California consumers
rights over personal information. Rights include knowing, deleting,
correcting, and opting out of certain sale or sharing. Exceptions and
verification rules apply.

The law covers a for-profit business that does business in California,
collects consumer data, and meets a statutory test. One test uses annual
gross revenue. The California Privacy Protection Agency raised that
amount to
[$26,625,000 for 2025](https://cppa.ca.gov/announcements/2024/20241217.html).
The amount can change with later adjustments.

Other tests include buying, selling, or sharing data tied to at least
100,000 consumers or households, or gaining at least half of annual
revenue from sale or sharing. Do not apply one threshold without checking
the others and the current law.

### COPPA and HIPAA: Check the Role and Data

The **Children's Online Privacy Protection Act (COPPA)** and its rule
cover certain online services aimed at children under 13. They can also
cover an operator with actual knowledge that it collects personal data
from a child under 13.

COPPA uses notice and **verifiable parental consent**. The FTC's 2025
rule update added stronger limits for child data. Among other changes,
it requires separate parental consent for certain third-party
disclosures tied to targeted ads. It also adds data-retention and
security duties. The FTC posts the
[current COPPA rule materials](https://www.ftc.gov/legal-library/browse/federal-register-notices/16-cfr-part-312-coppa-final-rule-amendments).

HIPAA uses a different scope. As Chapter 6 explained, it covers certain
health plans, clearinghouses, providers, and business associates. A
health fact in a general app is not always PHI.

### Build a Rule Matrix

Use a short matrix instead of a memory guess.

| Rule | Scope fact to test | Core IT question |
| --- | --- | --- |
| GDPR | EU establishment, offer, or monitoring | What lawful basis, right, or breach duty applies? |
| CCPA / CPRA | California business and threshold | Can the person know, fix, delete, or opt out? |
| COPPA | Child-directed service or actual knowledge | Did the operator get the right parental consent? |
| HIPAA | Covered entity or business associate and PHI | Which privacy, security, or breach rule applies? |

Keep a source title, URL, review date, and rule version with the matrix.
Rules change. A saved screenshot or vendor claim is weak proof of the
current law.

### Try It Yourself 8.1: Scope a Tutoring App 🛠️

**Predict:** An Arizona tutoring app serves families in California and
France. It allows children under 13 to create profiles. Which rules may
apply?

**Run:** Fill all six scope questions for GDPR, CCPA / CPRA, COPPA, and
HIPAA. Mark HIPAA as in or out based only on the facts given.

**Explain:** In 1-2 sentences, name the strongest rule match and one
fact still needed.

### Quick Check 8.1 ✅

1. Why does an EU visitor to a website not by itself prove GDPR scope? *(Understand)*

2. A California firm falls below the revenue test. Which other CCPA tests must it check? *(Apply)*

3. Why should an analyst state that a law does not apply instead of leaving it out? *(Analyze)*

---

## 8.2 Test Self-Regulation, Audits, and Sanctions

Government regulation creates binding duties through public law.
**Self-regulation** creates rules through a profession, industry, or
firm. Both can shape IT choices.

The hard question is not which source sounds better. Ask what conduct it
covers, who checks it, and what happens after a breach.

### Compare the Sources of Rules

A public law can reach parties that would not volunteer. A regulator may
investigate, order a change, or seek a penalty. The public process can be
slow and the rule may lag behind a new tool.

A professional standard can use deep field knowledge and change faster.
Yet a group may leave, ignore the rule, or accept a weak sanction.

The ACM Code of Ethics asks computing workers to avoid harm, assess
system risk, and give the public good first place. ACM can act within its
membership process. It cannot revoke a government license that most IT
roles do not need. The
[ACM Code of Ethics](https://www.acm.org/about-acm/code-of-ethics)
still gives workers a common duty test.

### Distinguish a Standard from a Law

The **Payment Card Industry Data Security Standard (PCI DSS)** is a
private standard for cardholder data. Payment agreements and card-brand
rules can make compliance a business condition. PCI DSS is not a law
only because a firm must follow it to process cards.

This distinction matters in a report. Name the source of the duty:

* A statute or regulation
* A contract or payment rule
* A professional code
* A firm policy
* An ethical duty beyond the written rule

More than one source may apply to the same act.

### Audit the Audit

A **social audit** reviews a firm's effects on people and communities.
An AI audit may test group results, access, data sources, and appeals. A
privacy audit may test notice, retention, deletion, and vendor sharing.

An audit is only as useful as its design. Check five facts:

1. Who chose the scope and paid the reviewer?
2. Did the reviewer have the data and access needed?
3. Did the test include affected groups and failure cases?
4. Will leaders publish the limits and bad results?
5. Who owns each fix, deadline, and follow-up test?

A badge without evidence can hide risk. A clear audit with no fix can do
the same.

### Test the Sanction

A sanction should deter harm, correct the system, and help those harmed
when possible. Test its strength:

* **Reach:** Does it apply to the party that made the choice?
* **Cost:** Is the loss large enough to change conduct?
* **Speed:** Can it act before more harm spreads?
* **Repair:** Does it require a fix, notice, or relief?
* **Review:** Can an independent party verify the result?

The best structure may mix law and self-regulation. A field group can
write a strong standard. A contract or public rule can give the standard
teeth.

### Case Study 8.1: The Narrow Privacy Audit 📋

**Fictional case:** TechBridge tracks shopping, location, and web use for
online stores. A voluntary industry audit finds three gaps. The firm
keeps data for seven years, takes up to 90 days to process some opt-outs,
and joins data from different clients without clear notice.

The privacy officer wants to report all three gaps and fix them. The CEO
wants to report only the slow opt-outs. The audit group can remove its
seal but cannot fine TechBridge.

Full repair may cost $2 million and worry clients. A narrow report saves
money now but weakens the audit and leaves people without a fair picture
of the data use.

### Try It Yourself 8.2: Test the Audit Seal 🛠️

**Predict:** Should the audit group renew TechBridge's seal while two
findings stay hidden?

**Run:** Apply the five audit facts and five sanction tests. Then compare
the result with stakeholder theory.

**Explain:** In 1-2 sentences, choose renew, suspend, or revoke. Name the
proof needed for a later renewal.

### Quick Check 8.2 ✅

1. How does a professional code differ from a government license? *(Understand)*

2. Why is PCI DSS a private standard even when a payment contract requires it? *(Apply)*

3. Which sanction tests matter most when harm can spread fast? Defend two. *(Analyze)*

---

## 8.3 H-1B and Offshore Work Choices

IT policy also shapes workers. A firm may sponsor a worker from another
country, hire an outside vendor, or move work abroad. Each choice affects
pay, power, voice, and job loss.

Avoid two false frames. A worker is not a cost unit. A global hire is not
the cause of every local job loss. Test the firm's exact plan and how it
treats each group.

### Know the H-1B Baseline

The **H-1B visa** lets an eligible US employer sponsor a worker for a
specialty occupation for a limited period. The job must meet current
legal tests. The employer files the petition and a Labor Condition
Application.

The wage rule is more precise than "pay the prevailing wage." The
employer must pay at least the higher of the local **prevailing wage** or
the actual wage paid to similar workers at the firm. The Department of
Labor lists this and other
[H-1B worker rights](https://www.dol.gov/agencies/whd/workers/h1b).

The program also bars certain retaliation for reporting a suspected
H-1B violation or helping an inquiry. Legal rights do not remove all
fear. A worker may still worry about job loss, a new petition, family
status, or a long-term immigration plan.

An H-1B worker is not locked forever to one firm. A new eligible employer
can file a petition, and portability rules may permit work to start after
a proper filing. The worker should get qualified advice for the facts.

### Test Power and Voice

A fair H-1B plan should ask:

* Does the worker receive the required wage, benefits, and work terms?
* Can the worker report a risk without a manager who controls the case?
* Does the firm explain job, site, and status changes in plain language?
* Can staff compare pay bands and promotion rules?
* Does the firm act on retaliation or threats?

The same checks protect US workers from unfair pay or hidden replacement
plans. Fair treatment is not a contest between worker groups.

### Test Offshore Outsourcing

**Offshore outsourcing**, or offshoring, moves work to a vendor or staff
in another country. The choice may add skill, lower cost, extend service
hours, or reach a new market. It may also displace staff, weaken voice,
or expose data to a new legal and security setting.

Use a fair-work transition test:

* **Need:** What goal cannot a safer option meet?
* **Notice:** When and how will each worker learn the plan?
* **Voice:** Can workers question facts and propose another path?
* **Support:** What severance, training, placement, or time will the firm provide?
* **Vendor work:** What pay, hours, safety, and report rights apply abroad?
* **Data:** Which access, location, contract, and incident rules change?
* **Accountability:** Who checks both firms after the move?

Lower pay in another labor market does not by itself prove abuse. A cost
gap also does not excuse unsafe work, hidden surveillance, or weak data
care.

### Try It Yourself 8.3: Review a Support-Center Move 🛠️

**Predict:** A firm will move 60 support jobs abroad and save $4 million
each year. It offers 14 days of pay and no training. Is the plan fair?

**Run:** Apply all seven transition tests. Add one option that saves part
of the cost with less worker harm.

**Explain:** In 1-2 sentences, choose approve, change, or reject. Name
the worker group your choice protects most.

### Quick Check 8.3 ✅

1. What two wage figures must an H-1B employer compare? *(Understand)*

2. Why can legal portability still leave a worker with less power to report harm? *(Analyze)*

3. Apply the fair-work transition test to an offshoring plan with no data-location review. *(Apply)*

---

## 8.4 Combine Binding AI Rules with Voluntary Controls

AI rules change by place, use, role, and date. A chatbot, hiring ranker,
medical device, and spam filter do not share one legal class.

Start with the Chapter 8 scope map. Then add the AI system's intended
use, affected people, provider, deployer, model source, and release date.

### Use the Current EU AI Act Timeline

The **EU AI Act** uses bans, duties for general-purpose models,
high-risk rules, transparency duties, and other requirements. It does
not place every AI tool in a simple four-box ladder.

Some bans and AI literacy duties have applied since February 2, 2025.
General-purpose AI duties began to apply on August 2, 2025. Some
transparency duties are scheduled for August 2, 2026.

The timeline for high-risk rules changed after a May 2026 political
agreement on the AI Omnibus. The European Commission's
[current AI Act page](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai)
lists December 2, 2027 for certain stand-alone high-risk uses, including
employment. It lists August 2, 2028 for high-risk AI in certain regulated
products.

These dates can change as the final legal steps and support standards
move forward. Check the official page and law on the date of the choice.

### Apply Existing US Law by Use

The United States has no single federal AI law that replaces all other
rules. Existing law may still govern an AI use.

The FTC can act against some unfair or deceptive commercial practices.
Employment discrimination law can apply when a firm uses software or AI
for a job choice. The
[EEOC publications page](https://www.eeoc.gov/eeoc-publications)
lists current worker and employer resources. Privacy, credit, health,
and state laws may also apply.

Do not accept "AI is unregulated" as a full answer. Name the use, claim,
data, people, and place.

### Use NIST as a Voluntary Control

The **NIST AI Risk Management Framework** is voluntary. It uses Govern,
Map, Measure, and Manage. It can help a firm set roles, define context,
test harm, and act on results.

Voluntary does not mean useless. It also does not mean legally complete.
A firm can use NIST to produce evidence for a duty that comes from law,
contract, policy, or ethics.

### Join the Tests

Use a rule-and-control record:

1. Name the system, version, intended use, and people affected.
2. List each binding rule, role, duty, and start date.
3. List each voluntary control and the risk it reduces.
4. Record test data, group results, limits, and open gaps.
5. Name the person who can stop use and the restart proof.
6. Set the next law and model review date.

This record keeps compliance tied to system facts. It also shows where
the ethical duty reaches past the legal floor.

### Try It Yourself 8.4: Check an AI Hiring Pilot 🛠️

**Predict:** A US firm wants to pilot an AI resume ranker for jobs in
France. The vendor calls it compliant but gives no group test results.
Should the pilot start?

**Run:** Build the rule-and-control record. Check the current EU date,
US employment law, NIST functions, group tests, stop right, and appeal.

**Explain:** In 1-2 sentences, choose start, start with conditions, or
delay. Name the proof that controls your choice.

### Quick Check 8.4 ✅

1. Why should you not describe the EU AI Act as only four risk tiers? *(Understand)*

2. How can NIST AI RMF evidence support a binding legal duty? *(Apply)*

3. Why must an AI compliance record include both a rule date and model version? *(Analyze)*

---

## 8.5 Summary and Retrieval 💡

### Key Concepts

* **Rule scope depends on facts.** Place, party, protected person, data act, date, duty, and proof decide whether GDPR, CCPA, COPPA, HIPAA, or an AI rule fits.

* **Self-regulation needs evidence and sanctions.** A code, audit, or seal is weak when it lacks reach, cost, speed, repair, or independent review.

* **H-1B ethics includes pay and power.** The legal wage uses the higher of the actual or prevailing wage, while fair practice also protects voice and report rights.

* **Offshoring affects workers in both places.** A sound transition tests need, notice, voice, support, vendor work, data, and later checks.

* **AI compliance joins law and voluntary controls.** Teams must check current dates and roles, then use tools such as NIST to gather proof and manage risk.

### Key Terms

#### Section 8.1

* GDPR
* CCPA / CPRA
* COPPA
* Verifiable parental consent

#### Section 8.2

* Self-regulation
* PCI DSS
* Social audit

#### Section 8.3

* H-1B visa
* Prevailing wage
* Offshore outsourcing (offshoring)

#### Section 8.4

* EU AI Act
* NIST AI Risk Management Framework

### Retrieval Practice

Try to answer these from memory before looking back at the chapter.

1. Name the six questions in the rule scope map.
2. Name the five tests for a sanction.
3. Name the seven parts of the fair-work transition test.

---

## 8.6 Skills Lab 8A: The TalentBridge Launch

**Goal:** Build a current regulation and ethics plan for an AI hiring platform.

**Evidence packet:** `assets/code/chapter-08/ai-hiring-regulation-case.md`, a fictional case and evidence packet created for this textbook.

**Estimated time:** 90-120 minutes

### Case: A Hiring Tool Crosses Borders

**Fictional case:** TalentBridge AI is a Phoenix startup. Its platform
ranks resumes and scores recorded job interviews. More than 200 US firms
use it. The firm plans to launch with clients in France and Germany.

The resume model helps decide which applicants receive an interview. An
outside group tested 400 matched resumes. In that small test, resumes
from historically Black colleges received an average score eight points
lower than matched resumes from other schools. TalentBridge disputes the
test but has not published its own group results.

The video tool scores speech pace, eye movement, word choice, and a
vendor-defined "confidence" measure. The contract does not explain
whether the tool infers emotion or uses biometric identification. Those
facts can change the legal analysis.

TalentBridge also plans to move its 45-person Phoenix data-labeling team
to a vendor in the Philippines. The US team received 90 days' notice but
no severance, training, or placement help. The vendor contract names pay
and hours but gives TalentBridge no audit right for worker complaints.

Twelve engineers hold H-1B status through TalentBridge. Two reported
model-bias concerns to a manager. They want an independent report path
before the EU launch.

Leaders may launch, run a limited pilot with added controls, or delay.

<!-- markdownlint-disable MD029 -->

### Part 1: Foundation (Aligns with MLO-8.1)

1. Apply the six-question scope map to GDPR, CCPA / CPRA, COPPA, and HIPAA. Mark each rule in, out, or uncertain and cite a case fact.
2. Test whether the resume and video uses may face a ban, high-risk rule, transparency duty, or another EU AI Act duty. State each missing fact and date.
3. Build a source log with the official title, URL, review date, and rule version for each possible binding duty.

### Part 2: Application (Aligns with MLO-8.1, MLO-8.2)

4. Apply the five audit facts and five sanction tests to the outside bias report and TalentBridge's proposed review.
5. Use Govern, Map, Measure, and Manage to list one control and one proof item for each NIST AI RMF function.
6. Design a report path for all engineers. Explain how it protects H-1B workers and other staff from retaliation or manager control.

### Part 3: Extension (Aligns with MLO-8.2, MLO-8.3)

7. Apply the seven-part fair-work transition test to the labeling-team move. Propose three contract or support changes.
8. Write a 200-300 word launch memo. Choose launch, conditional pilot, or delay. Name a stop rule and the evidence that would change your choice.

<!-- markdownlint-enable MD029 -->

### Questions & Analysis 🤔

1. Which missing fact creates the greatest legal or ethical risk?
2. Which voluntary control should the firm use even if no law requires it?

### Rubric: Skills Lab 8A

This lab is graded with the standard
[Skills Lab Rubric](../skills-lab-rubric.md): four criteria at
4 points each, 16 points total. The criteria are Technical Accuracy
and Efficiency, Output Quality, Documentation Quality, and Analysis,
Interpretation, and Response to QUESTION(s).

For CIS111, **Technical Accuracy and Efficiency** means matching each
rule and control to current scope facts, dates, and source evidence.
**Output Quality** means that your launch plan is clear, organized, and
safe for leaders and affected workers to use.

### Submission Guidelines

* **Length:** 800-1,200 words total across all parts
* **Format:** Submit one PDF named `skills-lab-8a-lastname.pdf`. Use clear headings for each part and label both Questions & Analysis answers.

---

## 8.7 Review Questions 🔄️

1. **Understand:** Explain why a data law's name does not prove its scope.
2. **Apply:** Apply the sanction test to a voluntary privacy seal.
3. **Analyze:** Analyze how visa sponsorship may affect a worker's power to report risk.
4. **Evaluate:** When should a firm delay an AI launch even if the legal start date is later? Defend a threshold.

## Further Reading 📖

* [Official GDPR Text](https://eur-lex.europa.eu/eli/reg/2016/679/oj/eng): The EU regulation gives the controlling scope, principles, rights, duties, and penalties.
* [California Privacy Protection Agency: CCPA Threshold Updates](https://cppa.ca.gov/announcements/2024/20241217.html): The agency lists the current inflation-adjusted revenue threshold and penalties.
* [FTC COPPA Rule Amendments](https://www.ftc.gov/legal-library/browse/federal-register-notices/16-cfr-part-312-coppa-final-rule-amendments): The FTC provides the current child-privacy rule text.
* [Department of Labor: H-1B Worker Rights](https://www.dol.gov/agencies/whd/workers/h1b): DOL explains wage, benefit, work-condition, and report rights.
* [European Commission: AI Act](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai): The Commission tracks current duties, dates, and implementation work.
* [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework): NIST provides voluntary tools for governing, mapping, measuring, and managing AI risk.

## Looking Ahead ⏩

Chapter 9 turns from rules about data and work to rights in code, media,
inventions, and brands. You will test ownership, permission, and fair use.
