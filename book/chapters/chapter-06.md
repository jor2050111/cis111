# Chapter 6: Healthcare IT Ethics

In February 2024, a cyberattack stopped key services at Change
Healthcare. Pharmacies had trouble checking benefits. Clinics could not
send claims or receive payments. One tech failure affected care
across the United States.

The harm did not end when systems came back online. In July 2025,
Change Healthcare told HHS that the breach had affected about
[192.7 million people](https://www.hhs.gov/hipaa/for-professionals/special-topics/change-healthcare-cybersecurity-incident-frequently-asked-questions/index.html).
The event linked privacy, data safety, money, and patient access. IT choices
shaped each part of the outcome.

This chapter gives you a method for those choices. You will test who a
health data rule covers, map where data moves, and select safeguards.
You will also assess mobile tools, care systems, telehealth, and AI.

## Module Overview 🧭

* **Estimated time:** 4-5 hours (reading + practice + Skills Lab)
* **Prerequisites:** Chapters 1-5
* **Deliverables:** Try It Yourself activities, Quick Checks, Skills Lab 6A

## Learning Objectives 🎯

By the end of this chapter, you will be able to:

* **MLO-6.1 (Understand):** Explain how HIPAA scope, privacy rules, security safeguards, and breach duties shape health data work
* **MLO-6.2 (Apply):** Apply ethical tests to mobile, wireless, care, and telehealth choices
* **MLO-6.3 (Analyze):** Analyze an AI health tool for patient risk, bias, privacy, and human oversight

### This chapter aligns with the following Course Learning Outcomes

* **CLO VI.** Analyze the major ethical challenges of operating in a healthcare environment using mobile and wireless technologies.

---

## 6.1 HIPAA Scope, Privacy, and Security

Health records can expose a diagnosis, medicine, test result, or care
plan. A leak can cause fear, fraud, or stigma. Poor access controls can
also delay care. Sound health IT must protect privacy without blocking
safe and timely treatment.

### Start with Scope

The **Health Insurance Portability and Accountability Act (HIPAA)**
sets federal rules for certain health information. HIPAA does not cover
every person, app, or file that contains a health fact.

A **covered entity** is one of these groups:

* A health plan
* A healthcare clearinghouse
* A healthcare provider that conducts certain standard transactions in electronic form

A **business associate** does certain work for a covered entity and
handles protected health information. A billing firm, cloud host, or IT
vendor may fill this role. The parties need a written business associate
agreement when HIPAA requires one.

The role and work link matter. A cloud firm does not become a business
associate only because it can store data. Its service, client, contract,
and access to health data help decide its status. HHS
gives [current business associate guidance](https://www.hhs.gov/hipaa/for-professionals/privacy/guidance/business-associates/index.html).

### Identify PHI and ePHI

**Protected Health Information (PHI)** is health information that can
identify a person and is held or sent by a covered entity or business
associate. **Electronic PHI (ePHI)** is PHI in electronic form.

The same blood pressure reading can have one legal status at a clinic
and another in an app. A clinic record may be PHI. A reading stored only in
a personal fitness app may fall outside HIPAA. Other federal or state
rules may still apply.

HIPAA has two paths to de-identify PHI. An expert may find that the risk
of linking the data to a person is small. A group may use the Safe Harbor
path and remove a set list of details. It must not know that the data
left behind can name a person. Removing a name alone is not enough.
HHS explains both methods in its
[de-identification guidance](https://www.hhs.gov/hipaa/for-professionals/special-topics/de-identification/index.html).

### Apply the Privacy Rule

The **Privacy Rule** governs many uses and shares of PHI. It also
gives people rights over records in a designated record set. Those
rights include access, a request to amend a record, and an accounting of
certain shares. Each right has limits and steps.

The **minimum necessary standard** asks a covered entity to take reasonable
steps to limit many uses, shares, and requests. The
limit does not apply to every use. For example, it does not apply to a
share to a provider for care. A sound access plan starts
with job duties, not curiosity or status.

Suppose a billing worker needs a patient name, service code, and plan
number. The worker may not need full therapy notes. Role-based access
can make that difference part of the system.

### Apply the Security Rule

The **Security Rule** protects the confidentiality, integrity, and
availability of ePHI. It groups safeguards into three areas:

* **Administrative safeguards:** risk checks, assigned duties, training, and plans for an event
* **Physical safeguards:** controls for a site, work area, device, and media
* **Technical safeguards:** controls for access, logs, data integrity, identity, and data sent on a network

The rule requires each standard. Some implementation details are
"required" and others are "addressable." Addressable does not mean that
a group may ignore the issue. The group must use the measure when it is
reasonable and appropriate. If it chooses another measure, it must
record why and protect the same goal.

This risk-based plan makes local facts key. A small clinic and a
large hospital may use other tools. Both must assess risk and protect
ePHI at a reasonable and appropriate level.

### Respond to a Breach

The **Breach Notification Rule** applies after a breach of unsecured PHI.
An improper use or share is presumed to be a breach unless a risk check
shows a low chance that PHI was exposed. The rule also
has narrow exceptions.

Notice duties depend on the facts. A covered entity must tell affected
people without unreasonable delay and no later than 60 days after it
discovers a reportable breach. It must also tell HHS. The timing for
HHS depends on whether the breach affects at least 500 people. Media
notice applies when a breach affects more than 500 residents of a state
or jurisdiction.

Do not decide from the record count alone. Ask whether the data was PHI,
whether it was secured, what occurred, and whether an exception or risk
risk check applies. HHS lists the steps in its
[Breach Notification Rule guidance](https://www.hhs.gov/hipaa/for-professionals/breach-notification/index.html).

Use one short work log when you change a health IT system:

* **Task:** State the care or work need in plain words
* **Data:** List the least data the task needs
* **Role:** Name who may view, add, change, or send the data
* **Rule:** State which law, policy, or care rule guides the task
* **Guard:** Name the lock, log, check, or staff step that cuts risk
* **Proof:** State how the team will know that the guard works

For example, a clinic may give help desk staff a masked view of a chart.
The view can show the system error but hide the test result. An audit log
can show who used the view and when. This plan meets the work need with
less data at risk.

### Try It Yourself 6.1: Limit an Accidental View 🛠️

**Predict:** While fixing a clinic printer, you see a lab result for a
person you know. You did not need the result for your task. What should
you do next?

**Run:** Check your job need, the least data needed, the clinic's
incident path, and the risk of further disclosure.

**Explain:** In 1-2 sentences, state the next action and one action you
must avoid.

### Quick Check 6.1 ✅

1. Why does a health fact in a fitness app not always count as PHI? *(Understand)*

2. How do the Privacy Rule and Security Rule address separate parts of data care? *(Understand)*

3. A vendor hosts ePHI for a hospital. Name two facts that help test whether the vendor is a business associate. *(Apply)*

---

## 6.2 Mobile Health, Wearables, and BYOD

Mobile health tools collect data outside a clinic. A phone can record
movement, heart rate, sleep, medicine use, or symptoms. Wireless devices
can send those facts to a patient, provider, vendor, or data broker.

The ethical question starts with a data map: what is collected, where it
goes, who can use it, and when it is deleted.

### Do Not Use One Label for Every App

**Mobile health (mHealth)** includes health work done through phones,
wearables, sensors, and wireless services. A **consumer health app** may
help a person track sleep or meals. A regulated medical device may help
diagnose or treat a condition. FDA status and HIPAA status answer
separate questions.

The FDA looks at a product's medical function and risk. HIPAA looks at
the parties, their roles, and the data relationship. A regulated device
does not enter HIPAA only because the FDA reviews it. A simple app may
enter HIPAA when its developer acts as a business associate.

HHS, the FTC, FDA, and ONC offer a
[mobile health app tool](https://www.hhs.gov/hipaa/for-professionals/special-topics/health-apps/index.html)
to help developers identify federal rules that may apply.

### Check Rules Beyond HIPAA

Some health apps fall outside HIPAA but still face legal duties. The
FTC's **Health Breach Notification Rule (FTC)** covers certain vendors of
personal health records and related firms. Its 2024 update makes clear
that many health apps and connected devices can fall within the rule.

For a covered firm, a breach can include an outside attack or an
unauthorized disclosure by the firm. The firm may need to notify people,
the FTC, and sometimes the media. The FTC Act and state laws may also
govern a claim or data practice.

This closes part of the old gap, but it does not answer each ethics
question. A practice can meet a notice rule and still collect too much
data or use consent that few people can grasp.

### Test Consent and Data Use

**Informed consent** requires a clear explanation, a fair choice, and a
person who can decide. A long privacy policy is weak proof that a person
understood a sensitive use.

Use five questions:

1. What data does the tool collect?
2. Which use does the person expect?
3. Which other parties receive the data?
4. Can the person refuse without an unfair cost or loss?
5. Can the person withdraw and request deletion?

A wearable from an employer raises extra pressure. A cash reward can
make a program feel less voluntary to a low-paid worker. Small group
reports may also expose one person even when names are removed.

### Control BYOD Risk

**Bring Your Own Device (BYOD)** lets workers use personal phones or
tablets for work. It can speed communication and remote access. It also
mixes private life, firm control, and patient data on one device.

A sound BYOD design may use these controls:

* A managed work container that separates firm data
* Strong sign-in and short lock times
* Encryption and secure network links
* Remote removal of work data
* Limits on downloads, screenshots, and local storage
* A fast process for lost devices

Map each mobile data flow before launch. Start with the sensor. Follow
the data through the phone, network, cloud, and report. At each stop,
write who can read it and why. Mark each copy and backup. Add the date
when each copy should be erased.

This map can expose a hidden risk. A clinic may protect the phone app but
miss a vendor log that keeps full IDs. A firm may hide names in a report
but use a team so small that a boss can guess each worker. The map turns
a broad promise into facts that a team can test.

The group should state what its management tool can see. A worker should
know whether the group can view location, photos, apps, or only the work
container. Security does not excuse hidden worker monitoring.

### Case Study 6.1: The Small Group Report 📋

**Fictional case:** Midland Manufacturing offers a wellness watch. A
worker who joins saves $50 each month on health coverage. The watch
tracks steps, heart rate, sleep, and stress.

Leaders say that managers will see only group results. Yet one report
breaks sleep data into teams of four. A supervisor then tells Darnell to
"get more sleep." Darnell never shared his result with the supervisor.

The vendor also uses de-identified data for product research. The notice
does not name its research partners or a deletion date.

The case raises four tests. Was the choice free? Could a manager infer a
person's data? Did the notice state each use? Did the firm collect only
what it needed for the program?

Do not assume HIPAA covers the watch. First test the parties and their
roles. Then check the FTC rule, other laws, the contract, and the ethics
of the design.

### Try It Yourself 6.2: Map a Wearable Program 🛠️

**Predict:** Should Midland keep the program, change it, or end it?

**Run:** Draw a four-step data map from the watch to the final report.
Apply the five consent questions at each transfer.

**Explain:** In 1-2 sentences, choose one required change and name the
person it protects.

### Quick Check 6.2 ✅

1. Why do FDA status and HIPAA status answer separate questions? *(Understand)*

2. How can a report about four workers expose a person without listing a name? *(Apply)*

3. A clinic permits BYOD. Choose two device controls and explain the patient risk each one reduces. *(Apply)*

---

## 6.3 Clinical Systems, Telehealth, and Patient Safety

Care systems do more than store data. They shape orders, warnings,
and care choices. A slow screen can delay medicine. A weak alert can hide
a danger. A broken interface can block a patient from care.

### EHRs and Interoperability

An **Electronic Health Record (EHR)** holds digital care records.
It may contain notes, test results, medicines, allergies, and orders.
**Interoperability** means that other systems can share and use data.

Data exchange can prevent a repeated test or show an allergy during an
emergency. Poor exchange can split one patient's story across systems.
More exchange also creates more access points. IT teams must protect the
data while keeping it available to the right care team.

Useful controls include role-based access, audit logs, data checks, and
an emergency access process. Emergency access should not become a hidden
shortcut. A system can log the reason, user, time, and records viewed.

### CDS, CPOE, and Alert Fatigue

**Clinical Decision Support (CDS)** gives timely, patient-specific
facts that can aid a care choice. A **Clinical Decision Support
System (CDSS)** may show a drug warning, dose guide, or care rule. It
supports a choice. It does not make every choice for the clinician.

**Computerized Provider Order Entry (CPOE)** lets a provider enter an
order for medicine, a test, or treatment. It can remove handwriting
errors and check a dose. Poor menus, defaults, or copied text can create
new errors.

**Alert fatigue** occurs when users see so many warnings that they stop
giving each one due care. More alerts do not always mean more safety. A
team should track which alerts fire, which users override, and which
alerts prevent harm. It should remove weak alerts and test high-risk
ones with care staff.

ONC explains that [CDS must fit the care workflow](https://healthit.gov/clinical-quality-and-safety/clinical-decision-support/).
This is both a design rule and an ethics rule. A tool that interrupts the
wrong person at the wrong time may fail the patient it was meant to help.

### Telehealth Access and Privacy

**Telemedicine** provides care through remote technology. It can reduce
travel and connect a patient with a distant specialist. It can also
widen the **digital divide** when a patient lacks broadband, a private
room, a usable device, or help with the platform.

A fair telehealth plan asks:

* Does the patient have an accessible way to join?
* Can the patient speak without being overheard?
* What can the remote visit assess well?
* When must the provider move to in-person care?
* What backup works if the link fails?

Cross-state practice also requires a current license check. State rules
vary. A provider may need a full license, a compact privilege, a
registration, or another state path. HHS advises providers to verify the
patient's location and consent before the visit. Its
[cross-state licensure guide](https://telehealth.hhs.gov/licensure/licensing-across-state-lines)
lists common paths.

Use a safety loop for each care tool. First, watch how the team works
without the tool. Next, test the tool with staff and people who use the
care site. Track close calls, wrong clicks, slow steps, and workarounds.
Then fix the rule or screen and test again.

The loop should include a stop rule. A team may stop a drug alert if it
fires at the wrong time or hides a high-risk warning. A clinic may stop
a video visit when the link makes a safe exam hard. A clear stop rule
gives staff the right to protect the patient.

### Try It Yourself 6.3: Design a Fair Remote Visit 🛠️

**Predict:** A patient lives 90 miles from a heart specialist. The
patient has slow internet and shares a home with family. Is a video visit
the best first choice?

**Run:** Test access, privacy, care limits, patient choice, and a
backup plan. Compare video, phone, a local clinic room, and travel.

**Explain:** In 1-2 sentences, choose an option and state one condition
that would change your choice.

### Quick Check 6.3 ✅

1. How can interoperability improve care and increase security risk? *(Understand)*

2. Why can a high number of low-value alerts make a care system less safe? *(Analyze)*

3. A patient cannot use a video platform without help. Name two ways a provider can preserve access and choice. *(Apply)*

---

## 6.4 AI in Healthcare: Evidence and Accountability

AI can sort images, predict risk, draft notes, or flag a change in a
patient's condition. A useful model may help a care team act sooner. A
poor model may hide risk behind a confident score.

The right question is not, "Does the system use AI?" Ask whether the
system is fit for its stated use, patient group, site, and workflow.

### Test Intended Use and Performance

**AI-assisted diagnostics** use AI to help check care data. A
result may support a clinician who reads an image or reviews a risk
score. The team must know what the tool was built to do and what it was
not built to do.

A **false negative** misses a condition that is present. A **false
positive** flags a condition that is not present. These errors cause
harm patients in separate ways. A missed case can delay care. A false alarm can cause
fear, tests, cost, and treatment risk.

Overall accuracy can hide a weak subgroup result. Ask for sensitivity,
specificity, false result rates, and confidence ranges. Ask for results
across the patient groups who will receive care. A local test can reveal
whether a tool fits the site's data and workflow.

### Find Bias in the Full System

**Algorithmic bias** can enter through data, labels, features, goals, or
deployment. A model may underrepresent a group. It may use cost as a
weak stand-in for health need. It may work in one hospital and fail in
another.

A [2019 study in *Science*](https://pubmed.ncbi.nlm.nih.gov/31649194/)
examined a care-management algorithm that used health spending to
predict need. Black patients with the same level of illness had lower
spending than White patients. The proxy caused the system to rate many
Black patients as less in need of added care.

The lesson reaches beyond one model. Test the target that the model
learns. Then test the system after it enters local work.

### Build Human Oversight and Change Control

**Human oversight (AI)** means more than placing a person after a model.
The reviewer needs time, skill, authority, and useful evidence. The
reviewer must be able to reject an output and record why.

Assign duties across the full system:

* The vendor states the intended use, limits, data basis, and change plan
* The health group checks the contract, local fit, security, and workflow
* Care leaders define when a person must review or override a result
* IT teams log versions, inputs, outputs, access, and failures
* A governance group reviews subgroup results, incidents, and appeals

Do not make a final legal liability claim from this list. The law can
depend on the product, contract, license, use, and place. The list maps
ethical and operating responsibility.

The FDA maintains a list of
[AI-enabled medical devices](https://www.fda.gov/medical-devices/software-medical-device-samd/artificial-intelligence-enabled-medical-devices)
that it identified from marketing records. The list is not a complete
list of all AI health tools. FDA guidance also treats intended use,
limits, bias, test results, and later changes as key facts.

### Protect PHI in AI Workflows

An ambient AI scribe may record a visit and draft a note. A prediction
tool may send EHR data to a vendor cloud. Each transfer needs a scope and
security test.

Ask which data leaves the health group, which vendor receives it, and
whether a business associate agreement applies. Check storage, access,
subcontractors, model training, retention, deletion, and incident notice.
Do not assume a claim that a tool is "HIPAA compliant" answers these
questions.

Patients also need clear facts when AI has a major role in a care
choice. The exact legal consent duty can vary. The ethical aim is clear:
state the tool's role, its material limits, the human review, and the way
to raise a concern.

Use a release gate before an AI tool reaches care. Give each gate an
owner and a pass rule:

* **Use:** Does the tool match the care task and patient group?
* **Data:** Does the input fit the data used to build and test the tool?
* **Harm:** Are missed cases and false alarms within a safe bound?
* **Fairness:** Do group results meet the same safe bound?
* **Review:** Can a trained person reject the score and record why?
* **Change:** Will the team know when the model, data, or threshold shifts?
* **Stop:** Who can pause the tool after harm or drift appears?

A gate is more than a form. The owner must have the time and power to
stop the launch. The proof may be a local test, a log review, a staff
drill, or a signed risk choice. If proof is missing, the gate does not
pass.

### Try It Yourself 6.4: Gate an AI Triage Tool 🛠️

**Predict:** A hospital wants to use a triage model trained at suburban
hospitals. The local hospital serves many patients with chronic illness
and limited access to care. Should leaders approve it now?

**Run:** Check intended use, local data fit, subgroup results, false
results, human review, privacy, and change control.

**Explain:** In 1-2 sentences, choose approve, approve with conditions,
or decline. Name the evidence that controls your choice.

### Quick Check 6.4 ✅

1. How do false negatives and false positives harm patients in separate ways? *(Understand)*

2. Why can a model's overall score hide unfair group results? *(Analyze)*

3. Name three abilities a human reviewer needs to provide meaningful oversight. *(Apply)*

---

## 6.5 Summary and Retrieval 💡

### Key Concepts

* **HIPAA scope depends on roles and relationships.** Covered entities and business associates have defined duties. Not every health app or health fact falls under HIPAA.

* **Privacy and security work together.** The Privacy Rule limits many uses and disclosures. The Security Rule requires risk-based safeguards for ePHI.

* **Mobile tools need a full data map.** HIPAA, the FTC rule, state law, consent, BYOD controls, and group size may all affect a choice.

* **Clinical systems shape patient safety.** EHR exchange, CDS, CPOE, alerts, and telehealth must fit the person, task, and care setting.

* **Healthcare AI needs evidence and human control.** Teams must test local fit, subgroup results, false results, data flows, change control, and review authority.

### Key Terms

#### Section 6.1

* HIPAA
* Protected Health Information (PHI)
* Electronic PHI (ePHI)
* Covered entity
* Business associate
* Privacy Rule
* Security Rule
* Minimum necessary standard
* Breach Notification Rule

#### Section 6.2

* mHealth
* Consumer health app
* Health Breach Notification Rule (FTC)
* Informed consent
* BYOD

#### Section 6.3

* Electronic Health Record (EHR)
* Interoperability
* Clinical Decision Support System (CDSS)
* Computerized Provider Order Entry (CPOE)
* Alert fatigue
* Telemedicine
* Digital divide

#### Section 6.4

* AI-assisted diagnostics
* False negative
* False positive
* Algorithmic bias
* Human oversight (AI)

### Retrieval Practice

Try to answer these from memory before looking back at the chapter.

1. Name the three HIPAA safeguard groups and one example of each.
2. Why might a health app fall outside HIPAA but face an FTC notice rule?
3. Name four gates a hospital should test before it deploys an AI tool.

---

## 6.6 Skills Lab 6A: The MedPredict Decision

**Goal:** Evaluate a healthcare AI contract and recommend a safe decision.

**Evidence packet:** `assets/code/chapter-06/healthcare-ai-case.md`, a fictional case and evidence packet created for this textbook.

**Estimated time:** 90-120 minutes

### Case: Sepsis Prediction at Valley Regional Medical Center

**Fictional case:** Valley Regional Medical Center (VRMC) is a 350-bed
hospital. Leaders are considering a three-year, $1.8 million contract
with MedPredict AI.

The system uses vital signs, lab results, and EHR data to flag patients
at risk of sepsis. MedPredict reports 82% sensitivity and 95%
specificity in trials at 12 academic hospitals. The firm has not given
VRMC results by race, ethnicity, insurance status, disability, age, or
sex.

The training sites served more White and privately insured patients
than VRMC. VRMC serves a diverse urban community. Fifteen percent of its
patients are uninsured or covered by Medicaid.

The proposed workflow sends ePHI to MedPredict's cloud. The contract
includes a business associate agreement. It lets approved subcontractors
process data, but it does not list them in the main contract.

Each score appears in the EHR with a high, medium, or low risk label.
The tool does not show the main factors behind a score. MedPredict may
update the model each quarter with 14 days' notice. The contract gives
VRMC no right to an independent model audit.

Nurses already manage many alerts. A 95% specificity rate means about
five false alerts per 100 patients without sepsis under similar test
conditions. Local alert volume will also depend on how common sepsis is
and how VRMC sets the alert threshold.

Leaders may sign the contract, negotiate safeguards, or decline it.

<!-- markdownlint-disable MD029 -->

### Part 1: Foundation (Aligns with MLO-6.1)

1. List each stakeholder, the stakeholder's main interest, and one possible harm.
2. Test whether MedPredict is a business associate. Name four contract or Security Rule controls that VRMC should verify.
3. Explain what the reported sensitivity and specificity do and do not prove about local patient safety.

### Part 2: Application (Aligns with MLO-6.1, MLO-6.2)

4. Apply utilitarianism and deontology to the three choices: sign, negotiate, or decline.
5. Apply fairness, transparency, accountability, explainability, and human oversight from Chapter 3. Cite one case fact for each test.
6. Create a pre-deployment gate with one check for privacy, security, subgroup performance, alert burden, accessibility, and human review.

### Part 3: Extension (Aligns with MLO-6.2, MLO-6.3)

7. Write a 200-300 word recommendation to VRMC leaders. Choose one option and state the evidence that would change your choice.
8. Propose three contract changes. For each change, name the patient or worker risk it reduces and the proof VRMC should require.

<!-- markdownlint-enable MD029 -->

### Questions & Analysis 🤔

1. Which missing fact creates the greatest decision risk, and why?
2. When should patient safety outweigh a vendor's claim of trade secrecy?

### Rubric: Skills Lab 6A

This lab is graded with the standard
[Skills Lab Rubric](../skills-lab-rubric.md): four criteria at
4 points each, 16 points total. The criteria are Technical Accuracy
and Efficiency, Output Quality, Documentation Quality, and Analysis,
Interpretation, and Response to QUESTION(s).

For CIS111, **Technical Accuracy and Efficiency** means applying HIPAA
scope, safeguards, ethics tests, and performance facts correctly.
**Output Quality** means that your recommendation is clear, organized,
and safe for hospital leaders to use.

### Submission Guidelines

* **Length:** 800-1,200 words total across all parts
* **Format:** Submit one PDF named `skills-lab-6a-lastname.pdf`. Use clear headings for each part and label both Questions & Analysis answers.

---

## 6.7 Review Questions 🔄️

1. **Understand:** Distinguish PHI from a health fact that falls outside HIPAA.
2. **Apply:** Apply the minimum necessary standard to an IT support task.
3. **Analyze:** Analyze how telehealth can improve access and create a new barrier.
4. **Evaluate:** Which AI deployment gate should stop a hospital launch? Defend your threshold.

## Further Reading 📖

* [HHS Summary of the HIPAA Security Rule](https://www.hhs.gov/hipaa/for-professionals/security/laws-regulations/index.html): HHS explains current risk analysis and safeguard duties.
* [FTC Health Breach Notification Rule](https://www.ftc.gov/legal-library/browse/rules/health-breach-notification-rule): The FTC lists the rule and its 2024 update for many health apps and connected tools.
* [HHS Cross-State Telehealth Licensing](https://telehealth.hhs.gov/licensure/licensing-across-state-lines): HHS explains common state licensing paths for remote care.
* [ONC Clinical Decision Support](https://healthit.gov/clinical-quality-and-safety/clinical-decision-support/): ONC explains how CDS supports care choices and workflow.
* [FDA Transparency Principles for Machine Learning Medical Devices](https://www.fda.gov/medical-devices/software-medical-device-samd/transparency-machine-learning-enabled-medical-devices-guiding-principles): FDA identifies useful information about intended use, limits, bias, and later changes.

## Looking Ahead ⏩

Chapter 7 examines software defects, secure design, and liability. You
will test who should act when a software choice can cause harm.
