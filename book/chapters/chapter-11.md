# Chapter 11: Cybersecurity, Identity Theft, and Risk Assessment

In December 2020, the public learned that attackers had compromised SolarWinds Orion software. [SolarWinds told the SEC that fewer than 18,000 customers may have installed an affected version](https://www.sec.gov/Archives/edgar/data/1739942/000162828020017451/swi-20201214.htm). The attackers had placed malicious code in a software update and reached government and corporate networks. FireEye uncovered the campaign while investigating a breach of its own systems.

SolarWinds illustrates a sobering reality: even well-resourced groups with dedicated security teams can be breached. For IT professionals, knowing how to protect systems, respond to incidents, and build security policies is core professional responsibility.

This chapter covers a broad range because cybersecurity sits at the intersection of technology, law, policy, and ethics. You will learn the CIA Security Triad, identity theft, federal cybercrime laws, breach cases, and risk-assessment frameworks. You will also study security policy, incident response, and AI's role in attacks and defense.

## Module Overview 🧭

* **Estimated time:** 5-6 hours (reading + practice + Skills Lab)
* **Prerequisites:** Chapters 1-10
* **Deliverables:** Try It Yourself activities, Quick Checks, Skills Lab 11A

## Learning Objectives 🎯

By the end of this chapter, you will be able to:

* **MLO-11.1 (Analyze):** Analyze major identity theft methods and evaluate the effectiveness of prevention and response strategies
* **MLO-11.2 (Evaluate):** Evaluate IT security breaches using the CIA Security Triad and risk assessment frameworks to identify what went wrong and how threats should be prioritized
* **MLO-11.3 (Create):** Formulate security policies and develop prevention, detection, and response procedures for IT security threats

### This chapter aligns with the following Course Learning Outcomes

* **CLO XIV.** Analyze the major identity theft issues.
* **CLO XV.** Evaluate Information Technology security breaches and risk assessments.
* **CLO XVI.** Formulate security policies within Information Technology.
* **CLO XVIII.** Develop prevention, detection, and responses to Information Technology security attacks.

---

## 11.1 The CIA Security Triad and Current Threats

Every cybersecurity choice connects back to three principles. Whether you configure a firewall, write a policy, or respond to a breach, they tell you what you are protecting and why.

### The CIA Security Triad

The **CIA Security Triad** is the foundational framework for information security:

* **Confidentiality** keeps information accessible only to authorized users. A hospital restricting patient records to medical staff protects confidentiality. A hacker stealing a database of Social Security numbers breaches it.
* **Integrity** keeps information accurate, complete, and untampered. A bank guaranteeing your account balance reflects actual transactions protects integrity. An attacker altering financial records or modifying a software update (as in SolarWinds) compromises it.
* **Availability** keeps information and systems accessible to authorized users when needed. A hospital EHR operational during an emergency has availability. Ransomware locking down a city's systems destroys it.

These principles often trade against each other. Maximizing confidentiality (complex authentication for every action) reduces availability. Maximizing availability (easy access from anywhere) reduces confidentiality. Effective security balances all three based on the group's risk tolerance.

### Implementing CIA at Multiple Levels

Groups implement CIA at four levels:

* **Organizational.** Clear governance, defined roles, security budgets, and a culture treating security as everyone's responsibility. Chapter 3's principles apply: leadership that underfunds security puts stakeholders at risk.
* **Network.** Firewalls, **intrusion detection systems (IDS)**, **intrusion prevention systems (IPS)**, **VPNs**, and network segmentation protect data in transit.
* **Application.** Secure coding (Chapter 7), input validation, authentication, and encryption protect individual applications. SQL injection and cross-site scripting remain common attack vectors.
* **End-user.** The human element is consistently the weakest link. Strong passwords, **multi-factor authentication (MFA)**, security awareness training, and acceptable-use policies help against social engineering and phishing. No technical infrastructure compensates for a user who clicks a malicious link.

### Current Threats

Why are computer incidents so prevalent? Several factors converge:

* **Expanding attack surface.** Every new device, application, cloud service, and **Internet of Things (IoT)** sensor is another entry point. Groups now manage thousands of connected endpoints.
* **Professionalization of cybercrime.** Organized criminal groups operate like businesses with specialized roles and customer service for ransomware victims. **Ransomware as a Service (RaaS)** lets criminals with limited skills launch devastating attacks using tools developed by others.
* **Nation-state actors.** Russia, China, North Korea, and Iran conduct cyber operations for espionage, sabotage, and strategic advantage. The SolarWinds attack is attributed to Russia's SVR. Their resources and patience exceed typical criminal groups.
* **The speed gap.** Once a vulnerability is discovered, attackers develop **exploits** within hours or days. Many groups take weeks or months to apply patches.
* **Human factors.** Social engineering, phishing, and credential theft exploit psychology instead of technical flaws and are involved in most successful breaches.

Common types of exploits include:

| Exploit Type | How It Works | CIA Impact |
|---|---|---|
| **Phishing** | Deceptive emails or messages trick users into revealing credentials or installing malware | Confidentiality |
| **Ransomware** | Malware encrypts data and demands payment for the decryption key | Availability, Integrity |
| **Distributed Denial of Service (DDoS)** | Overwhelms systems with traffic to make them unavailable | Availability |
| **SQL injection** | Inserts malicious database commands through application input fields | Confidentiality, Integrity |
| **Man-in-the-middle (MITM)** | Intercepts communication between two parties without their knowledge | Confidentiality, Integrity |
| **Zero-day exploit** | Targets a previously unknown vulnerability before a patch is available | All three |
| **Insider threat** | An authorized user intentionally or accidentally causes harm | All three |


### Try It Yourself 11.1: Test Your First Judgment 🛠️

**Predict:** Think about the devices and accounts you use every day: your phone, email, social media, banking apps, school accounts. How many of these use multi-factor authentication? How many share the same password? If an attacker compromised one of your accounts today, what other accounts or data could they reach from there?

**Run:** Apply the main framework or choice test from Section 11.1. Identify the stakeholder whose interest carries the most weight.

**Explain:** In 1-2 sentences, state whether the structured test confirmed or changed your first judgment.

### Quick Check 11.1 ✅

1. Explain the three components of the CIA Security Triad and give one example of how each can be compromised. *(Understand)*

2. A university stores student grades in a cloud-based system. During final exams week, a DDoS attack makes the system inaccessible for 12 hours. Which component of the CIA triad was primarily compromised, and what secondary impacts might this have on the other two components? *(Analyze)*

3. Why is the "speed gap" between vulnerability discovery and patch deployment such a persistent cybersecurity challenge? Identify at least two reasons groups struggle to close this gap. *(Analyze)*

---

## 11.2 Identity Theft and Cybercrime

Identity theft is one of the most personal effects of cybersecurity failures. Victims spend months or years restoring credit, correcting fraudulent records, and recovering from the emotional toll. Understanding how it works is essential for IT professionals who protect the systems where personal data lives.

### What Is Identity Theft?

**Identity theft** is the unauthorized use of another person's **personally identifiable information (PII)** for financial gain. PII includes names, SSNs, dates of birth, addresses, and financial account numbers.

Identity theft takes several forms:

* **Financial identity theft** (most common): the thief opens credit cards, takes out loans, or makes purchases in the victim's name.
* **Medical identity theft**: someone uses another person's identity to obtain medical care, prescriptions, or insurance benefits, creating false medical records that can lead to dangerous treatment choices.
* **Criminal identity theft**: someone provides another person's identity during an arrest, leaving the victim with a criminal record they know nothing about.
* **Synthetic identity theft** (growing): criminals combine real and fabricated information, often pairing a real Social Security number (often a child's or a deceased person's) with a fake name and address. Synthetic identities are hard to detect because they do not match any existing person's records.
* **Tax identity theft**: filing a fraudulent return using someone else's SSN to claim their refund.

### Methods and Scale

Thieves obtain PII through multiple channels:

* **Data breaches** expose millions of records at once. The 2017 Equifax breach (Chapter 7) compromised data on about 147 million people.
* **Phishing and social engineering** trick people into voluntarily providing information through convincing emails, fake websites, or phone calls.
* **Dumpster diving and mail theft** remain effective: financial statements, pre-approved credit card offers, and medical bills all contain valuable PII.
* **Skimming** uses devices attached to ATMs or point-of-sale terminals to capture card data during legitimate transactions.
* **Dark web marketplaces** sell stolen identities, credit card numbers, and login credentials in bulk. A stolen SSN sells for a few dollars. A complete identity package can sell for significantly more.

The FTC receives millions of identity theft reports each year, and the actual number is likely much higher because many cases go unreported.

### Prevention and Response

Prevention requires action at both individual and organizational levels:

**Individual:**

* Strong, unique passwords and MFA wherever possible
* Regular credit monitoring (free annual reports from AnnualCreditReport.com)
* Credit freezes at Equifax, Experian, and TransUnion
* Caution about sharing personal information in response to unsolicited requests
* Shredding documents containing PII before disposal

**Organizational:**

* Collect only PII that is genuinely necessary (data minimization)
* Encrypt PII at rest and in transit
* Apply access controls so staff see only data they need
* Conduct regular security audits and vulnerability assessments
* Maintain a breach notification plan before a breach occurs
* Train staff to recognize social engineering

**If identity theft occurs,** the FTC sequence: place a fraud alert on credit reports, review for unfamiliar accounts, report at IdentityTheft.gov, file a police report, and contact fraud departments of affected firms. Recovery takes months and requires persistent follow-up.

### Federal Laws for Prosecuting Cybercrime

Several federal laws frame the prosecution of identity theft and computer crimes:

* **Computer Fraud and Abuse Act (CFAA):** Primary federal law for computer crimes. Criminalizes unauthorized access, exceeding authorized access, password trafficking, and malicious code. Critics argue its broad language can criminalize minor activities like terms-of-service violations.
* **Identity Theft and Assumption Deterrence Act (1998):** Made identity theft a federal crime.
* **Electronic Communications Privacy Act (ECPA):** Governs interception of electronic communications via the Wiretap Act and Stored Communications Act. Critics argue ECPA offers weaker protection for stored data than for real-time communications.
* **CAN-SPAM Act (2003):** Rules for commercial email and the right to opt out. Relevant because phishing often violates it.
* **State breach notification laws:** All 50 states have them, with specifics varying widely.


### Try It Yourself 11.2: Test Your First Judgment 🛠️

**Predict:** The CFAA's broad language has led to debates about whether activities like sharing a password with a friend or using a work computer for personal tasks could technically be federal crimes. Where do you think the line should be between legitimate security protection and overcriminalization of everyday computer use?

**Run:** Apply the main framework or choice test from Section 11.2. Identify the stakeholder whose interest carries the most weight.

**Explain:** In 1-2 sentences, state whether the structured test confirmed or changed your first judgment.

### Case Study 11.1 - The Anthem Healthcare Breach 📋

**The Situation:** In February 2015, Anthem, Inc. disclosed a breach affecting about 78.8 million current and former members and staff. The stolen data included names, birth dates, Social Security numbers, home addresses, email addresses, and employment information. The breach did not compromise medical records or financial data, but it exposed an extraordinary amount of PII.

The investigation revealed that the attackers had gained access through a spear phishing email sent to an Anthem worker. The email contained a malicious link that, when clicked, installed malware that allowed the attackers to move through Anthem's network and eventually access a database warehouse containing years of member information. The attackers had been inside the network for weeks before detection.

Several factors compounded the severity. Anthem had not encrypted the Social Security numbers stored in the compromised database. The firm argued that encryption would have been impractical given the volume of data that needed to be accessed for daily business operations. Critics responded that this choice prioritized operational convenience over the protection of highly sensitive data. Anthem ultimately agreed to a $115 million class-action settlement and a $16 million settlement with the U.S. Department of Health and Human Services for HIPAA violations.

**Stakeholders:**

* **78.8 million members and staff** whose PII was stolen, creating long-term identity theft risk
* **Anthem leadership and IT security team** who made choices about encryption, access controls, and phishing defenses
* **Healthcare providers and partners** who relied on Anthem's data security for patient trust
* **Federal and state regulators** responsible for enforcing data protection standards
* **The broader healthcare industry** which faced increased scrutiny of data security practices following the breach

**Questions to Consider:**

1. Anthem argued that encrypting the database was impractical for daily operations. Using the CIA triad, analyze whether this choice was a reasonable trade-off between availability and confidentiality, or an unjustifiable risk to member data.

2. The breach began with a single phishing email. To what extent should Anthem be held responsible for a worker's action, and what organizational measures could have limited the damage even after the initial compromise?

3. If you were an IT professional at Anthem who had recommended encryption of the database but was overruled by management, what would you do after the breach became public? Consider the whistleblowing principles from Chapter 5 and the fiduciary responsibilities discussed there.

### Quick Check 11.2 ✅

1. Name and briefly describe three different forms of identity theft. *(Remember)*

2. The CFAA criminalizes "unauthorized access" and "exceeding authorized access" to computer systems. Explain why the broad language of these terms has been controversial. *(Understand)*

3. An group stores customer Social Security numbers in an unencrypted database because encrypting it would slow down their claims processing system. Using the CIA triad, analyze this choice. Which principle did they prioritize, and which did they sacrifice? *(Analyze)*

---

## 11.3 Security Breaches, Risk Assessment, and Security Policies

Major breaches almost always reveal a chain of choices and systemic failures instead of a single catastrophic error. Understanding what goes wrong, how to assess risk, and how to build security policies are interconnected skills.

### IT Security Breaches: What Goes Wrong and Why

Common breach factors:

* **Unpatched vulnerabilities.** The 2017 Equifax breach exploited a known Apache Struts flaw for which a patch had been available for two months.
* **Weak access controls.** The 2013 Target breach began with compromised credentials from a third-party HVAC vendor. Attackers moved laterally to point-of-sale systems because the network was not properly segmented, stealing about 40 million card numbers.
* **Inadequate monitoring.** Attackers often operate inside networks for weeks or months before detection. The SolarWinds attackers had access for at least nine months.
* **Insufficient encryption.** As the Anthem case study shows, unencrypted data at rest means a breach of access controls immediately exposes data in readable form.
* **Human error.** Misconfigured cloud buckets, accidental email disclosures, lost devices, and weak passwords cause many breaches. These are preventable mistakes, not sophisticated attacks.
* **Third-party risk.** Vendors, cloud providers, and software supply chains are entry points. SolarWinds exploited this explicitly through a trusted software provider.

### Risk Assessment Frameworks

**Risk assessment** systematically identifies, analyzes, and evaluates threats to information assets, helping groups prioritize security investment where it matters most.

Standard steps:

1. **Asset identification.** What are you protecting? Data, systems, applications, IP, and physical infrastructure. A database of customer SSNs requires more protection than a marketing website.
2. **Threat identification.** External attackers, insider threats, natural disasters, hardware failures, and software defects.
3. **Vulnerability assessment.** Vulnerability scanning, penetration testing, and security audits reveal weaknesses.
4. **Likelihood estimation.** Historical data, industry intelligence, and threat modeling inform estimates.
5. **Impact analysis.** Financial loss, reputational damage, regulatory penalties, operational disruption, and harm to people.
6. **Risk calculation.** **Risk = Likelihood x Impact.** High-likelihood, high-impact threats demand immediate attention.
7. **Risk response.** Mitigate (reduce likelihood or impact), transfer (e.g., cyber insurance), accept (low-priority risks), or avoid (eliminate the risky activity).

The **NIST Cybersecurity Framework** organizes security functions into five categories, Identify, Protect, Detect, Respond, Recover, and has become a de facto standard, particularly for groups working with the U.S. government.


### Try It Yourself 11.3: Test Your First Judgment 🛠️

**Predict:** Think about a small business you are familiar with, such as a local restaurant, a tutoring service, or a small retail shop. What digital assets does that business have (customer data, financial records, online ordering systems)? If you were conducting a risk assessment for that business, what would you identify as the three most significant risks? How would your recommendations differ from those for a large corporation?

**Run:** Apply the main framework or choice test from Section 11.3. Identify the stakeholder whose interest carries the most weight.

**Explain:** In 1-2 sentences, state whether the structured test confirmed or changed your first judgment.

### Formulating Security Policies

A **security policy** is a formal document defining a group's rules and procedures for protecting information assets. Policies translate CIA principles and risk-assessment findings into actionable guidelines.

Effective policies address several areas:

* **Acceptable use policy (AUP):** What staff can and cannot do with organizational technology, such as personal-device-for-work rules (**BYOD**).
* **Password and authentication:** Complexity, expiration, and MFA requirements. Weak passwords remain a primary attack vector.
* **Data classification and handling:** Categorizes data by sensitivity (public, internal, confidential, restricted) and defines storage, transmission, and disposal for each. A **data classification** policy ensures a customer's SSN gets stronger protection than a firm newsletter.
* **Access control:** Implements the **principle of least privilege**, granting users access only to data and systems necessary for their job. Limits damage from compromised credentials or insider threats.
* **Incident response:** What happens when a security incident occurs (Section 11.4).
* **Remote work and mobile device:** Security for staff working from home or using mobile devices. Far more critical post-2020.
* **Vendor and third-party risk management:** Security requirements for partners with access to data or systems. Target and SolarWinds both demonstrate the effects of inadequate vendor management.

### Policy Enforcement and Compliance

A policy on paper provides no protection. Enforcement requires:

* **Training and awareness.** Annual security awareness training at minimum. Strong security cultures provide ongoing education.
* **Technical controls.** Enforce through technology where possible: if password policy requires 12 characters, the system should reject shorter passwords.
* **Monitoring and auditing.** Audits verify compliance. This raises workplace monitoring tensions from Chapter 10. Transparent policies stating what is monitored and why help balance security with worker privacy.
* **Effects for violations.** Clear, consistent effects. If executives are exempt, policies lose credibility.
* **Regular review.** Threats change constantly. Review the policy at least once a year and after major incidents.

### Quick Check 11.3 ✅

1. List the four possible responses to an identified risk in a risk assessment framework and give a brief example of when each would be appropriate. *(Remember)*

2. Explain the principle of least privilege and describe how violating it contributed to a real breach discussed in this chapter. *(Understand)*

3. A firm drafts a strict security policy requiring complex passwords, mandatory encryption, and limited remote access. However, staff routinely bypass these controls because they slow down daily work. What does this situation reveal about the relationship between security policies and organizational culture? What would you recommend? *(Evaluate)*

---

## 11.4 Incident Response, Computer Forensics, and AI in Cybersecurity

No matter how strong policies and controls are, breaches occur. The question is not whether but how prepared you are.

### Incident Response Across CSF 2.0

**Incident response** is the organized work of preparing for, detecting,
containing, communicating about, and recovering from a security incident.
[NIST SP 800-61 Revision 3](https://csrc.nist.gov/pubs/sp/800/61/r3/final)
connects that work to all six Cybersecurity Framework 2.0 functions:

* **Govern:** Set authority, policy, reporting duties, and choice roles.
* **Identify:** Know critical assets, dependencies, threats, and business impact.
* **Protect:** Apply safeguards, train people, keep backups, and prepare playbooks.
* **Detect:** Find possible incidents and analyze their scope and severity.
* **Respond:** Contain harm, remove the cause, coordinate actions, and communicate.
* **Recover:** Restore services, verify normal operation, and improve the program.

The functions support each other. A response team cannot protect an asset
that nobody identified. It cannot make a fast containment choice if
governance never assigned authority.

### Notification and Legal Obligations

When a breach involves personal data, groups face legal notification requirements. All 50 states have breach notification laws with varying specifics:

* **Who must be notified?** Affected people. Many laws also require state AGs, the FTC, or industry-specific regulators (HHS for health data, per Chapter 6's HIPAA discussion).
* **How quickly?** 30 to 90 days in most states. Some require "as expeditiously as possible." Delays bring additional penalties and erode trust.
* **What must it include?** What happened, what data was compromised, what the group is doing, and what affected people should do.

The ethical obligation extends beyond the law. Even when not legally required, the question is whether people whose data was exposed have a right to know. Grounded in Chapter 5's fiduciary principles, the answer is almost always yes. Transparency protects people and preserves trust.

### Computer Forensics

**Computer forensics** (or **digital forensics**) collects, preserves, analyzes, and presents digital evidence in a legally admissible way. After a breach, it answers: who did this, how did they get in, what did they access, how long were they inside?

Evidence integrity depends on strict procedures:

* **Preservation.** Create **forensic images** (specific bit-for-bit copies) before any changes. Shutting down, rebooting, or opening files can destroy evidence. The principle is "collect first, analyze later."
* **Chain of custody.** Document every step: who collected what, when, where, how stored. A break in the **chain of custody** can make evidence inadmissible. Investigators use write blockers (preventing changes to the original) and cryptographic hashes (verifying evidence is unaltered).
* **Analysis.** Examine log files, file systems, network traffic, email, and memory dumps. Recover deleted files, trace connections, analyze malware, reconstruct attacker timelines. Tools are specialized. The principle is systematic, methodical investigation.
* **Reporting.** Findings must withstand legal scrutiny. Analysts may testify as expert witnesses. Testimony rests on evidence, not speculation.

For non-specialists, the lesson is: do not contaminate the evidence. If you suspect an incident, do not run your own investigation on affected systems. Secure them, document what you observed, and contact the incident response team or a qualified forensic specialist. Well-intentioned actions by untrained personnel are one of the most common ways digital evidence is compromised.

### AI Touchpoint: AI on Both Sides of the Cybersecurity Equation

The same AI capabilities that strengthen defenses empower attackers, creating an escalating arms race.

**AI-powered cyberattacks:**

* **Spear phishing at scale.** AI generates thousands of personalized phishing emails by scraping social media and public records, industrializing what was once labor-intensive.
* **Social engineering automation.** AI chatbots conduct real-time conversational attacks. Voice cloning replicates an specific person's voice from seconds of audio, enabling phone calls that sound like the CEO requesting an urgent wire transfer.
* **AI-generated malware.** LLMs write or modify malicious code, generating variants that evade detection. Vendor safeguards exist. Open-source models without them are freely available.
* **Deepfake-enabled fraud.** In 2024, a Hong Kong finance worker transferred roughly $25 million after attending a video call where every other participant, such as the CFO, was a deepfake.

**AI in defense:**

* **SOCs** use AI to analyze vast security data, flagging the handful of millions of log entries that represent genuine threats.
* **Behavioral analytics** establish normal-behavior baselines and alert on deviations: a worker who normally works business hours suddenly downloading large volumes at 3 AM gets flagged.
* **Automated response.** AI can isolate a compromised endpoint or block a malicious IP without waiting for humans, critical when attacks spread in minutes.
* **Threat intelligence.** AI predicts emerging threats from global data, dark web activity, and vulnerability databases.

**Limitations:**

* **False positives and alert fatigue.** Too many false alarms cause teams to miss real threats.
* **Adversarial AI.** Attackers can craft inputs that cause AI to misclassify malicious activity as benign.
* **Bias.** AI trained on historical threat data detects familiar patterns better than novel ones, and may flag user behaviors based on demographic correlations.
* **Over-reliance.** AI enhances human analysts. It does not replace them. Groups that cut teams based on AI find themselves vulnerable to threats AI was not trained for.

### AI Security Tools Need Their Own Controls

AI can help group alerts, detect patterns, and draft response steps. It can also miss new attacks, reproduce bias from historical data, or accept adversarial input. A team should know which actions the tool may take, which require approval, and how to restore an alert that was closed incorrectly.

The [NIST Cybersecurity Framework 2.0](https://www.nist.gov/cyberframework) treats governance as part of cybersecurity risk management. The [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework) applies the same idea to AI risk. Together, they support documented authority, testing, monitoring, escalation, and recovery.

When a security tool recommends containment, ask what evidence supports the action, what business process it may interrupt, and who can override it. Automation should shorten response time without removing accountability.


### Try It Yourself 11.4: Test Your First Judgment 🛠️

**Predict:** The same AI voice cloning technology that enables fraud (replicating a CEO's voice for a fake phone call) also has legitimate uses in accessibility and entertainment. How should society balance the benefits of this technology against its potential for harm? Should there be restrictions on who can use voice cloning tools and for what purposes?

**Run:** Apply the main framework or choice test from Section 11.4. Identify the stakeholder whose interest carries the most weight.

**Explain:** In 1-2 sentences, state whether the structured test confirmed or changed your first judgment.

### Quick Check 11.4 ✅

1. List the six CSF 2.0 functions and explain how Govern, Identify, and Protect prepare a group for incident response. *(Understand)*

2. Explain why an IT professional who discovers a potential security breach should not attempt their own forensic investigation on the affected systems. What specific risks does untrained investigation create? *(Understand)*

3. A firm's AI-powered security system flags a worker's activity as suspicious because the worker is accessing files outside normal business hours. The worker, who works a late shift, complains that the system unfairly targets their work pattern. Evaluate the ethical trade-offs between AI-powered behavioral monitoring and worker privacy. What steps could the group take to address both security and fairness concerns? *(Evaluate)*

---

## 11.5 Summary and Retrieval 💡

### Key Concepts

* **The CIA Security Triad is the foundation for all security thinking.** Confidentiality, integrity, and availability must be implemented at organizational, network, application, and end-user levels and balanced via risk assessment.
* **Identity theft is a pervasive and personal consequence of security failures.** Financial, medical, criminal, synthetic, and tax forms all exploit stolen PII. Prevention requires individual (strong passwords, credit monitoring, MFA) and organizational action (data minimization, encryption, access controls). Federal laws (CFAA, Identity Theft and Assumption Deterrence Act, ECPA) frame prosecution.
* **Breaches follow recognizable patterns.** Unpatched vulnerabilities, weak access controls, inadequate monitoring, insufficient encryption, human error, and third-party risk recur across breach analyses.
* **Risk assessment prioritizes security investments.** Identifying assets, threats, vulnerabilities, likelihood, and impact lets groups allocate limited resources where they matter most. The NIST Cybersecurity Framework provides a widely adopted structure.
* **Security policies translate principles into practice.** Effective policies cover acceptable use, authentication, data classification, access control, incident response, remote work, and vendor management, enforced through training, technical controls, monitoring, and effects.
* **Incident response requires preparation, not improvisation.** NIST SP 800-61 Revision 3 connects response work to all six CSF 2.0 functions. Computer forensics preserves evidence under controlled procedures.
* **AI is transforming both attack and defense.** AI-powered phishing, social engineering, malware generation, and deepfake fraud escalate threats.  AI threat detection, behavioral analytics, and automated response strengthen defense. Neither side has a permanent advantage, and human judgment remains essential.

### Key Terms

#### Section 11.1

* CIA Security Triad
* Confidentiality
* Integrity
* Availability
* Exploit
* Ransomware as a Service (RaaS)
* Intrusion detection system (IDS)
* Multi-factor authentication (MFA)

#### Section 11.2

* Identity theft
* Personally identifiable information (PII)
* Synthetic identity theft
* Computer Fraud and Abuse Act (CFAA)
* Electronic Communications Privacy Act (ECPA)
* Breach notification laws

#### Section 11.3

* Risk assessment
* NIST Cybersecurity Framework
* Security policy
* Principle of least privilege
* Data classification
* Acceptable use policy (AUP)

#### Section 11.4

* Incident response
* Computer forensics (digital forensics)
* Chain of custody
* Forensic image
* Security Operations Center (SOC)
* Behavioral analytics

### Retrieval Practice

Try to answer these from memory before looking back at the chapter.

1. Draw or describe the CIA Security Triad and explain how a single incident, such as a ransomware attack, can compromise all three components simultaneously.

2. Name three forms of identity theft, explain how each one works, and identify what type of stolen data enables each form.

3. Use the six CSF 2.0 functions to outline one incident-response action for each function.

4. Explain how AI is being used on both the attack and defense sides of cybersecurity. Give one specific example of an AI-powered attack and one specific example of an AI-powered defense.

---

## 11.6 Skills Lab 11A: Developing an Incident Response Plan

**Goal:** Analyze a credential breach and create an incident response plan that addresses identity theft risk, security policy, prevention, detection, response, and recovery.

**Evidence packet:** `assets/code/chapter-11/incident-response-case.md`, a fictional case and evidence packet created for this textbook.

**Estimated time:** 90-120 minutes

### Case

MidState Community College (MCC) enrolls about 12,000 students and employs 800 faculty and staff. The college's IT infrastructure includes:

* A student information system (SIS) containing student names, Social Security numbers, dates of birth, addresses, financial aid data, and academic records
* A learning management system (LMS) used by all students and faculty
* A cloud-based email system and collaboration platform
* A network of campus computers in labs, offices, and the library
* A public-facing website with an online application and payment portal
* A campus Wi-Fi network accessible to students, staff, and visitors

MCC recently experienced the following incident: A phishing email that appeared to come from the IT help desk was sent to about 200 faculty members. The email asked recipients to "verify their credentials" by clicking a link and entering their username and password. Thirty-two faculty members entered their credentials before the phishing attack was identified. During the investigation, the IT team discovered that six of the compromised accounts had been used to access the student information system, potentially exposing the personal data of about 4,500 students. The attackers also used two compromised accounts to send additional phishing emails to students, requesting financial information for a fake "emergency scholarship."

### Part 1: Foundation (Aligns with MLO-11.1)

1. Using the CIA Security Triad, analyze which components were compromised at each stage of this incident (the initial phishing attack, the credential theft, the SIS access, and the secondary phishing campaign targeting students).

2. Identify at least three specific security failures or vulnerabilities that allowed this incident to escalate from a phishing email to a potential breach of 4,500 student records.

3. What forms of identity theft are the 4,500 affected students now at risk for? Be specific about which types of stolen data enable which types of identity theft.

### Part 2: Application (Aligns with MLO-11.1, MLO-11.2)

4. Draft three specific security policy recommendations that MCC should implement to prevent a similar incident in the future. For each policy, identify:
   * What the policy requires
   * How it would be technically enforced
   * How it addresses an specific vulnerability revealed by this incident

5. MCC does not currently require multi-factor authentication for any systems. Write a brief policy statement (100-150 words) that establishes an MFA requirement for the college. Specify which systems and user groups it applies to, the timeline for implementation, and any exceptions.

### Part 3: Extension (Aligns with MLO-11.2, MLO-11.3)

6. Using the six CSF 2.0 functions, outline the actions MCC should take:
   * **Govern:** Who has authority, and what reporting duties apply?
   * **Identify:** Which assets, records, users, and dependencies are affected?
   * **Protect:** Which safeguards should have limited the attack?
   * **Detect:** How should the college determine scope and severity?
   * **Respond:** What containment, eradication, communication, and evidence actions come first?
   * **Recover:** How should MCC restore service and verify that the threat is gone?

7. Draft a breach notification letter (150-200 words) to the affected students. Include what happened, what data was potentially exposed, what MCC is doing in response, and what steps students should take to protect themselves. Your letter should be clear, honest, and written for a non-technical audience.

### Questions & Analysis 🤔

1. Which control would have broken the attack sequence earliest?
2. How should the notification balance transparency with investigative uncertainty?

### Rubric: Skills Lab 11A

This lab is graded with the standard
[Skills Lab Rubric](../skills-lab-rubric.md): four criteria at
4 points each, 16 points total. The criteria are Technical Accuracy
and Efficiency, Output Quality, Documentation Quality, and Analysis,
Interpretation, and Response to QUESTION(s).

### Submission Guidelines

* **Length:** 1,200-1,800 words total across all parts
* **Format:** Submit as a single document organized by part number. Use clear headings for each section.

---

## 11.7 Review Questions 🔄️

1. Explain how confidentiality, integrity, and availability guide security choices.
2. Apply a risk assessment to an identity-theft case.
3. Analyze why incident response must protect evidence while restoring service.
4. Create one policy control for a deepfake payment request. Explain how it reduces risk without blaming one worker.

## Further Reading 📖

* [NIST Cybersecurity Framework 2.0](https://www.nist.gov/cyberframework) - NIST organizes risk work around Govern, Identify, Protect, Detect, Respond, and Recover.
* [NIST SP 800-61 Revision 3](https://csrc.nist.gov/pubs/sp/800/61/r3/final) - NIST connects incident response to group-wide risk management.
* [IdentityTheft.gov](https://www.identitytheft.gov/steps) - The FTC provides reporting steps and personal recovery plans.
* [CISA: Recognize and Report Phishing](https://www.cisa.gov/secure-our-world/recognize-and-report-phishing) - CISA explains common phishing signs and reporting actions.
## Looking Ahead ⏩

In Chapter 12, you shift from systems to the duties of the people who build and manage them. You will study the ACM, IEEE, and (ISC)² codes of ethics. You will also assess IT licensing, certification, emerging technology, and a capstone case.
