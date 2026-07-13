# Chapter 5: Whistleblowing and Accountability

In October 2021, Frances Haugen, a former data scientist at Facebook (now Meta), appeared before the United States Senate Commerce Committee. She had secretly copied tens of thousands of internal firm documents and shared them with journalists and regulators. Those documents revealed that Facebook's own researchers had found evidence that its algorithms amplified misinformation, that Instagram harmed the mental health of teenage users, and that the firm had repeatedly chosen growth over safety. Haugen argued that she had tried to raise concerns internally and was ignored. Going public, she said, was the only option left.

Haugen's choice made her a public figure overnight. Supporters called her a hero who put the public interest above corporate loyalty. Critics questioned whether she had the right to take confidential documents and share them with the press. Her case illustrates the core tension at the heart of this chapter: when does a worker's obligation to the public outweigh their obligation to their employer? And what happens when the information at stake involves the private data of millions of people?

This chapter examines whistleblowing from both ethical and legal perspectives. You will learn what makes whistleblowing ethically justified, what legal protections exist for whistleblowers, and how fiduciary responsibilities create obligations to protect private information. You will also explore practical guidance for handling a whistleblowing situation, such as the emerging role of AI in both enabling and suppressing the act of speaking up.

## Module Overview 🧭

* **Estimated time:** 4-5 hours (reading + practice + Skills Lab)
* **Prerequisites:** Chapters 1-4
* **Deliverables:** Try It Yourself activities, Quick Checks, Skills Lab 5A

## Learning Objectives 🎯

By the end of this chapter, you will be able to:

* **MLO-5.1 (Understand):** Explain the concept of whistleblowing, distinguish between internal and external whistleblowing, and describe the ethical criteria that justify whistleblowing in IT contexts
* **MLO-5.2 (Apply):** Apply legal and ethical frameworks to evaluate whistleblower protections and determine appropriate courses of action in a whistleblowing scenario
* **MLO-5.3 (Analyze):** Analyze the fiduciary responsibilities organizations hold regarding private information and examine the ethical tensions between employer loyalty and the duty to protect data subjects

### This chapter aligns with the following Course Learning Outcomes

* **CLO V.** Illustrate whistle-blowing and protection for whistle-blowers.
* **CLO VII.** Interpret fiduciary responsibilities of private information.

---

## 5.1 When Is Whistleblowing Ethically Justified?

### Defining Whistleblowing

**Whistleblowing** is the act of reporting illegal, unethical, or harmful activities within a group to someone with the power to take corrective action. A **whistleblower** is the person who makes that report, usually an insider with direct knowledge of wrongdoing who chooses to speak up despite the effects.

Whistleblowing is distinct from ordinary workplace complaints. The distinction matters because whistleblowing exposes conduct that causes serious harm or violates a law, regulation, or ethical standard. It is about accountability at an organizational or societal level, not personal grievances.

In IT, whistleblowing cases are common because technology professionals often have access to information that others in the group do not see. A database administrator might discover that customer data is being sold without consent. A software engineer might find that a safety-critical system has known bugs management has chosen not to fix. A cybersecurity analyst might learn that the firm is concealing a data breach. In each case, the IT professional has knowledge that the public or regulators would want, and the question becomes: what do you do with it?

### Internal vs. External Whistleblowing

The most important distinction is between **internal whistleblowing** and **external whistleblowing**.

**Internal whistleblowing** means reporting through channels inside the group: a supervisor, compliance department, ethics hotline, or board of directors. The information stays inside the firm, which has the opportunity to investigate and correct the problem.

**External whistleblowing** means reporting to someone outside: a regulator, law enforcement, the media, or the public. This is a more dramatic step that takes the information beyond the group's control and can lead to investigations, lawsuits, and reputational damage.

Most ethical frameworks and legal protections assume internal reporting should come first: if the group can fix the problem internally, that is usually the least harmful path. External whistleblowing becomes justified when internal channels fail, when the group retaliates, or when the harm is so immediate and severe that waiting puts people at risk.

### Ethical Criteria for Justified Whistleblowing

