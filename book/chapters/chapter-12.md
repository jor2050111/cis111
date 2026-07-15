# Chapter 12: Professional Duty and Ethical Action

A vendor asks you to hide a test failure until after launch. Your manager
says the client owns the risk. A coworker says the code of ethics bars
the release. Who is right, and what should you do next?

A professional code can name a duty and support action. It cannot check
the logs, read the law, or make the choice for you. This chapter shows
how to read codes as source documents, compare their force, turn duties
into controls, and raise a concern with proof.

## Module Overview 🧭

* **Estimated time:** 5-6 hours (reading + practice + Skills Lab)
* **Prerequisites:** Chapters 1-11
* **Deliverables:** Try It Yourself activities, Quick Checks, Skills Lab 12A

## Learning Objectives 🎯

By the end of this chapter, you will be able to:

* **12.1 (Analyze):** Analyze an ACM, IEEE, or ISC2 code duty through source, scope, priority, enforcement, and proof
* **12.2 (Evaluate):** Evaluate a code, license, certification, or escalation path for its strengths, limits, and effects
* **12.3 (Create):** Create a capstone recommendation that joins ethical frameworks, professional duties, law, technical proof, controls, and review

### This chapter aligns with the following Course Learning Outcomes

* **CLO XVII.** Critique professional codes of ethics for Information Technology professionals.

---

## 12.1 Read Each Code as a Source Document

A **code of ethics** states duties for a group or role. It may guide a
choice, support a complaint, or set a condition of membership. It is not
the same as a law, contract, job policy, or technical standard.

Do not rely on a quote from a slide or blog. Open the current code and
record what it covers.

Use this six-line code record:

1. **Source and date:** Who issued the code, and which version is current?
2. **People and work:** Who must or may follow it?
3. **Duty:** Which exact principle or canon fits the case?
4. **Priority and conflict:** Does the code rank duties or explain conflicts?
5. **Enforcement:** Who can receive a complaint, find a violation, and impose a result?
6. **Proof and remedy:** What facts are needed, and what action would reduce harm?

The record prevents two common errors. One is treating a broad value as
a full answer. The other is claiming a code can punish a person when the
issuer has no power over that person.

### Apply the ACM Code

The **ACM Code of Ethics and Professional Conduct** is meant to guide
computing professionals. Its four sections cover:

* Broad duties such as public good, avoiding harm, honesty, fairness, privacy, and respect for creative work
* Professional duties such as quality, competence, review, risk checks, and approved access
* Leadership duties for healthy work, public good, and systems that support ethical action
* Compliance with the code

The code applies beyond narrow software tasks. It asks a professional to
consider all people affected by a system.

ACM also has a formal enforcement process for covered members and award
holders. A complaint must name facts, proof, and the code parts at issue.
The process can include review, investigation, a finding, a sanction, and
an appeal. Possible results range from a letter or remedy to suspension
or expulsion.

