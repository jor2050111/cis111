# Chapter 7: Software Liability and Secure Design

On July 19, 2024, a faulty CrowdStrike update caused Windows systems to
crash. Microsoft estimated that the event affected
[8.5 million devices](https://blogs.microsoft.com/blog/2024/07/20/helping-our-customers-through-the-crowdstrike-outage/).
Flights stopped. Clinics delayed care. Payment and emergency systems
lost access to key tools.

The event was not a cyberattack. Code and release controls failed. One
update moved through many linked systems before teams could stop it.
The harm came from both the defect and the way the update was sent.

This chapter separates legal liability from ethical responsibility. You
will map software claims, use secure design rules, plan a safe update,
and assess when cost cannot excuse risk.

## Module Overview 🧭

* **Estimated time:** 4-5 hours (reading + practice + Skills Lab)
* **Prerequisites:** Chapters 1-6
* **Deliverables:** Try It Yourself activities, Quick Checks, Skills Lab 7A

## Learning Objectives 🎯

By the end of this chapter, you will be able to:

* **7.1 (Apply):** Apply negligence, product liability, warranty, and contract questions to a software harm case
* **7.2 (Analyze):** Analyze a software life cycle for secure design, safe release, disclosure, and patch duties
* **7.3 (Evaluate):** Evaluate a safety-critical software choice with cost, risk, stakeholder, and stop-rule tests

### This chapter aligns with the following Course Learning Outcomes

* **CLO VIII.** Examine issues with software and software liability.
* **CLO IX.** Apply cost/benefit analysis in information technology ethical decision-making.

---

## 7.1 From Software Harm to a Liability Claim

A **software defect**, often called a bug, is a flaw that causes a wrong
or unsafe result. The flaw may sit in code, a design, a setting, a data
link, or an update. A weak warning can also leave a user open to harm.

Do not ask only, "Who wrote the bad line?" A software system includes
people, tools, tests, contracts, and release choices. Each part can add
or reduce risk.

### Separate Ethics from Law

Ethical responsibility asks who could see the risk, prevent the harm,
or give a fair warning. Legal liability asks whether a claim meets the
law of a place. The two tests may reach different results.

A firm can meet a narrow contract term and still make a reckless choice.
A severe outage can also occur without proof that one party broke a
legal duty. Keep the tests separate, then compare them.

This chapter is not legal advice. Software claims depend on the product,
service, contract, harm, use, and jurisdiction.

### Map Four Claim Paths

**Negligence** asks whether a party owed a duty of reasonable care,
failed that duty, and caused harm. In a software case, facts may include
a known flaw, skipped test, weak warning, or unsafe release plan. A bad
result alone does not prove each part of the claim.

**Product liability** covers harm tied to a defective product. Some
claims use **strict liability**, which can focus on the defect and harm
without a test of the maker's level of care. Yet software does not receive one
legal label in every place or case.

Arizona law, for example, defines a
[product liability action](https://www.azleg.gov/ars/12/00681.htm)
through harm tied to design, testing, sale, warnings, and other product
work. The statute does not say that all software is or is not a product.
A court would still need facts and legal analysis.

The European Union made a different policy choice. Its 2024
[Product Liability Directive](https://eur-lex.europa.eu/legal-content/EN/TXT/?uri=CELEX%3A32024L2853)
treats software as a product for its no-fault liability rules. The text
includes software supplied through a device, a network, the cloud, or
Software as a Service. EU member states must put the directive into
national law on its schedule.

**Breach of warranty** asks whether software failed to meet an express
or implied promise. A sales claim, contract, or law may shape the
promise. A claim such as "blocks all threats" differs from a careful
statement of tested limits.

Contract claims may also matter. An **End User License Agreement
(EULA)** or service contract can set rights, duties, limits, and dispute
rules. Do not assume that each term will always hold or always fail. A
court may test notice, assent, law, wording, and public policy.

### Classify the Software and the Harm

**Software as a Service (SaaS)** is hosted by a provider and reached
through a network. Embedded code runs inside a device. A phone app may
stand alone. Open source code may enter a paid product through another
firm.

Those forms can change the legal questions. They do not erase the
ethical duty to test, warn, patch, and limit harm.

Use this six-line claim map:

* **Party:** Who built, sold, set up, changed, or used the system?
* **Duty or promise:** What care, warning, or result did that party owe?
* **Defect or breach:** Which act, gap, or product state may have failed?
* **Cause:** How did the failure lead to the harm?
* **Harm:** Was there injury, death, property loss, data loss, or another loss the law recognizes?
* **Law and contract:** Which place, statute, case, and term controls?

The map does not decide the case. It shows what proof is present and
what proof is still missing.

### Try It Yourself 7.1: Map a Failed Security Promise 🛠️

**Predict:** A security tool promises to block "all known threats." It
misses a threat listed in its own test set. The EULA limits damages.
Which claim path should counsel check first?

**Run:** Fill all six lines of the claim map. Mark each fact that the
case does not give you.

**Explain:** In 1-2 sentences, name one possible claim and the missing
fact that most limits your answer.

### Quick Check 7.1 ✅

1. How does ethical responsibility differ from legal liability? *(Understand)*

2. Why does a software defect not by itself prove negligence? *(Apply)*

3. Compare a warranty claim with a strict product liability claim. What proof differs? *(Analyze)*

---

## 7.2 Secure Design Across the Software Life Cycle

Software quality is not a polish step. **Software quality** includes fit
for the stated need, sound results, safe use, clear limits, and support
after release. The risk of harm should shape the depth of each check.

A game menu and an insulin pump do not need the same test plan. Both need
honest claims and a process that fits their risk.

### Use the NIST SSDF

**Secure coding** aims to prevent flaws that attackers can use. It is
one part of a wider life cycle. The
[NIST Secure Software Development Framework](https://csrc.nist.gov/pubs/sp/800/218/final)
groups secure work into four areas:

* **Prepare the group:** Set security needs, roles, training, and tools
* **Protect the software:** Guard code, build tools, accounts, and releases
* **Produce sound software:** Review design, check reused parts, test code, and record the release
* **Respond to flaws:** Receive reports, fix root causes, issue patches, and learn from events

The SSDF can fit agile, DevOps, waterfall, or another method. The method
name does not prove that the work is safe. The controls and proof do.

### Shift Risk Upstream

**Secure by design** places the main duty for safe product choices on
the maker, not on each customer. CISA asks software makers to take
ownership of customer security outcomes and be open about risk.

CISA and the FBI list
[product security bad practices](https://www.cisa.gov/resources-tools/resources/product-security-bad-practices)
that makers should avoid. The guidance covers product traits, security
features, and firm processes. It applies to installed software, cloud
services, SaaS, and code in operational systems.

A maker should not force each small clinic or school to repair the same
unsafe default. One upstream fix can protect many users at once.

### Track Technical Debt

**Technical debt** is the future cost and risk created by a shortcut.
Debt can come from old code, weak tests, an unsupported part, or a quick
manual fix.

Not all debt is wrong. A team may accept a short-term gap during an
emergency. The ethical failure starts when the team hides the debt,
gives it no owner, or lets users bear the risk without a plan.

Record each debt item with five facts:

1. The shortcut and reason
2. The people and systems at risk
3. The chance and scale of harm
4. The owner and due trigger for repair
5. The stop rule if risk grows

### Build a Safe Release Gate

A release gate is a test that software must pass before it reaches more
users. A safe update plan may use a small first group, staged growth,
health checks, a pause switch, and a tested rollback.

The gate should ask:

* Did tests cover the highest-risk use and failure mode?
* Did the build use the approved code and parts?
* Can the team detect harm fast?
* Can the team stop the rollout before it spreads?
* Can the team restore the last sound version?
* Who has the power to pause the release?

Speed is not the enemy. Unchecked speed is. A fast patch with a safe
gate may reduce harm. A slow release with weak tests may still fail.

### Case Study 7.1: The Silent Heart Alert 📋

**Fictional case:** MedTrack sells a patient monitor to regional
hospitals. Priya, a senior developer, finds a flaw. The tool can mark a
low heart rate and low oxygen reading as normal when both occur at once.

Her manager wants to wait three months for the next planned release. A
large sales deal is in progress. Leaders fear that a warning could end
the deal and lead to job cuts. Nurses still watch patients, but they use
the alert as a safety net.

Priya has proof from a repeatable test. The firm has no staged hotfix
plan and has not told hospital clients.

The case presents more than a code choice. It tests the release gate,
the debt record, the warning duty, and the report path from Chapter 5.

### Try It Yourself 7.2: Gate the MedTrack Fix 🛠️

**Predict:** Should MedTrack wait, warn clients and patch now, or stop
the affected feature while it tests a fix?

**Run:** Apply the six release-gate questions. Add the five technical
debt facts if any gap remains.

**Explain:** In 1-2 sentences, choose a path and state the stop rule.

### Quick Check 7.2 ✅

1. Name the four NIST SSDF practice groups. *(Understand)*

2. How does secure by design shift risk away from customers? *(Apply)*

3. Why must a technical debt record include an owner and stop rule? *(Analyze)*

---

## 7.3 Vulnerability Reports, Patches, and AI Code

A **vulnerability** is a weakness that a threat can use. Some flaws come
from code. Others come from access rules, unsafe settings, old parts, or
a broken supply chain.

Teams must prevent common flaws and respond well when someone finds a
new one.

### Use the Current OWASP Top 10

The **OWASP Top 10** is an awareness list for web app risk. The
[2025 release](https://owasp.org/Top10/2025/0x00_2025-Introduction/)
includes broken access control, bad settings, supply chain failures,
cryptographic failures, injection, and insecure design.

**SQL injection** occurs when untrusted input becomes part of a database
command. Safe parameter use can block this class of flaw. **Cross-site
scripting (XSS)** lets untrusted content run as script in another user's
browser. Output handling and a sound design help block it.

Do not use the Top 10 as a full test plan. It is a place to start. The
team must also test the language, framework, data, users, and threats for
its own product.

### Coordinate a Vulnerability Report

**Coordinated Vulnerability Disclosure (CVD)** gives a finder, vendor,
and sometimes a third-party coordinator a way to reduce harm. The finder
shares enough facts for the vendor to repeat the flaw. The parties plan
a fix and public notice with user safety in mind.

There is no single wait time for all flaws. A public attack, unsafe
medical tool, slow vendor, or hard patch can change the plan. A vendor
should publish a report path, safe-harbor terms, expected reply times,
and the facts it needs.

CISA's
[coordinated disclosure process](https://www.cisa.gov/coordinated-vulnerability-disclosure-process)
can help when a report affects several vendors or direct work breaks
down. Full public release may be sound in some cases, but it can also
give attackers a guide before users have a fix.

### Patch with Both Speed and Care

**Patch management** covers the choice, test, release, and tracking of a
fix. Teams should rank a flaw by active use, ease of attack, reach,
impact, and available controls.

The 2017 Equifax breach showed the cost of a known patch gap. The FTC
said the breach affected about 147 million people. Its
[Equifax settlement page](https://www.ftc.gov/enforcement/refunds/equifax-data-breach-settlement)
describes the case and relief.

A patch can also cause harm. Use a small first group, backups, health
checks, a rollback, and clear notice. Track which systems received the
fix. End-of-life software needs an honest date, a move plan, and added
controls while use remains.

### Review AI-Generated Code

An AI coding tool can write useful code and unsafe code. A clean build
does not prove safe access, input checks, cryptography, error handling,
or license use.

Put AI code through the same life cycle as human code:

* Record the tool, prompt context, source limits, and reviewer
* Check each reused package and license
* Review access, data flow, secrets, errors, and logs
* Run tests that cover misuse and odd inputs
* Require a person to approve the change

The person who approves the release owns the choice to trust the code.
The tool does not remove that duty.

### Try It Yourself 7.3: Plan a Library Disclosure 🛠️

**Predict:** You find a severe flaw in a library used by many apps. One
volunteer maintains it and has no public report policy. What should you
do first?

**Run:** Plan the first contact, proof, coordinator option, user guard,
patch test, and notice trigger.

**Explain:** In 1-2 sentences, choose a first step and state the fact
that would make you change the disclosure plan.

### Quick Check 7.3 ✅

1. Why is the OWASP Top 10 a starting point instead of a full test plan? *(Understand)*

2. Compare a fast public disclosure with a coordinated report. Which user risk does each path accept? *(Analyze)*

3. Name three checks that AI-generated code must pass before release. *(Apply)*

---

## 7.4 Cost, Risk, and Safety-Critical Systems

**Risk assessment** asks what can go wrong, how likely it is, and how
much harm it can cause. A simple teaching model is:

**Formula:** Risk = Likelihood x Impact

The model helps teams rank work. It does not turn a weak estimate into a
fact. A rare event can still need fast action when the harm is grave.

### Put Guardrails Around Cost and Benefit

**Cost/benefit analysis** compares the costs of a choice with its gains.
Costs may include time, money, lost service, safety, privacy, and trust.
Some values fit a dollar estimate. Others do not.

Use six guardrails:

* **Floor:** Does a law, right, promise, or duty rule out an option?
* **Distribution:** Who gains, and who bears the risk?
* **Uncertainty:** Which rate, cost, or outcome is not known?
* **Scale:** How many people and linked systems could face harm?
* **Reversibility:** Can the team stop and repair the choice?
* **Alternatives:** Is there a safer path that the first estimate left out?

A choice is weak when the buyer gains and a person with no voice bears
the worst harm. Add the missing harm to the record even when no fair
dollar value exists.

### Treat Safety-Critical Work Differently

A **safety-critical system** can cause death, grave injury, or major
physical harm when it fails. Examples include code in aircraft, medical
devices, rail control, and industrial plants.

Such work needs strong proof. The exact standard depends on the field
and product. Common controls include:

* Independent checks for high-risk work
* More than one way to detect or stop a fault
* A safe state when the system cannot act with trust
* Trace links from each safety need to its test
* A release record with known limits and open risks
* Drills for stop, rollback, and recovery

A **safety case** joins a claim, evidence, and reasons that support safe
use in a stated setting. It also names the limits. "No failure seen" is
not the same as proof that the next use is safe.

### Map Responsibility in AI Systems

**AI liability** asks who may bear legal or ethical responsibility when
an AI system causes harm. The chain can include a data source, base-model
maker, app maker, buyer, system integrator, operator, and reviewer.

Do not let a long chain become an excuse. Give each party a named duty:

* The maker states intended use, limits, and test results
* The integrator tests local data, access, and failure modes
* The buyer sets contract rights, logs, audit access, and change notice
* The operator follows use limits and reports a fault
* The reviewer can reject an output and stop the tool

Legal fault still depends on the claim and place. The duty map helps a
team prevent harm before a court must assign fault.

### Apply a Stop Rule

A stop rule states when a team must pause a release or use. It should use
facts that the team can see.

Examples include a rise in crash rate, a failed safety test, harm to one
group, loss of logs, or a rollback that no longer works. The rule also
names who can stop the system and what must occur before restart.

Cost belongs in the choice after the safety floor, not in place of it.

### Try It Yourself 7.4: Set a Transit Stop Rule 🛠️

**Predict:** A bus control tool brakes too hard in a small share of
heavy-rain tests. The maker can delay launch, limit use in rain, or
launch as planned. Which path is sound?

**Run:** Apply the six cost guardrails. Then write one stop rule with a
measure, owner, and restart test.

**Explain:** In 1-2 sentences, choose a path and name the fact that most
limits your choice.

### Quick Check 7.4 ✅

1. Why can a low-likelihood event still cross a safety floor? *(Understand)*

2. Apply the six guardrails to a firm that wants to skip a security review to save money. *(Apply)*

3. How does a duty map prevent an AI supply chain from hiding responsibility? *(Analyze)*

---

## 7.5 Summary and Retrieval 💡

### Key Concepts

* **Software harm and legal liability use separate tests.** A claim needs the right party, duty, defect or breach, cause, harm, law, and contract.

* **Secure design spans the full life cycle.** NIST groups the work into preparing, protecting software, producing sound releases, and responding to flaws.

* **Release and patch speed need controls.** Small first groups, health checks, pause rights, rollback, and clear notice can limit spread.

* **Disclosure should reduce user harm.** A good process gives finders a safe report path and adapts its timing to the flaw, attack, patch, and user risk.

* **Cost does not erase a safety floor.** Sound choices test who bears risk, what is unknown, how far harm can spread, and when the team must stop.

### Key Terms

#### Section 7.1

* Software defect (bug)
* Negligence
* Product liability
* Strict liability
* Breach of warranty
* End User License Agreement (EULA)
* Software as a Service (SaaS)

#### Section 7.2

* Software quality
* Secure coding
* Secure Software Development Framework (SSDF)
* Secure by design
* Technical debt

#### Section 7.3

* Vulnerability
* OWASP Top 10
* SQL injection
* Cross-site scripting (XSS)
* Coordinated Vulnerability Disclosure (CVD)
* Patch management

#### Section 7.4

* Risk assessment
* Cost/benefit analysis
* Safety-critical system
* Safety case
* AI liability

### Retrieval Practice

Try to answer these from memory before looking back at the chapter.

1. Name the six lines in the software claim map.
2. Name the four NIST SSDF practice groups.
3. Which six guardrails make a cost/benefit analysis more ethical?

---

## 7.6 Skills Lab 7A: The AutoPilot Express Choice

**Goal:** Evaluate a known software risk and recommend a defensible release choice.

**Evidence packet:** `assets/code/chapter-07/software-liability-case.md`, a fictional case and evidence packet created for this textbook.

**Estimated time:** 90-120 minutes

### Case: Hard Braking in Monsoon Rain

**Fictional case:** TransitTech tests software for self-driving public
buses in Phoenix. The pilot has completed 50,000 trips with no grave
injury. A new contract would add 15 routes and pay $45 million over five
years.

Tomoko, a quality engineer, finds a rain defect. In 20,000 simulated
heavy-rain runs, the tool treats a large puddle as a solid object 60
times. The bus brakes hard in those runs. Ten runs, or 0.05% of all
heavy-rain runs, reach a force that may injure a standing rider.

The test does not show how many people would stand, how often a bus would
meet the same puddle and speed, or how well the result matches a bus on a
road. Dry and light-rain tests do not show the flaw.

A full fix would delay launch by 8-12 months. Added work and lost revenue
may total $9.2 million. The firm may also lose the contract.

Leaders offer three choices:

* **Launch as planned:** Keep the date and monitor for hard-brake events
* **Limit rain use:** Shift buses to a trained driver when an official monsoon warning is active
* **Delay and fix:** Redesign the sensor logic and repeat road and simulation tests

The rain limit may cut risk. Fast storms can start before an official
warning, and a driver may not be on each bus. The proposed contract does
not yet assign the cost of extra drivers or give the transit agency a
right to review safety tests.

<!-- markdownlint-disable MD029 -->

### Part 1: Foundation (Aligns with Objective 7.1)

1. Complete the six-line claim map for an injured rider. Do not decide which claim wins.
2. Compare negligence, product liability, and warranty paths. Name one missing legal or contract fact for each path.
3. Classify the bus tool as safety-critical or not. Support the choice with three case facts.

### Part 2: Application (Aligns with Objectives 7.1 and 7.2)

4. Apply the NIST SSDF areas to TransitTech. Name one control or proof missing from each area.
5. Test the rain-limit plan against the six release-gate questions. State which checks pass, fail, or lack proof.
6. Write a coordinated report and notice plan for TransitTech, the transit agency, drivers, and riders.

### Part 3: Extension (Aligns with Objectives 7.2 and 7.3)

7. Build a cost/benefit table with money, safety, trust, access, uncertainty, and risk distribution. Do not assign a dollar value to injury.
8. Write a 200-300 word board memo. Choose one option, set a stop rule, and name the evidence that would change your choice.

<!-- markdownlint-enable MD029 -->

### Questions & Analysis 🤔

1. Which missing fact has the most power to change your recommendation?
2. Who should pay for the safer choice when riders bear the main risk?

### Rubric: Skills Lab 7A

This lab is graded with the standard
[Skills Lab Rubric](../skills-lab-rubric.md): four criteria at
4 points each, 16 points total. The criteria are Technical Accuracy
and Efficiency, Output Quality, Documentation Quality, and Analysis,
Interpretation, and Response to QUESTION(s). Your instructor sets
the point weights in your course. The criteria and levels are the
same everywhere.

For CIS111, **Technical Accuracy and Efficiency** means using claim
elements, secure design controls, and risk facts without filling gaps
with guesses. **Output Quality** means that your release advice is clear,
organized, and safe for a board to use.

### Submission Guidelines

* **Length:** 800-1,200 words total across all parts
* **Format:** Submit one PDF named `skills-lab-7a-lastname.pdf`. Use clear headings for each part and label both Questions & Analysis answers.

---

## 7.7 Review Questions 🔄️

1. **Understand:** Distinguish ethical responsibility from legal liability.
2. **Apply:** Apply the NIST SSDF areas to a software update.
3. **Analyze:** Analyze how a poor rollback plan shifts risk to users.
4. **Evaluate:** When should a known defect stop a release? Defend a threshold.

## Further Reading 📖

* [NIST Secure Software Development Framework](https://csrc.nist.gov/pubs/sp/800/218/final): NIST defines secure work across the software life cycle.
* [CISA Product Security Bad Practices](https://www.cisa.gov/resources-tools/resources/product-security-bad-practices): CISA and the FBI identify high-risk choices that software makers should avoid.
* [OWASP Top 10: 2025](https://owasp.org/Top10/2025/0x00_2025-Introduction/): OWASP lists current web app risk categories and their root causes.
* [CISA Coordinated Vulnerability Disclosure Process](https://www.cisa.gov/coordinated-vulnerability-disclosure-process): CISA explains how it receives and coordinates vulnerability reports.
* [ACM Code of Ethics and Professional Conduct](https://www.acm.org/about-acm/code-of-ethics): ACM addresses system quality, risk review, and public harm.

## Looking Ahead ⏩

Chapter 8 asks what governments and professional groups should require
from technology firms. You will compare law, rules, and self-regulation.