Leaking confidential information for personal revenge or competitive advantage is not whistleblowing. Ethical analysis usually involves several criteria that distinguish justified disclosure from unauthorized leaking.

**Severity of the harm.** The wrongdoing must involve serious harm, either actual or potential. Exposing a firm knowingly shipping defective medical devices is different from exposing one that is merely inefficient.

**Exhaustion of internal channels.** A whistleblower should generally try to resolve the issue internally first. Using a compliance department, ethics hotline, or designated reporting mechanism demonstrates good faith. This criterion has limits: if internal channels are controlled by the same people responsible for the wrongdoing, or if using them puts the whistleblower at immediate risk, bypassing them may be justified.

**Reasonable belief in the truth of the claims.** The whistleblower should have a genuine, evidence-based belief that the wrongdoing is occurring. Ethical whistleblowing rests on facts and documentation, not rumors or speculation.

**Proportionality.** The disclosure should match the harm being reported. Disclosing more information than necessary, or to a wider audience than necessary, raises ethical concerns even when the underlying report is valid.

**Motivation.** Some frameworks consider motivation relevant. Is the whistleblower acting from concern for public safety, or primarily from personal grievance, financial reward, or revenge? The answer may not change whether the information should be disclosed, but it can affect how the whistleblower's actions are judged.


### Try It Yourself 5.1: Test Your First Judgment 🛠️

**Predict:** You discover that your IT department has been storing customer credit card numbers in plain text, a serious security vulnerability that violates industry standards. You report it to your manager, who says, "We know, but fixing it would cost too much and delay our product launch. Keep this to yourself." What would you do next? Which of the ethical criteria above support your choice?

**Run:** Apply the main framework or choice test from Section 5.1. Identify the stakeholder whose interest carries the most weight.

**Explain:** In 1-2 sentences, state whether the structured test confirmed or changed your first judgment.

### Quick Check 5.1 ✅

1. In your own words, explain the difference between internal and external whistleblowing. Why do most ethical frameworks recommend trying internal channels first? *(Understand)*

2. A software engineer notices that a colleague is cutting corners on quality testing for a medical device application. The engineer reports it to their manager, who dismisses the concern. Using the ethical criteria from this section, determine whether the engineer would be justified in escalating the report externally. Explain your reasoning. *(Apply)*

3. Why is the criterion of "reasonable belief in the truth of the claims" important for ethical whistleblowing? What risks arise if a person blows the whistle based on rumors instead of evidence? *(Analyze)*

---

## 5.2 Legal Protections for Whistleblowers

Ethical justification is one thing. Legal protection is another. Many people who are ethically justified in blowing the whistle still face devastating personal and professional effects. Legal protections exist to reduce those effects, but they are imperfect and inconsistent.

### The Sarbanes-Oxley Act (SOX)

The **Sarbanes-Oxley Act of 2002 (SOX)** was passed after the collapse of Enron and WorldCom, whose accounting fraud destroyed billions in shareholder value and retirement savings. Congress recognized that staff inside these firms had known about the fraud but feared retaliation.

SOX includes whistleblower protections for staff of publicly traded firms:

* **Protection from retaliation.** Firms cannot fire, demote, suspend, threaten, harass, or discriminate against staff who report suspected fraud to a regulatory agency, law enforcement, or a supervisor.
* **Complaint process.** Staff who believe they were retaliated against can file with OSHA. If OSHA does not act within 180 days, they can sue in federal court.
* **Criminal penalties.** People who knowingly retaliate against a whistleblower can face fines and up to ten years in prison.

SOX has limitations. It applies primarily to staff of publicly traded firms, leaving workers at private firms, contractors, and gig workers with weaker or no coverage. The complaint process can be slow, and proving retaliation is often difficult because employers can point to other reasons for adverse actions.

### The Dodd-Frank Act

The **Dodd-Frank Wall Street Reform and Consumer Protection Act of 2010**, passed after the 2008 financial crisis, expanded protections beyond SOX in two significant ways.