The [ACM Code](https://www.acm.org/about-acm/code-of-ethics) and
[ACM enforcement process](https://www.acm.org/about-acm/code-of-ethics-enforcement-procedures)
should be read together when enforcement matters.

### Apply the IEEE Code

The **IEEE Code of Ethics** guides IEEE members. Its current form groups
ten commitments under three broad duties:

* Act with integrity, sound conduct, and care in professional work
* Treat people fairly and with respect, reject harassment and bias, and avoid harm
* Help coworkers follow the code and protect good-faith reporting from retaliation

The ten points address public safety, conflicts, honest claims, bribery,
the effects of technology, competence, fair treatment, harassment, false
harm, and support for others who follow the code.

The code is short. That makes it easy to recall but leaves more work for
the case record. "Protect safety" does not state which test must pass or
who may stop a release.

IEEE's article on its
[approved code revision](https://spectrum.ieee.org/board-of-directors-approves-revisions-to-the-ieee-code-of-ethics)
provides the current grouped text and ten commitments.

### Apply the ISC2 Code

The **ISC2 Code of Ethics** applies to ISC2 members and people who hold
its credentials, such as CISSP. It lists four mandatory canons in
priority order. In plain terms, they require a professional to:

1. Protect society, public trust, and key systems.
2. Act with honor, honesty, fairness, care, and respect for law.
3. Give principals diligent and competent service.
4. Support and protect the profession.

The order helps with a conflict. Service to an employer or client does
not outrank the duty to society.

ISC2 has an ethics complaint process. The people allowed to complain can
depend on the canon. A peer review can lead to action, including loss of
a credential. The code does not give a member a free right to break a
law, reveal protected data, or skip sound process.

The [ISC2 ethics page](https://www.isc2.org/Ethics) states the canons,
complaint scope, and possible result.

**Worked code record:** A security lead learns that a client portal has
a flaw that exposes account data. The manager wants to wait until a sales
event ends. The lead holds a CISSP.

The public-trust canon comes before service to the employer. That duty
supports prompt containment and a fact-based notice review. It does not
prove which notice law applies or permit the lead to send client data to
a personal account.

The lead should preserve proof through approved systems, state the harm,
ask for a written risk choice, and use the response path. The code helps
name the duty. The incident plan, law map, and evidence set the action.

### Try It Yourself 12.1: Compare Two Duties 🛠️

**Predict:** An engineer is told to approve a release that passed the
business test but failed an accessibility test. Which code gives the
clearest duty?

**Run:** Complete the six-line code record for the ACM and IEEE codes.
Use a current source for each.

**Explain:** In 1-2 sentences, name the stronger duty and the control it
should require.

### Quick Check 12.1 ✅

1. What six facts belong in a code record? *(Understand)*

2. How does the ISC2 canon order help resolve a client conflict? *(Apply)*

3. Why must a team read a code and its enforcement process together? *(Analyze)*

---

## 12.2 Compare Scope, Force, and Gaps

Codes can share a value yet guide action in different ways. Compare more
than wording.

Use five critique tests:

1. **Scope:** Does the code reach the person, role, system, and harm?
2. **Priority:** Does it rank duties or explain how to resolve a conflict?
3. **Specificity:** Can a team turn the duty into a control and test?
4. **Enforcement:** Is there a fair complaint, proof, finding, result, and appeal path?
5. **Revision:** Does the issuer review the code as work and harm change?

### Compare the Three Codes

| Test | ACM | IEEE | ISC2 |
| --- | --- | --- | --- |
| Main reach | Computing work | Engineering and technical work | Cybersecurity roles and credentials |
| Form | Four sections with guidance | Three broad duties and ten points | Four ranked canons |
| Conflict help | Context and public good | Broad duty language | Stated priority order |
| Complaint force | Formal ACM process for covered people | IEEE conduct rules apply to members and activities | Ethics complaint and peer review |
| Strong use | Full system and social-impact review | Clear safety, honesty, fairness, and coworker duties | Security trust, client conflict, and credential duty |

This table is a start, not a score. A short code can guide a clear case.
A detailed code can still leave a hard conflict open.

### Find What a Code Does Not Supply

A code may name "avoid harm" without supplying:

* A test threshold or release metric
* A law or contract map
* A data retention rule
* A person with stop authority
* A safe report channel
* A remedy for people already harmed
* A way to include people outside the profession

Those are gaps in the decision system, not always defects in the code.
A code cannot contain a full rule for each tool and country. The team can
join it with standards, law, risk records, and local controls.

### Distinguish Guidance from Enforcement

An **aspirational code** states values and conduct a group seeks. An
**enforceable code** also has a process that can impose a result on a
person within its scope.

Enforceable does not mean government law. A professional group may
suspend membership or revoke a private credential. It cannot send a
person to jail or block all work in a field unless law grants that power.

Good enforcement needs **due process**, a fair notice and response path.
Ask:

* Who may file a complaint?
* What proof and time limit apply?
* Who checks the claim and conflicts of interest?
* Can the person respond?
* Which findings and results are allowed?
* Is there an appeal?
* How does the process guard against retaliation?

Weak process can turn a sound code into a tool for rank or revenge.

**Worked code critique:** A city buys an AI tool that ranks housing
inspections. The contract team follows no professional group. The vendor
engineer is an ACM member. The city wants the model kept secret.

The ACM code reaches the engineer's conduct, but ACM cannot bind the city
through membership. The public-good, fairness, honesty, and risk duties
support testing and clear limits. The contract and public law must set
rights for the city and residents.

A strong control would require test results by building type and area,
an appeal, audit access, and a stop rule. A code complaint may address
member conduct. It will not replace those product controls.

### Try It Yourself 12.2: Critique a Short Code 🛠️

**Predict:** A firm adopts one rule: "Build technology for good." Is that
enough to guide a launch?

**Run:** Apply all five critique tests. Add the complaint, proof, appeal,
and retaliation facts.

**Explain:** In 1-2 sentences, name the largest gap and one fix.

### Quick Check 12.2 ✅

1. Distinguish an aspirational code from an enforceable code. *(Understand)*

2. Apply the specificity test to the duty to avoid harm. *(Apply)*

3. Why can a formal complaint process still be unfair? *(Evaluate)*

---

## 12.3 Test Licensing, Certification, and Accountability

Professional duty can also come from a government license or a private
credential. These are not the same.

**Professional licensing** is government approval to perform a protected
task or use a protected title. Law sets the scope, entry rules, and
discipline process.

**Professional certification** is a credential from a private group. It
shows that a person met the issuer's stated test. The credential may also
require work history, ongoing learning, and a code of ethics.

A certificate does not prove skill in every tool or role. A license does
not prove that each act is sound. Both need current scope and proof.

### Apply a Seven-Line Scope Test

Before proposing a license for IT work, ask:

1. **Protected task:** Which exact act or title would the law control?
2. **Harm threshold:** What public harm is common or severe enough to justify the limit?
3. **Competence:** Which skill, test, experience, and ongoing learning are needed?
4. **Regulator:** Who grants, checks, limits, and removes the license?
5. **Access and equity:** Who may be shut out by cost, time, language, or degree rules?
6. **Alternatives:** Could a firm license, product rule, audit, code, or narrow task limit work better?
7. **Review:** How will the rule change as tools and harms change?

"License all IT workers" fails the first test. Help desk work, cloud
design, health software, security tests, and AI model review involve
different tasks and risks.

A narrow rule may fit a high-harm task better. It could require a named
professional to approve a safety case while leaving other work open to
many entry paths.

### Audit a Certification Claim

Use a credential card:

* Issuer and current credential name
* Tested job or skill scope
* Exam, work, and identity requirements
* Renewal and ongoing-learning duties
* Code and complaint process
* Public status check
* Limits on what the credential proves

The **CISSP** credential, for example, ties certification to the ISC2
Code of Ethics. A knowing code breach may lead to peer review and loss of
the credential. That creates one form of professional accountability.

The employer still must check role fit and current skill. A valid CISSP
does not by itself prove that its holder can review a medical model,
write safe code in each language, or lead each incident.

### Build Accountability around the Work

Accountability should not rest on one person's title. Build an
**accountability record** for high-impact work. Record:

* The claim and affected people
* The qualified owner and reviewer
* The tests and pass threshold
* The code, law, contract, and standard used
* The approval, exception, and stop authority
* The logs and version released
* The remedy and next review

This record allows a colleague to see what happened and why. It also
keeps a group from using a credential as a shield for weak proof.

**Worked scope test:** A state wants to require a license for any person
who edits health software. The goal is patient safety. The task, though,
includes text changes, network setup, clinical rules, and device code.

The proposal is too broad. The state could first name the acts that can
directly change diagnosis, dose, or treatment. It could require an
approved safety owner, tested competence, review, and a report path for
those acts.

It should also test access effects. A high fee or degree rule may block
skilled people without improving patient safety. Product and firm duties
may guard some risks better than a personal license.

### Try It Yourself 12.3: Test an AI License Plan 🛠️

**Predict:** A state plans to license every person who works on AI. Will
that rule protect the public?

**Run:** Apply the seven-line scope test. Compare a broad license with a
narrow approval role for high-impact uses.

**Explain:** In 1-2 sentences, choose a scope and name the public proof it
should require.

### Quick Check 12.3 ✅

1. Distinguish professional licensing from certification. *(Understand)*

2. What does a credential card prove and leave open? *(Apply)*

3. When might a narrow task license work better than a field-wide license? *(Evaluate)*

---

## 12.4 Turn Ethical Concern into Safe Action

A code has value when it changes a choice. The move from duty to action
needs proof, controls, authority, and a remedy.

### Join a Code Duty to a Control

Use a six-column duty-to-control record:

| Field | Question |
| --- | --- |
| Duty | Which code, principle, or canon applies? |
| System claim | What does the team claim the system will do? |
| Proof | Which test, log, source, or person supports the claim? |
| Control | What prevents, detects, limits, or repairs harm? |
| Authority | Who may approve, pause, reverse, or report the act? |
| Remedy | How can an affected person get notice, appeal, repair, or support? |

For AI work, the voluntary
[NIST AI Risk Management Framework](https://airc.nist.gov/airmf-resources/airmf/)
adds four functions:

* **Govern:** Set policy, roles, risk limits, and accountability.
* **Map:** Set the use context, people, impacts, and risk.
* **Measure:** Test function, limits, error, bias, and uncertainty.
* **Manage:** Rank risk, act, monitor, report, and improve.

These functions are not four one-time steps. The team should keep using
them while the system is in service.

### Use an Eight-Step Concern Path

When you think a task may cause harm:

1. **State the concern:** Name the act, people, harm, and time pressure.
2. **Separate fact from inference:** List proof, source, and uncertainty.
3. **Name the duty:** Cite the code, law, contract, policy, or role.
4. **Reduce immediate harm:** Use the stop, containment, or safe-work rule you are allowed to use.
5. **Offer a control:** Give a test, limit, repair, or safer option.
6. **Use the report path:** Contact the named manager, safety owner, ethics office, legal team, union, regulator, or other proper channel.
7. **Protect people and proof:** Keep records lawfully. Do not take data or reveal secrets without a valid right.
8. **Record the choice:** State who decided, why, what remains open, and when to review.

Internal reporting may be unsafe or futile in some cases. A manager may
be part of the harm. Delay may put people at once-in-time risk. Law may
require a report to a regulator or emergency service.

Do not assume that public disclosure is always protected. Whistleblower,
trade-secret, privacy, contract, and security rules vary. Seek qualified
advice when the path is unclear. If there is an urgent threat to life or
safety, use the emergency path that fits the case.

### Keep Human Review Meaningful

"A human is in the loop" does not prove oversight. A reviewer needs:

* The time and context to review the case
* Access to the source facts and model limits
* Skill for the type of choice
* Power to change or stop the result
* A record of the reason
* A way to repair an error

Low-impact acts may be safe to automate. High-impact acts need controls
that match the harm. The professional duty is to design the right form
of review, not to add a person as a label.

**Worked concern path:** A hiring tool rejects applicants after a voice
test. The vendor reports 91% total accuracy. It gives no disability,
accent, language, or job-validity results. The launch owner wants to use
the tool for all open roles.

The concern is not that AI is always wrong. The proof does not support
the planned scope. ACM fairness, harm, honesty, and risk duties apply.
IEEE fair-treatment and honest-claim duties also fit.

The team can pause auto-rejection, run role and group tests, give notice,
add an appeal, and set a stop threshold. If the owner rejects those
controls, the reviewer should use the next report path and record the
choice without copying applicant data to a personal system.

### Try It Yourself 12.4: Raise a Safety Concern 🛠️

**Predict:** A manager asks you to remove a failed test from a release
report because the issue affects few users. Should you comply?

**Run:** Apply the duty-to-control record and all eight concern steps.
Name any immediate stop rule and safe report path.

**Explain:** In 1-2 sentences, state your next act and the proof you will
preserve.

### Quick Check 12.4 ✅

1. Name the four NIST AI RMF functions. *(Understand)*

2. Apply a code duty to one testable control. *(Apply)*

3. What makes human review meaningful instead of nominal? *(Evaluate)*

---

## 12.5 Summary and Retrieval 💡

### Key Concepts

* **Read the source.** Record the code issuer, scope, duty, priority, enforcement, proof, and remedy.

* **Compare force, not just words.** A code's value depends on scope, conflict help, specificity, process, and revision.

* **Keep private enforcement separate from law.** A group may discipline a member or revoke a credential within its scope.

* **Test licensing with a narrow task.** Name the harm, competence, regulator, access effects, alternatives, and review.

* **Audit credential claims.** Record what the credential tested, its current status, code, renewal, and limits.

* **Turn duty into action.** Join the code to proof, a control, authority, a report path, and a remedy.

* **Raise concerns safely.** Keep facts apart from inference, protect people and proof, and use the right channel.

### Key Terms

#### Section 12.1

* Code of ethics
* ACM Code of Ethics
* IEEE Code of Ethics
* ISC2 Code of Ethics
* Canon

#### Section 12.2

* Aspirational code
* Enforceable code
* Due process

#### Section 12.3

* Professional licensing
* Professional certification
* CISSP
* Accountability record

#### Section 12.4

* AI ethics
* NIST AI Risk Management Framework
* Human oversight (AI)
* Responsible AI

### Retrieval Practice

Try to answer these from memory before looking back at the chapter.

1. Name the six lines in the code record.
2. Name five tests used to critique a code.
3. Name four steps in the concern path.

---

## 12.6 Skills Lab 12A: The CivicLink Benefits Decision

**Goal:** Create a capstone recommendation that joins ethical frameworks, professional codes, law, technical proof, controls, and remedies.

**Evidence packet:** `assets/code/chapter-12/capstone-scenario-builder.md`, a fictional case and evidence packet created for this textbook.

**Estimated time:** 120-150 minutes

### Case: Launch, Narrow Pilot, or Pause

**Fictional case:** Marston County plans to launch CivicLink, an online
tool that helps residents apply for housing, food, and health benefits.
NovaPath built the tool under a county contract.

CivicLink checks forms, ranks fraud risk, and drafts a benefit choice.
A county worker approves or changes the draft. The review screen gives
the worker 45 seconds before the next case appears.

The vendor reports 92% total accuracy. A county test finds a 7% false-
flag rate for standard English web forms. The rate is 22% for translated
forms and 24% for forms completed with a screen reader. The vendor calls
those groups too small for a firm result.

The system keeps identity, health, housing, device, and location data for
10 years. The contract says NovaPath may use de-identified records to
improve its products. It does not state the method or re-identification
test.

The public notice says that a county worker decides each case. It does
not name the AI rank, 45-second limit, vendor use, or appeal path. The
county has no process for a resident to correct a bad data link.

An engineer sends leaders a memo about the test gaps. She cites the ACM
Code and asks for a limited pilot. Her manager removes her from the
launch meeting and tells her not to put more concerns in writing.

A stolen vendor admin password was also used to open 300 test records.
The team reset the password but did not use MFA, keep an evidence log, or
review all account actions. The public launch is set for 30 days.

The county may launch for all residents, run a narrow pilot with new
controls, or pause until the gaps close.

<!-- markdownlint-disable MD029 -->

### Part 1: Foundation (Aligns with Objective 12.1)

1. Build a fact, inference, and open-question table for the case. Name the proof needed for each open question.
2. Complete the six-line code record for ACM, IEEE, and ISC2. State which people and acts each code can reach.
3. Map at least five case issues to tools from earlier chapters. Include privacy, AI risk, worker voice, security, and accessibility or fairness.

### Part 2: Application (Aligns with Objectives 12.1 and 12.2)

4. Apply two ethical frameworks. State where their recommendations agree and conflict.
5. Apply all five code critique tests. Select the code that gives the strongest guidance and state its largest gap.
6. Build a duty-to-control record for false flags, data use, human review, worker retaliation, and the admin-account event.

### Part 3: Extension (Aligns with Objectives 12.2 and 12.3)

7. Create an eight-control release plan. Include tests, notice, consent or legal basis, access, retention, human review, appeal, security, and a stop rule.
8. Write a 400-500 word memo. Choose full launch, narrow pilot, or pause. Address the strongest counterclaim and name the proof that would change your choice.

<!-- markdownlint-enable MD029 -->

### Questions & Analysis 🤔

1. Which professional duty has the most force in this case, and why?
2. Which control best protects a resident with the least power?

### Rubric: Skills Lab 12A

This lab is graded with the standard
[Skills Lab Rubric](../skills-lab-rubric.md): four criteria at
4 points each, 16 points total. The criteria are Technical Accuracy
and Efficiency, Output Quality, Documentation Quality, and Analysis,
Interpretation, and Response to QUESTION(s). Your instructor sets
the point weights in your course. The criteria and levels are the
same everywhere.

For CIS111, **Technical Accuracy and Efficiency** means matching each
ethical, code, legal, and technical claim to the case proof and book
tool. **Output Quality** means that the release plan and memo are clear,
consistent, fair, evidence-based, and ready for county review.

### Submission Guidelines

* **Length:** 1,500-2,000 words total across all parts
* **Format:** Submit one PDF named `skills-lab-12a-lastname.pdf`. Use clear headings for each part and label both Questions & Analysis answers.
* **Sources:** Cite each professional code and any outside source used.

---

## 12.7 Review Questions 🔄️

1. **Understand:** Compare the scope of the ACM, IEEE, and ISC2 codes.
2. **Apply:** Turn one code duty into a testable release control.
3. **Evaluate:** Critique a broad plan to license all IT work.
4. **Create:** Draft the first three steps for raising a supported concern.

## Further Reading 📖

* [ACM Code of Ethics and Professional Conduct](https://www.acm.org/about-acm/code-of-ethics): ACM states broad, professional, leadership, and compliance duties.
* [ACM Code Enforcement Process](https://www.acm.org/about-acm/code-of-ethics-enforcement-procedures): ACM explains complaints, proof, findings, sanctions, and appeals.
* [IEEE Code of Ethics](https://spectrum.ieee.org/board-of-directors-approves-revisions-to-the-ieee-code-of-ethics): IEEE provides the approved grouped code and ten commitments.
* [ISC2 Code of Ethics](https://www.isc2.org/Ethics): ISC2 states four canons and its complaint scope.
* [NIST AI Risk Management Framework](https://airc.nist.gov/airmf-resources/airmf/): NIST explains Govern, Map, Measure, and Manage.

## Course Conclusion: Where You Go from Here

The book ends here. The duty does not.

New tools will change the facts, risks, and rules. The method remains:
name the people and harm, check the source, test the claim, record the
choice, and build a remedy. That is how ethical judgment becomes
professional action.

Carry the method into every course and job that follows. Read one
security or ethics story each week and run it through the five moves.
When a workplace policy crosses your desk, you know how to question
it. When an incident lands, you know how to act. The field needs
professionals who can do both.