**Financial incentives.** Whistleblowers who report securities violations to the SEC can receive 10% to 30% of monetary sanctions collected from their information, when sanctions exceed $1 million. The SEC has awarded over $2 billion under the program.

**Stronger anti-retaliation provisions.** Dodd-Frank lets whistleblowers sue their employer directly in federal court without first going through OSHA, and extends coverage to a broader range of workers, such as some contractors and temporary staff.

Dodd-Frank changed the calculus for potential whistleblowers. Before it, whistleblowing was almost entirely a personal sacrifice. Financial rewards do not eliminate the risk, but they offset some of the career damage and personal cost.

### The False Claims Act

The **False Claims Act (FCA)**, originally passed during the Civil War and amended in 1986, lets private citizens file lawsuits on behalf of the federal government against entities defrauding government programs. This is the **qui tam** provision, from the Latin for "who sues on behalf of the king."

The FCA matters in IT when firms defraud the government through technology contracts. If a defense contractor bills for cybersecurity protections that were never implemented, a worker who discovers the fraud can file a qui tam suit and receive 15% to 30% of any recovery.

### Limitations of Legal Protections

Despite these laws, whistleblowers continue to face significant risks.

**Retaliation is hard to prove.** Employers rarely say, "We fired you because you blew the whistle." They point to performance issues, restructuring, or other seemingly legitimate reasons, and gathering evidence of the real cause is difficult.

**Career damage is real and lasting.** Even whistleblowers who win legal cases often struggle to find work in their industry afterward. Research consistently shows higher rates of job loss, financial hardship, and mental health challenges among whistleblowers than among their peers.

**Coverage gaps exist.** Independent contractors, staff of private firms, and workers in some industries may have fewer protections. State laws vary widely.

**International inconsistency.** Protections vary dramatically across countries. The European Union's Whistleblower Protection Directive (2019) requires member states to establish reporting channels and protect whistleblowers. Other jurisdictions offer little or none. For IT professionals in global groups, the landscape can be unpredictable.

### Case Study 5.1 - The Quiet Database 📋

**The Situation:** Priya Nair is a senior database administrator at MedVault, a mid-sized health IT firm that manages electronic health records for over 200 regional hospitals. During a routine audit, Priya discovers that MedVault's patient data encryption system has a critical flaw: data is encrypted during transmission but stored unencrypted on MedVault's internal servers. This means that anyone with internal server access, such as dozens of MedVault staff and contractors, can view unencrypted patient records containing diagnoses, medications, Social Security numbers, and insurance information.

Priya reports the vulnerability to her direct supervisor, Marcus Chen, who escalates it to MedVault's Chief Technology Officer, David Park. Two weeks later, David tells Priya that the firm has decided not to fix the vulnerability immediately. The encryption upgrade would cost about $2.3 million and require 14 months of development work. MedVault is preparing for a major funding round, and David says the timing is "not right" to disclose a security weakness. He instructs Priya to document the issue but to keep it confidential. "We will get to it after the funding closes," he says.

Three months pass. The funding round is still ongoing, and no action has been taken. Priya learns that MedVault recently signed a contract with a new hospital network, representing the health data of 400,000 additional patients, without disclosing the encryption flaw. She is increasingly concerned that a data breach could expose millions of patient records. She also knows that the Health Insurance Portability and Accountability Act (HIPAA) requires groups to implement reasonable safeguards for protected health information, and she believes MedVault is in violation.

**Stakeholders:**

* **Priya Nair**, the database administrator who discovered the vulnerability, faces career risk if she escalates externally but feels a professional and ethical obligation to protect patient data
* **Patients** whose health records are stored on MedVault's servers without adequate encryption, such as those at the newly signed hospital network who are unaware of the risk
* **MedVault's executives and investors** who are focused on closing a funding round and fear that disclosing the flaw will scare off investors
* **The hospital networks** that contract with MedVault and trust that patient data is being protected according to industry standards and legal requirements
* **Government regulators (HHS Office for Civil Rights)** who enforce HIPAA and have the authority to investigate and penalize groups that fail to protect health data

**Questions to Consider:**

1. Using the ethical criteria for justified whistleblowing from Section 5.1, evaluate whether Priya would be justified in reporting MedVault's encryption flaw to federal regulators. Consider each criterion (severity, internal channels, reasonable belief, proportionality, motivation) in your analysis.

2. Identify the competing obligations Priya faces. What does she owe to her employer? What does she owe to the patients whose data is at risk? How would a deontological framework from Chapter 1 help Priya sort through these competing duties?

3. If you were Priya, what would you do at this point? Be specific about the steps you would take and explain the ethical reasoning behind each step.

### Quick Check 5.2 ✅

1. Name the three major federal laws discussed in this section that provide whistleblower protections and briefly describe what each one covers. *(Understand)*

2. A cybersecurity analyst at a private startup discovers that the firm is concealing a data breach from customers. The analyst wants to report it but is worried about retaliation. Based on the legal protections discussed in this section, what options does the analyst have, and what limitations might they face? *(Apply)*

3. Why does the financial incentive structure under the Dodd-Frank Act matter ethically? Does paying whistleblowers for information strengthen or weaken the integrity of whistleblowing? Consider arguments on both sides. *(Analyze)*

---

## 5.3 Fiduciary Responsibilities and Private Information

Whistleblowing often involves private information. Sometimes the wrongdoing being reported is the mishandling of that information. To understand the full ethical picture, you need to understand what groups owe to the people whose data they hold. That obligation is called **fiduciary responsibility**.

### What Is Fiduciary Duty?

A **fiduciary duty** is a legal and ethical obligation to act in the best interest of another party. It arises when one party trusts another to manage something valuable. Examples include a doctor's duty to a patient, a lawyer's duty to a client, and a financial advisor's duty to an investor.

In IT, fiduciary duty extends to data. When a group collects personal information from customers, patients, staff, or users, it takes on responsibility to protect that information. The data does not belong to the group the way inventory or equipment does. It belongs to the people it describes. The group holds it in trust. This is the foundation of data privacy law and ethics, and it means groups have obligations beyond minimum legal compliance.

### Data as a Trust

When you sign up for an online service and provide your name, email, and phone number, you are not giving that information away. You are lending it for an specific purpose. The firm becomes the **custodian** of that data, and custodianship carries responsibility.

**Personally identifiable information (PII)** is any data that can identify an specific individual: names, addresses, Social Security numbers, phone numbers, email addresses, biometric data, IP addresses, and health records. The more sensitive the PII, the greater the group's obligation to protect it.

Groups that collect PII owe data subjects five things:

* **Transparency.** Clearly explain what data is collected, why, how it is used, who it is shared with, and how long it is retained, in plain language.
* **Purpose limitation.** Use data only for the purposes it was collected for. An email collected for order confirmations should not be repurposed for marketing without explicit consent.
* **Data minimization.** Collect only what is needed. Collecting data "just in case" is inconsistent with fiduciary responsibility.
* **Security.** Implement reasonable technical and administrative safeguards against unauthorized access, theft, or accidental exposure.
* **Accountability.** When something goes wrong, take responsibility: notify affected people, cooperate with regulators, and act to prevent recurrence.

### When Loyalty to Your Employer Conflicts with Duty to Protect Data

This is where fiduciary responsibility connects directly to whistleblowing. An IT professional has an obligation to their employer, but they also have an obligation to the people whose data the employer holds. When the two conflict, the ethical tension can be intense.

Consider this case: you work for a firm that has experienced a data breach affecting 500,000 customer records. Your employer decides not to disclose the breach, hoping to fix the vulnerability quietly. You know affected customers are at risk of identity theft and that several state laws require notification within an specific timeframe.

Loyalty to your employer pulls one direction. Obligation to the data subjects pulls another. Fiduciary responsibility argues the obligation to the data subjects should take priority, because the data was entrusted for safekeeping and the group has failed in that duty.

This is not a simple choice. Reporting externally could cost you your job and damage the firm. Coworkers uninvolved in the cover-up could be harmed. But staying silent while hundreds of thousands of people remain unaware their information is compromised carries its own costs. The ethical frameworks from Chapter 1 help sort through this tension. Utilitarianism weighs the harm of concealment against the harm of disclosure. Deontology asks whether honesty is a duty regardless of effects. Social contract theory asks what rules a fair society would accept.


### Try It Yourself 5.2: Test Your First Judgment 🛠️

**Predict:** You work at a firm that sells a popular fitness tracking app. The app collects users' location data, heart rate, sleep patterns, and exercise routines. You discover that the firm has been selling aggregated (but not fully anonymized) user health data to insurance firms. The privacy policy technically allows it in a vague clause buried on page 12. Is the firm fulfilling its fiduciary duty to users? Does the fact that it is technically "legal" make it ethical? What would you want to know if you were one of the app's users?

**Run:** Apply the main framework or choice test from Section 5.2. Identify the stakeholder whose interest carries the most weight.

**Explain:** In 1-2 sentences, state whether the structured test confirmed or changed your first judgment.

### Quick Check 5.3 ✅

1. Define fiduciary duty in your own words and explain how it applies to groups that collect personal data. *(Understand)*

2. A social media firm collects user data for ad targeting and then begins sharing that data with law enforcement agencies without user consent or a court order. Apply the five obligations of data custodianship (transparency, purpose limitation, data minimization, security, accountability) to evaluate whether this practice is ethically defensible. *(Apply)*

3. Analyze the ethical tension between an IT professional's loyalty to their employer and their obligation to protect the data subjects whose information the employer holds. Under what circumstances should the obligation to data subjects take priority? *(Analyze)*

---

## 5.4 Practical Guidance for Handling a Whistleblowing Situation

If you find yourself in a situation where whistleblowing may be necessary, what should you do?

### Step 1: Document Everything

Before taking any action, start collecting evidence. Without documentation, claims can be dismissed as hearsay and protections are weak.

**What to document:**

* Dates, times, and locations of events you observed
* Names of people involved and their roles
* Copies of relevant emails, messages, reports, or files (consult a lawyer before taking proprietary materials)
* Your own written account, recorded as close to each event as possible
* Records of internal reports you made: who, when, and what response you received

**Where to keep it:** Store copies outside firm systems. A personal email, a secure cloud account, or a physical copy at home is safer than a file on a work laptop the firm can access or delete.

### Step 2: Use Internal Channels First (When Safe to Do So)

Internal reporting is usually the right first step, both ethically and legally. Many whistleblower protections require or encourage it before external disclosure.

Report to your direct supervisor if they are not involved. If they are, go up: next-level management, compliance, the ethics hotline, or the board. Put it in writing and keep a copy. If your group has a Chief Ethics Officer (Chapter 3), that person is the designated resource. The firm's code of ethics may also outline specific procedures and protections.

Consider skipping internal channels if:

* The wrongdoing involves senior leadership and there is no independent reporting mechanism
* You have already reported internally and been ignored or told to stay silent
* Reporting internally is likely to result in destruction of evidence
* The harm is so immediate and severe that waiting for an internal response would put people at risk

### Step 3: Seek Legal Advice

Before going external, consult a lawyer who specializes in whistleblower cases. The legal landscape is complex, and a single misstep can undermine your protections. A lawyer can help you understand which laws apply, what evidence you need, how to file without exposing yourself to liability, and what financial or legal protections you may be entitled to. Many whistleblower attorneys offer free initial consultations. The Government Accountability Project and the National Whistleblower Center provide resources and referrals.

### Step 4: Report to the Appropriate External Authority

If internal channels have failed, the appropriate external authority depends on the type of wrongdoing:

* **Financial fraud or securities violations:** Securities and Exchange Commission (SEC)
* **Health data violations:** Department of Health and Human Services, Office for Civil Rights
* **Government contract fraud:** The relevant federal Inspector General, using the False Claims Act
* **Environmental violations:** Environmental Protection Agency (EPA)
* **General workplace safety:** Occupational Safety and Health Administration (OSHA)

Filing with the correct agency activates specific legal protections and routes the complaint to investigators with appropriate authority.

### Step 5: Prepare for the Personal Impact

Whistleblowing is stressful even when it is the right thing to do. Research consistently shows whistleblowers face anxiety, isolation, and depression, and professional and family relationships often suffer. A support system, such as legal representation, trusted friends or family, and possibly a therapist, matters. Whistleblower Network News and ExposeFacts offer peer support communities.

### AI Touchpoint: Technology as Both Shield and Weapon

Artificial intelligence is changing the whistleblowing landscape in two ways, neither entirely positive.

**AI-enabled retaliation monitoring.** Some groups now deploy AI-powered surveillance to monitor worker email, chat, and keystrokes. These systems flag behavior such as searching for whistleblower-protection information, contacting external lawyers, or copying unusual volumes of data. Firms frame the tools as protection against data theft and insider threats, but the same flags can identify potential whistleblowers before they ever make a report. The **accountability** principle from Chapter 3 raises the question: who is responsible when AI surveillance is used to suppress legitimate whistleblowing? If a system flags a worker documenting evidence of fraud and management uses that flag to fire the worker preemptively, both the technology and the people who deployed it share responsibility.

**AI systems trained on private data.** Many AI systems are trained on datasets that include personal information collected without meaningful consent. When a whistleblower discovers that their firm's AI models were trained on data users never agreed to share for that purpose, the case sits at the intersection of whistleblowing and fiduciary duty. The **transparency** and **fairness** principles from Chapter 3 apply directly: if users do not know their data is being used to train AI, transparency fails. If the resulting model treats certain groups unfairly because of biased or improperly sourced training data, fairness fails too.

Electronic monitoring can affect protected reporting and organizing. The [NLRB](https://www.nlrb.gov/about-nlrb/rights-we-protect/your-rights/interference-with-worker-rights) warns that electronic monitoring and algorithmic management may interfere with rights protected by federal labor law. The [EEOC](https://www.eeoc.gov/newsroom/us-eeoc-and-us-department-justice-warn-against-disability-discrimination) also explains that employment software can create unlawful disability barriers.

The EU AI Act places some employment systems in its high-risk category. Application dates and duties follow the [European Commission's current timeline](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai). Separate whistleblower laws govern reporting channels and retaliation.

If you help deploy an insider-risk tool, ask what behavior it flags, who reviews a flag, and whether workers can challenge an adverse choice. A possible data-loss alert may also identify someone preserving evidence of wrongdoing. Human review needs a written standard, not a manager's instinct.


### Try It Yourself 5.3: Test Your First Judgment 🛠️

**Predict:** Imagine you work at a firm that uses AI-powered tools to monitor all worker emails and chat messages. You have just discovered evidence that the firm is violating customer privacy. You want to report it, but you know the monitoring system might flag your communications with a lawyer or a regulator. How does the existence of AI surveillance change your approach to whistleblowing? What steps would you take to protect yourself?

**Run:** Apply the main framework or choice test from Section 5.3. Identify the stakeholder whose interest carries the most weight.

**Explain:** In 1-2 sentences, state whether the structured test confirmed or changed your first judgment.

### Try It Yourself 5.4: Test the Boundary 🛠️

**Predict:** Which option in this section creates the least ethical risk?

**Run:** Apply one ethical framework and one stakeholder test from Section 5.4.

**Explain:** Defend your result with one fact from the section.

### Quick Check 5.4 ✅

1. List the five practical steps for handling a whistleblowing situation discussed in this section and briefly explain why each one matters. *(Understand)*

2. An IT security specialist at a private firm discovers that customer data is being shared with unauthorized third parties. The specialist has already reported the issue to their manager and the compliance department, but both dismissed the concern. Apply the practical guidance from this section to recommend the specialist's next steps. *(Apply)*

3. How does AI-powered worker surveillance create new ethical challenges for potential whistleblowers? Analyze the tension between a firm's legitimate interest in preventing data theft and a whistleblower's need to document and report wrongdoing. *(Analyze)*

---

## 5.5 Summary and Retrieval 💡

### Key Concepts

* **Whistleblowing** is reporting illegal, unethical, or harmful activities. It can be internal (through firm channels) or external (to regulators, media, or the public). Ethical whistleblowing is justified when harm is serious, internal channels have failed or are unsafe, the whistleblower has a reasonable evidence-based belief, and the disclosure is proportionate.

* **Legal protections** vary by situation. The Sarbanes-Oxley Act covers certain fraud reports by staff of public firms. The Dodd-Frank Act adds incentives and anti-retaliation provisions for securities reports. The False Claims Act allows private citizens to sue on behalf of the government. Despite these laws, whistleblowers face career damage, retaliation that is hard to prove, and coverage gaps depending on employment status and location.

* **Fiduciary responsibility** in IT means groups holding personal data must act in the best interest of the data subjects: transparency, purpose limitation, data minimization, security, and accountability. Data is held in trust, not owned.

* **Loyalty to employer can conflict with the duty to protect data subjects.** When an employer mishandles data, an IT professional's fiduciary obligation may take priority over loyalty. Chapter 1 frameworks and Chapter 3 AI principles help work through the tension.

* **AI creates new whistleblowing challenges.** AI surveillance can identify and suppress potential whistleblowers before they report. AI models trained on improperly sourced data create new categories of wrongdoing. Accountability and transparency from Chapter 3 apply directly.

### Key Terms

#### Section 5.1

* Whistleblowing
* Whistleblower
* Internal whistleblowing
* External whistleblowing

#### Section 5.2

* Sarbanes-Oxley Act (SOX)
* Dodd-Frank Act
* False Claims Act (FCA)
* Qui tam

#### Section 5.3

* Fiduciary duty
* Personally identifiable information (PII)
* Data minimization
* Purpose limitation

#### Section 5.4

* AI-enabled retaliation monitoring

### Retrieval Practice

Try to answer these from memory before looking back at the chapter.

1. Name the four ethical criteria for justified whistleblowing and explain why each one matters.
2. What are the key differences between the whistleblower protections in the Sarbanes-Oxley Act and the Dodd-Frank Act? Which law provides financial incentives, and how does that work?
3. Explain the concept of fiduciary duty as it applies to groups that hold personal data. Give an specific example of how a firm could violate this duty and describe why an IT professional might face a whistleblowing choice as a result.

---

## 5.6 Skills Lab 5A: The DataStream Dilemma

**Goal:** Assess a whistleblowing choice and recommend a responsible escalation path.

**Evidence packet:** `assets/code/chapter-05/datastream-case.md`, a fictional case and evidence packet created for this textbook.

**Estimated time:** 90-120 minutes

### Case: DataStream Analytics and the Training Data Problem

Kenji Watanabe is a machine learning engineer at DataStream Analytics, a fast-growing firm that sells AI-powered customer behavior prediction tools to retailers. DataStream's flagship product, PredictShop, analyzes customer purchase histories, browsing behavior, and location data to predict what products individual customers are likely to buy next. Retailers use PredictShop to personalize marketing, adjust pricing, and manage inventory.

Six months ago, Kenji was assigned to improve PredictShop's accuracy. While reviewing the training data pipeline, he discovered several troubling facts:

* PredictShop is trained on data from a consumer rewards app called ShopPoints, which DataStream acquired two years ago. When ShopPoints users signed up, they agreed to share their data "to improve the ShopPoints experience." The terms of service said nothing about selling data to third parties or using it to train AI models for other firms.
* The training data includes detailed location histories, allowing PredictShop to infer where customers live, work, worship, and receive medical care. None of this information is relevant to predicting purchase behavior, but it remains in the dataset.
* DataStream's retail clients can access individual customer profiles generated by PredictShop, such as inferred demographic information such as estimated income level, household composition, and ethnicity. DataStream markets this as a "premium analytics" feature.
* Kenji found that PredictShop's pricing recommendations vary by inferred demographic group, with customers in lower-income zip codes consistently shown higher prices for identical products.

Kenji raised his concerns with his team lead, who told him the data usage was "probably fine" and that the legal team had reviewed the ShopPoints acquisition. Kenji then sent a detailed written report to DataStream's Vice President of Engineering, who responded that the firm was "aware of the data sourcing and comfortable with it." No further action was taken.

Kenji now faces a choice. He believes DataStream is violating the trust of millions of ShopPoints users, engaging in discriminatory pricing, and using personal data far beyond what was originally authorized. He is also aware that DataStream recently installed an AI-powered worker monitoring system that flags unusual data access patterns and external communications.

### Part 1: Foundation (Aligns with MLO-5.1)

1. Identify all stakeholders in this case. For each stakeholder, describe their specific interest and what they stand to gain or lose from Kenji's choice.
2. Using the ethical criteria for justified whistleblowing from Section 5.1, evaluate whether Kenji meets the threshold for ethically justified whistleblowing. Address each criterion (severity, internal channels, reasonable belief, proportionality, motivation).
3. Define fiduciary duty as it applies to this case. Explain what DataStream owes to the original ShopPoints users whose data is now being used in ways they did not agree to.

### Part 2: Application (Aligns with MLO-5.1, MLO-5.2)

4. Identify which whistleblower protection laws might apply to Kenji's situation. Explain which law(s) would be most relevant and what limitations he might face. Consider whether DataStream is publicly traded or private and how that affects his options.
5. Apply one ethical framework from Chapter 1 (utilitarianism, deontology, virtue ethics, or social contract theory) to Kenji's choice. What does your chosen framework recommend he do, and why?

### Part 3: Extension (Aligns with MLO-5.2, MLO-5.3)

6. Analyze the AI ethics dimensions of this case. Using the principles from Chapter 3 (fairness, transparency, accountability, explainability, human oversight), identify which principles DataStream is violating and explain how each violation harms specific stakeholders.
7. Write a 200-300 word recommendation advising Kenji on what to do next. Your recommendation should address the specific steps he should take, the risks he faces (such as from the AI monitoring system), and the ethical reasoning that supports your advice.

### Questions & Analysis 🤔

1. What threshold must be met before external disclosure becomes justified?
2. Which safeguard best protects both the whistleblower and affected data subjects?

### Rubric: Skills Lab 5A

This lab is graded with the standard
[Skills Lab Rubric](../skills-lab-rubric.md): four criteria at
4 points each, 16 points total. The criteria are Technical Accuracy
and Efficiency, Output Quality, Documentation Quality, and Analysis,
Interpretation, and Response to QUESTION(s).

### Submission Guidelines

* **Length:** 800-1,200 words total across all parts
* **Format:** Submit as a single document organized by part number. Use clear headings for each section.

---

## 5.7 Review Questions 🔄️

1. Distinguish internal from external whistleblowing.
2. Apply the chapter's justification criteria to a concealed security flaw.
3. Analyze how fiduciary duty can conflict with employer loyalty.
4. When internal reporting fails, what level of harm justifies public disclosure? Defend a threshold.

## Further Reading 📖

* [OSHA Whistleblower Protection Program](https://www.whistleblowers.gov/front) - OSHA explains protected activity, retaliation, and complaint paths.
* [SEC Whistleblower Program](https://www.sec.gov/enforcement-litigation/whistleblower-program) - The SEC describes reporting, awards, and anti-retaliation rules.
* [U.S. Department of Justice: False Claims Act](https://www.justice.gov/civil/false-claims-act) - DOJ explains federal fraud liability and qui tam actions.
* [ACM Code of Ethics Enforcement Procedures](https://www.acm.org/about-acm/code-of-ethics-enforcement-procedures) - ACM explains complaints, review, and protection against retaliation.
## Looking Ahead ⏩

In Chapter 6, you turn to healthcare IT ethics. You will study HIPAA, mobile health and telemedicine privacy, electronic health records, and clinical choice support. Each topic raises questions about patient safety and data protection. The fiduciary concepts from this chapter apply because healthcare groups hold sensitive data with high stakes.
