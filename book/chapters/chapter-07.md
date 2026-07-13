# Chapter 7: Software Liability and Secure Coding

On July 19, 2024, a CrowdStrike software update caused Windows computers to crash. [Microsoft estimated that 8.5 million devices were affected](https://blogs.microsoft.com/blog/2024/07/20/helping-our-customers-through-the-crowdstrike-outage/). Airlines grounded flights. Hospitals postponed care. Banks and emergency systems faced outages. This was not a cyberattack. A flawed update passed through an automated process without enough safeguards. One defect disrupted vital systems around the world within hours.

This incident is not an outlier. Software failures have caused passenger jets to crash, medical devices to deliver lethal radiation doses, and the personal data of hundreds of millions of people to be exposed. As software becomes embedded in everything from pacemakers to power grids, the question of who is responsible when that software fails is no longer theoretical. It is urgent, and it directly affects you as an IT professional.

This chapter examines software liability, software quality, secure coding, and cost/benefit analysis in IT choices. You will explore how product liability law applies to software and why development methods carry ethical weight. You will also study what happens when groups cut security to save time or money. The chapter closes with a hard question: when an AI system causes harm, who is accountable?

## Module Overview 🧭

* **Estimated time:** 4-5 hours (reading + practice + Skills Lab)
* **Prerequisites:** Chapters 1-6
* **Deliverables:** Try It Yourself activities, Quick Checks, Skills Lab 7A

## Learning Objectives 🎯

By the end of this chapter, you will be able to:

* **MLO-7.1 (Apply):** Apply product liability concepts, including negligence, strict liability, and warranty frameworks, to industry-relevant software failure scenarios
* **MLO-7.2 (Analyze):** Analyze the ethical obligations of software developers and organizations regarding software quality, secure coding, and vulnerability management
* **MLO-7.3 (Evaluate):** Evaluate cost/benefit trade-offs in IT decision-making, particularly in safety-critical systems and AI deployment

### This chapter aligns with the following Course Learning Outcomes

* **CLO VIII.** Examine issues with software and software liability.
* **CLO IX.** Apply cost/benefit analysis in information technology ethical decision-making.

---

## 7.1 Software Defects and Product Liability

A **software defect** (commonly called a "bug") is an error or unintended behavior in a program that causes incorrect or unexpected results. Some defects are trivial: a button displaying the wrong color, or a date that formats incorrectly. Others are deadly. In the late 1980s, the Therac-25 radiation therapy machine delivered massive radiation overdoses to at least six patients due to a software race condition. Three died. The software had been reused from an earlier model without adequate testing for the new hardware.

The critical ethical question is not whether defects will occur (they will), but what obligations developers and groups have to prevent, detect, and respond to them.

### Product Liability Frameworks

When a physical product injures someone, **product liability** law provides a framework for holding the manufacturer responsible. Software complicates that framework in several ways. Three theories cover most claims:

* **Negligence** requires proving that the developer or firm failed to exercise reasonable care: ignoring known defects, skipping industry-standard testing, or rushing a release without adequate quality assurance. If a firm knew about a critical vulnerability but shipped the product anyway to meet a deadline, a negligence claim has strong footing.

* **Strict liability** holds manufacturers responsible for defective products regardless of how careful they were. The question is not "Did you try hard enough?" but "Was the product defective, and did it cause harm?" Courts have been reluctant to apply strict liability uniformly to software.

* **Breach of warranty** occurs when software fails to perform as promised. Warranties can be **express** (explicitly stated in marketing or contracts) or **implied** (assumed by law, such as the implied warranty that a product is fit for its intended purpose).

### Is Software a "Product" or a "Service"?

This is one of the most contested questions in software liability law. When you purchase software on a disc or embedded in a device, courts are more likely to treat it as a product subject to product liability. When you access software through a cloud service or subscription (Software as a Service, or **SaaS**), courts have sometimes classified it as a service, which carries weaker liability standards. This distinction matters: if software is a product, strict liability may apply. If it is a service, the injured party must prove negligence, a higher burden.

The trend toward SaaS delivery means that much of the software you interact with daily exists in a legal gray area, and vendors may argue that product liability does not apply.

### Liability Limitations: EULAs and Terms of Service

Before you can use most software, you must agree to an **End User License Agreement (EULA)** or **Terms of Service (ToS)** that limits the firm's liability. Most users never read them. Even those who do have no practical alternative: you agree or you cannot use the software.

Courts have sometimes found egregious limitations **unconscionable** and unenforceable. In practice, most hold up, giving software vendors liability protection that manufacturers of physical products do not enjoy.


### Try It Yourself 7.1: Test Your First Judgment 🛠️

**Predict:** You install a popular antivirus program that promises "comprehensive protection against all known threats." A new strain of ransomware encrypts your files, and the antivirus software fails to detect it. The EULA says the firm is not liable for any damages. Do you think the firm has an ethical obligation to compensate you, even if the EULA says otherwise? What if the same ransomware affected a hospital and disrupted patient care?

**Run:** Apply the main framework or choice test from Section 7.1. Identify the stakeholder whose interest carries the most weight.

**Explain:** In 1-2 sentences, state whether the structured test confirmed or changed your first judgment.

### Quick Check 7.1 ✅

1. Explain the difference between negligence and strict liability in product liability law. Why does it matter which standard applies to software? *(Understand)*

2. A cloud-based accounting service has a defect that causes a small business to lose three months of financial records. The firm argues that because their product is a service (SaaS), not a product, strict liability should not apply. Using what you learned about the product-vs.-service distinction, explain whether this argument is ethically defensible, even if it is legally valid. *(Analyze)*

3. A software firm discovers a known defect in their hospital patient management system but decides to delay the fix until the next scheduled update in three months. Identify which product liability theory (negligence, strict liability, or breach of warranty) best applies to this situation and explain why. *(Apply)*

---

## 7.2 Software Quality and Development Ethics

Software quality is an ethical issue, not just a technical one. When groups choose how to build, test, and maintain their software, they are making choices that affect everyone who depends on it.

### What Does Software Quality Mean?

**Software quality** is the degree to which software meets its requirements and satisfies user needs. From an ethical standpoint, quality also means the software does not cause unnecessary harm, performs honestly, and communicates its limitations. A game with a minor graphical glitch has different quality obligations than a medical device that controls insulin dosing. Potential for harm shapes the standard.

### The Capability Maturity Model Integration (CMMI)

The **Capability Maturity Model Integration (CMMI)** measures a group's software development process maturity across five levels:

| Level | Name | Description |
|-------|------|-------------|
| 1 | Initial | Processes are unpredictable and reactive. Success depends on individual effort. |
| 2 | Managed | Projects are planned and tracked. Basic project management is in place. |
| 3 | Defined | Processes are standardized across the group. Consistent practices exist. |
| 4 | Quantitatively Managed | Processes are measured and controlled using statistical data. |
| 5 | Optimizing | Group focuses on continuous improvement based on data and innovation. |

Most groups operate at Level 1 or 2. Higher levels produce more predictable, reliable software. Groups that choose to remain at Level 1, accepting chaotic and unpredictable processes, are making a choice that affects everyone who depends on their software.

### Development Methodologies and Their Ethical Dimensions

How software is built shapes whether it is built well. Three dominant methodologies each carry distinct ethical implications:

**Waterfall** is a sequential process: requirements, then design, then coding, then testing, then deployment. Its strength is documentation and planning rigor. Its ethical risk is rigidity: if new risks emerge mid-development, waterfall makes adaptation difficult.

**Agile** delivers working software in short cycles (typically two-week "sprints"). Its ethical strength is adaptability: security flaws can be addressed in the next sprint. Its ethical risk is that pressure to ship quickly leads teams to cut corners on testing or security reviews. "Ship it now, fix it later" is an ethical problem.

**DevOps** integrates development and operations through automation, continuous integration, and continuous delivery (CI/CD). DevOps enables rapid patch deployment, an ethical advantage. The 2024 CrowdStrike incident shows the other side: an automated pipeline pushed a flawed update to millions of machines because its testing safeguards were insufficient. Speed without adequate safety checks creates ethical liability.

### Technical Debt and Ethical Implications

**Technical debt** is the accumulated cost of shortcuts taken during software development. Quick-and-dirty code meets a deadline but will be harder to maintain, harder to secure, and more likely to break. When groups accept technical debt without a repair plan, they transfer risk to users. Users bear the crashes, data loss, and security breaches while the group gains faster delivery.

### Case Study 7.1 - The MedTrack Patient Monitoring Dilemma 📋

**The Situation:** MedTrack Solutions is a mid-size software firm that develops patient monitoring systems for regional hospitals. Their flagship product, VitalWatch, tracks patient heart rate, blood pressure, and oxygen levels in real time and alerts nursing staff when readings fall outside safe ranges.

During a routine code review, senior developer Priya Nair discovers a defect in VitalWatch's alert logic. Under specific conditions (when a patient's heart rate drops below 40 beats per minute while oxygen saturation simultaneously falls below 88%), the system fails to trigger an alert. Instead, it logs the readings as normal. Priya estimates the defect affects roughly 2% of critical care patients.

Priya reports the defect to her manager, David Chen. David acknowledges the severity but explains the situation: MedTrack is in the middle of a major sales push. They are competing for a contract with a hospital network that would double the firm's revenue. David tells Priya that disclosing the defect now would derail the sales process and could lead to lawsuits from existing hospital clients. He asks her to document the bug internally and schedule the fix for the next quarterly release, three months away. He adds that the 2% occurrence rate is low and that nursing staff should catch most of those situations through manual monitoring anyway.

Priya is uncomfortable with this plan. She knows that in critical care, a missed alert could mean a patient dies. But she also knows that MedTrack employs 200 people, and losing the contract could lead to layoffs. She has a mortgage and a child in daycare.

**Stakeholders:**

* **Priya Nair (senior developer):** Discovered the defect. Feels a professional obligation to ensure patient safety but faces personal and professional risk if she escalates.
* **David Chen (engineering manager):** Responsible for the product timeline and aware of the firm's financial pressures. Prioritizing the sales contract over an immediate fix.
* **Hospital clients and patients:** Currently using a product with a known defect that could fail to alert staff during a life-threatening event. They do not know about the defect.
* **MedTrack Solutions (firm):** Faces financial risk from disclosure and legal risk from non-disclosure. Two hundred staff depend on the firm's stability.
* **Nursing staff:** Responsible for patient care. May rely on VitalWatch alerts as a safety net and may not catch every critical event through manual checks alone.

**Questions to Consider:**

1. Using the product liability frameworks from Section 7.1, which theory of liability (negligence, strict liability, or breach of warranty) would most likely apply if a patient is harmed because of this defect? Explain your reasoning.
2. Consider David's argument that the 2% occurrence rate is low and that nurses provide a backup. Is this an acceptable risk assessment, or is it a rationalization? How does the severity of potential harm change the calculation?
3. If you were Priya, what would you do? Identify which ethical framework (from Chapter 1) supports your choice and explain how you weighed the competing interests of patient safety, job security, and firm viability.

### Quick Check 7.2 ✅

1. Name and briefly describe the five CMMI maturity levels. At which level would you expect the most reliable and predictable software development outcomes? *(Remember)*

2. A startup uses agile development and ships a new feature every two weeks. They have no dedicated security review process because it would slow their release cycle. Analyze the ethical trade-off the startup is making and identify who bears the risk. *(Analyze)*

3. Explain the concept of technical debt using a non-technical analogy. Then describe one way that technical debt creates ethical risk for software users. *(Understand)*

---

## 7.3 Secure Coding and Vulnerability Management

Secure coding is not an afterthought. It is a fundamental ethical obligation for anyone who writes, reviews, or deploys software. Failures in secure coding create vulnerabilities that expose users to data theft, financial loss, and physical danger.

### What Is Secure Coding?

**Secure coding** is the practice of writing software that protects against security vulnerabilities by design. The core principle: every input is potentially malicious, every connection is potentially hostile, every assumption about software use is potentially wrong. These are design constraints from the start.

The **Open Web Application Security Project (OWASP)** maintains the OWASP Top 10, a regularly updated list of the most critical web application security risks.

### Common Vulnerability Types

As an IT professional, knowing the basic vulnerability categories helps you understand security risks, evaluate vendor claims, and participate in security discussions. You do not need to be a programmer.

**Injection flaws** occur when an attacker sends malicious data that a program treats as a command. The most common type is **SQL injection**: an attacker enters specially crafted text into a web form, and the application passes it directly to a database query. Without proper input validation, the attacker can read, modify, or delete database contents.

**Authentication and session management flaws** involve weaknesses in how software verifies identity: storing passwords in plain text, allowing weak passwords, failing to expire session tokens, or skipping multi-factor authentication for sensitive operations.

**Cross-site scripting (XSS)** occurs when an application includes untrusted data in a web page without validation, allowing attackers to inject malicious scripts that execute in other users' browsers. XSS is particularly dangerous because the malicious code runs in the context of a trusted website.

**Insecure direct object references** occur when an application exposes internal details (database record numbers, file paths) in URLs without checking authorization. A medical records portal where changing the patient ID in the URL reveals a different patient's records is a classic example.

**Security misconfiguration** refers to systems deployed with default settings, unnecessary features enabled, or incomplete configurations. It is one of the most common vulnerabilities because it results not from a coding error but from failure in deployment and maintenance.

### Responsible Disclosure vs. Full Disclosure

When a security researcher discovers a vulnerability in someone else's software, they face an ethical choice about how to report it.

**Responsible disclosure** (also called **coordinated disclosure**) means the researcher privately contacts the vendor, gives them a reasonable time (typically 90 days) to release a patch, and only then publishes details. Google's Project Zero team follows this approach.

**Full disclosure** means publishing the vulnerability immediately, without advance notice. Advocates argue it pressures vendors to act quickly. Critics argue it gives attackers a roadmap before a patch exists.

**Limited disclosure** involves sharing details with a trusted group (such as the CERT Coordination Center) that can coordinate response without publicizing the flaw. Each approach reflects different ethical priorities: user protection, vendor accountability, or a balance of both.

### Patch Management Ethics

**Patch management** is the process of developing, testing, and distributing updates that fix known vulnerabilities. It raises its own ethical questions: How quickly must a vendor release a patch? How much testing is required before deployment (a hasty patch can itself cause problems, as CrowdStrike demonstrated)? What obligation does a vendor have to patch software that has reached "end of life" but is still widely used?

The 2017 Equifax breach exposed the personal information of about 147 million people through a vulnerability that had a patch available two months earlier. Equifax knew about it but failed to apply it. The ethical failure was not the existence of the vulnerability. It was the organizational choice-making that left a known flaw unpatched in a system holding sensitive personal data.


### Try It Yourself 7.2: Test Your First Judgment 🛠️

**Predict:** Imagine you are a security researcher who discovers a critical vulnerability in a widely used open source library. The maintainer of the library is a single volunteer who responds to emails slowly and has no formal patching process. Meanwhile, you know that millions of applications depend on this library. Would you follow responsible disclosure (and wait, potentially for months, while users remain vulnerable), or would you choose a different approach? What factors would influence your choice?

**Run:** Apply the main framework or choice test from Section 7.2. Identify the stakeholder whose interest carries the most weight.

**Explain:** In 1-2 sentences, state whether the structured test confirmed or changed your first judgment.

### Quick Check 7.3 ✅

1. In your own words, explain what SQL injection is and why it is dangerous. You do not need to use technical code examples. Focus on the concept and the potential impact. *(Understand)*

2. Compare responsible disclosure and full disclosure of software vulnerabilities. What ethical values does each approach prioritize, and what risks does each approach accept? *(Analyze)*

3. The Equifax breach occurred because a known patch was not applied for two months. Identify at least two organizational factors that might explain why the patch was not applied, and explain whether any of those factors are ethically acceptable excuses. *(Evaluate)*

---

## 7.4 Cost/Benefit Analysis and Safety-Critical Systems

Every IT choice involves trade-offs, and cost/benefit analysis is a legitimate tool for navigating them. But when applied to choices affecting human safety, the ethical stakes increase dramatically.

### Risk Assessment Frameworks in IT

**Risk assessment** is the systematic process of identifying potential threats and estimating their likelihood and impact. The standard formula:

**Formula:** Risk = Likelihood x Impact

A highly likely threat with minimal impact (a minor website glitch) receives lower priority than an unlikely but catastrophic one (a complete data center failure). The **NIST Risk Management Framework** provides structured processes for evaluating and prioritizing risks.

**Cost/benefit analysis** weighs the cost of a security measure or improvement against the expected benefit, expressed as reduced risk. A $50,000 security upgrade that reduces expected annual losses from breaches by $200,000 clearly favors the investment.

### The Ethical Dimensions of Cost/Benefit Analysis

Cost/benefit analysis becomes ethically problematic when it reduces human safety to a dollar figure. The Ford Pinto case is the classic example: Ford calculated that paying settlements for burn injuries and deaths was cheaper than a recall. The math may have been accurate. The ethics were indefensible.

The same logic appears in IT. An group might conclude that skipping a security audit is "rational" because its cost exceeds expected breach losses. But this omits what is hard to quantify: human suffering from identity theft, erosion of public trust, and disproportionate impact on vulnerable populations with fewer resources to recover.

Ethical cost/benefit analysis requires acknowledging what the numbers leave out:

* **Who bears the risk?** Those who benefit from cost savings (executives, shareholders) are often not those who suffer the effects (users, patients, the public). That gap creates an ethical obligation to give extra weight to the interests of those who bear the risk.

* **What is being valued?** A patient whose medical records are exposed suffers harm credit monitoring cannot fully address.

* **What alternatives exist?** Cost/benefit analysis becomes dangerous when it frames the cheapest option as the only "rational" choice.

### Safety-Critical Systems

A **safety-critical system** is any system whose failure could result in death, serious injury, or significant environmental damage: aviation software, medical devices, nuclear plant controls, autonomous vehicles. These systems demand standards that make "good enough" wholly inadequate. Key principles include:

* **Redundancy:** Critical functions are backed by independent secondary systems.
* **Formal verification:** Mathematical methods prove that software meets its specifications.
* **Certification standards:** Aviation software follows DO-178C. Medical device software follows IEC 62304. Automotive software follows ISO 26262.
* **Fail-safe design:** When a safety-critical system encounters an error it cannot handle, it defaults to a safe state instead of continuing to operate unpredictably.

When failure means someone could die, the obligation to get it right is not measured by cost/benefit analysis. It is measured by the duty to protect human life.

### AI Liability: Who Is Responsible When AI Causes Harm?

Chapter 3 established AI ethics principles: fairness, transparency, accountability, explainability, and human oversight. Chapter 7 applies the accountability principle to liability specifically.

When traditional software causes harm, there is usually a clear chain: the developer wrote the code, the firm shipped the product, the failure can be traced to specific choices. AI complicates this chain in several ways:

* **Opacity:** Many AI systems, particularly deep learning models, operate as "black boxes." Developers may not be able to explain why a system produced a particular output, making it impossible to identify a "defect" in the traditional sense.

* **Training data:** AI systems learn from data. If that data is biased or unrepresentative, the outputs will reflect those flaws. Who is liable: the team that collected the data, the team that built the model, or the group that deployed it without adequate testing?

* **Evolving behavior:** Some AI systems continue to learn after deployment. A system that performs well during testing may behave differently after months of industry-relevant interaction, challenging the assumption that product behavior is fixed at the time of sale.

* **Multiple parties:** A foundation model built by one firm, fine-tuned by a second, deployed by a third creates a liability chain that current law does not clearly resolve.

Groups that rush AI systems to market without adequate testing are making the same ethical error as those that ship software with known defects: transferring risk to users for their own benefit.

### AI-Assisted Development and Human Review

An AI coding assistant can produce useful code and insecure code. A successful build does not prove that the output handles authorization, input validation, cryptography, errors, or unusual conditions safely.

The [NIST Secure Software Development Framework](https://csrc.nist.gov/pubs/sp/800/218/final) calls for security requirements, protected development environments, software verification, and a process for responding to vulnerabilities. It provides a common structure for secure development. [CISA's product security guidance](https://www.cisa.gov/news-events/alerts/2025/01/17/cisa-and-fbi-release-updated-guidance-product-security-bad-practices) places responsibility on software manufacturers to reduce customer risk.

AI-generated code belongs inside the same review process. Record where it came from, inspect it, test security assumptions, and confirm any license obligations. A developer cannot treat the tool's confidence as evidence of correctness.


### Try It Yourself 7.3: Test Your First Judgment 🛠️

**Predict:** Self-driving vehicle firms argue that autonomous cars do not need to be perfect. They only need to be safer than human drivers. If a self-driving car is statistically involved in fewer accidents per mile than a human driver, is that sufficient to justify deployment, even knowing that the AI will still cause some deaths? Who should make that choice: the firm, government regulators, or the public? And if an autonomous vehicle does cause a death, who should be held liable: the manufacturer, the software developer, the owner, or no one?

**Run:** Apply the main framework or choice test from Section 7.3. Identify the stakeholder whose interest carries the most weight.

**Explain:** In 1-2 sentences, state whether the structured test confirmed or changed your first judgment.

### Try It Yourself 7.4: Test the Boundary 🛠️

**Predict:** Which option in this section creates the least ethical risk?

**Run:** Apply one ethical framework and one stakeholder test from Section 7.4.

**Explain:** Defend your result with one fact from the section.

### Quick Check 7.4 ✅

1. Explain the formula "Risk = Likelihood x Impact" and give an example of an IT risk case where a low-likelihood, high-impact threat should receive priority attention. *(Apply)*

2. The Ford Pinto case involved a firm calculating that paying for injuries was cheaper than fixing a defect. Identify a parallel ethical risk in IT cost/benefit analysis and explain why the same logic is ethically problematic in a technology context. *(Analyze)*

3. An AI-powered hiring tool is found to systematically rank female candidates lower than male candidates with identical qualifications. Using the AI liability concepts from this section, identify at least two parties who might bear responsibility and explain why assigning liability is more complex for AI than for traditional software. *(Evaluate)*

---

## 7.5 Summary and Retrieval 💡

### Key Concepts

* **Software defects cause real harm.** From the Therac-25 radiation deaths to the 2024 CrowdStrike global outage, software failures range from financial disruption to loss of life. Ethical responsibility extends beyond writing functional code to writing safe, reliable, and secure code.

* **Product liability law applies unevenly to software.** Negligence, strict liability, and breach of warranty provide frameworks for accountability, but the product-vs.-service distinction and EULA protections leave significant gaps. Software vendors often enjoy less legal accountability than manufacturers of physical products.

* **Software quality is an ethical obligation.** Development methodologies (waterfall, agile, DevOps) shape quality outcomes. CMMI provides a maturity framework for assessing organizational capability. Technical debt transfers risk from groups to users when shortcuts are taken without plans to address them.

* **Secure coding prevents foreseeable harm.** Vulnerabilities like SQL injection, XSS, and authentication flaws are well-understood and preventable. Responsible disclosure, patch management, and ongoing security maintenance are ethical obligations throughout a product's lifecycle.

* **Cost/benefit analysis requires ethical guardrails.** Financial calculations that reduce human safety and privacy to dollar figures are incomplete and potentially dangerous. When failure means serious harm, "good enough" is not good enough.

* **AI-assisted development does not remove human review.** Opacity, biased training data, evolving behavior, and multi-party supply chains complicate responsibility. Teams should document AI use, apply secure development practices, test outputs, and name who can approve or reject generated code.

### Key Terms

* Software defect (bug)
* Product liability
* Negligence
* Strict liability
* Breach of warranty
* End User License Agreement (EULA)
* Software as a Service (SaaS)
* Software quality
* Capability Maturity Model Integration (CMMI)
* Technical debt
* Secure coding
* OWASP Top 10
* SQL injection
* Cross-site scripting (XSS)
* Responsible disclosure
* Patch management
* Risk assessment
* Cost/benefit analysis
* Safety-critical system
* AI liability
* Orchestrator-verifier

### Retrieval Practice

Try to answer these from memory before looking back at the chapter.

1. Name and explain the three product liability theories that can apply to software failures. For each one, give an example of a software case where that theory would most likely apply.

2. What is technical debt, and why is it an ethical concern instead of just a technical or business concern?

3. Explain why assigning liability for AI-caused harm is more complex than assigning liability for traditional software failures. Identify at least two factors that complicate AI liability.

---

## 7.6 Skills Lab 7A: Software Liability and Cost/Benefit Analysis

**Goal:** Evaluate a software release choice and assign responsibility for preventable harm.

**Evidence packet:** `assets/code/chapter-07/software-liability-case.md`, a fictional case and evidence packet created for this textbook.

**Estimated time:** 90-120 minutes

### Case: The AutoPilot Express Choice

TransitTech Inc. develops software for autonomous public transit buses operating in Phoenix, Arizona. Their system, AutoPilot Express, has been in pilot testing on two routes for 18 months. The pilot has been largely successful: the buses have completed over 50,000 trips with no serious incidents.

TransitTech is now pursuing a major contract with Valley Metro to expand AutoPilot Express to 15 additional routes across the metropolitan area. The contract is worth $45 million over five years and would make TransitTech the first firm to operate autonomous transit at this scale in the United States.

During final pre-deployment testing, quality assurance engineer Tomoko Hayashi identifies a pattern. In heavy monsoon rain, the sensor fusion algorithm sometimes treats large puddles as solid obstacles and brakes abruptly. In 0.3% of simulated heavy-rain cases, standing passengers would be thrown forward. In 0.05% of those cases, the braking force could cause injuries comparable to a low-speed car accident.

Tomoko's report also notes that the sensor fusion issue does not occur in light rain or dry conditions (which represent 95% of annual operating conditions in Phoenix). Fixing the issue would require a fundamental redesign of the sensor fusion algorithm, delaying deployment by 8-12 months and costing about $6 million in additional development.

TransitTech's leadership team is divided:

* **CEO Maria Santos** wants to proceed with deployment on schedule. She argues that the 0.3% occurrence rate in a condition that represents only 5% of operating days makes the actual risk extremely low. She proposes adding a policy that the buses operate in manual mode during monsoon warnings, which would reduce (but not eliminate) passenger exposure to the defect.
* **CTO James Okonkwo** wants to delay deployment to fix the sensor fusion issue. He argues that TransitTech is setting a precedent for the entire autonomous transit industry, and that a single injury could set public acceptance of autonomous vehicles back by years.
* **CFO Patricia Reeves** presents a financial analysis. An 8-12 month delay would cost $6 million in development and $3.2 million in lost revenue. It may also cost the firm the contract.
* **Tomoko Hayashi (QA engineer)** has documented the defect and presented her findings. She believes the manual mode policy is a reasonable mitigation but worries about the cases where monsoon conditions develop rapidly and buses are already in autonomous mode.

### Part 1: Foundation (Aligns with MLO-7.1)

Apply product liability concepts to this case:

1. If a passenger is injured due to the abrupt braking defect during a monsoon, which product liability theory (negligence, strict liability, or breach of warranty) would most likely apply? Explain your reasoning, referencing the fact that TransitTech knows about the defect before deployment.

2. Would the manual mode policy during monsoon warnings change the liability analysis? Why or why not?

3. Identify whether AutoPilot Express should be classified as a safety-critical system. Reference the characteristics of safety-critical systems discussed in Section 7.4 to support your answer.

### Part 2: Application (Aligns with MLO-7.1, MLO-7.2)

Analyze the ethical obligations of the development team and group:

4. Evaluate the quality of TransitTech's development process. Based on what you know about the case, what CMMI maturity level (1-5) does their process most closely resemble? Justify your assessment.

5. Consider Tomoko's position. She has reported the defect to leadership and they have acknowledged it. Does she have any further ethical obligation? If TransitTech proceeds with deployment over her objections, what options does she have? Reference the whistleblowing concepts from Chapter 5 if relevant.

6. Analyze the CEO's proposed mitigation (manual mode during monsoon warnings). Is this an adequate response to the identified risk, or is it a rationalization that allows the firm to proceed while shifting risk to passengers? Explain your reasoning.

### Part 3: Extension (Aligns with MLO-7.2, MLO-7.3)

Evaluate the cost/benefit trade-offs and formulate a recommendation:

7. Construct a cost/benefit analysis that includes both the financial costs (delay, development expense, lost revenue) and the non-financial costs (passenger safety risk, public trust, industry precedent, legal liability). Which factors are most difficult to quantify, and why does that difficulty matter for ethical choice-making?

8. Write a recommendation (200-300 words) to TransitTech's board of directors. State whether they should deploy on schedule, deploy with the manual mode mitigation, or delay to fix the defect. Support your recommendation with at least two ethical frameworks and reference specific concepts from this chapter.

### Questions & Analysis 🤔

1. Which party should bear the greatest responsibility if the system causes harm?
2. What risk threshold would make postponing release ethically required?

### Rubric: Skills Lab 7A

This lab is graded with the standard
[Skills Lab Rubric](../skills-lab-rubric.md): four criteria at
4 points each, 16 points total. The criteria are Technical Accuracy
and Efficiency, Output Quality, Documentation Quality, and Analysis,
Interpretation, and Response to QUESTION(s).

### Submission Guidelines

* **Length:** 800-1,200 words total across all parts
* **Format:** Submit as a single document organized by part number. Use clear headings for each section.

---

## 7.7 Review Questions 🔄️

1. Distinguish negligence, strict liability, and warranty claims in a software case.
2. Apply secure coding duties to a known vulnerability that lacks a patch.
3. Analyze which stakeholders should bear the cost of delayed security maintenance.
4. Should failure to install a known critical patch create strict liability? Defend your answer with a cost/benefit analysis.

## Further Reading 📖

* [NIST Secure Software Development Framework](https://csrc.nist.gov/pubs/sp/800/218/final) - NIST defines secure development practices across the software life cycle.
* [CISA Product Security Bad Practices](https://www.cisa.gov/news-events/alerts/2025/01/17/cisa-and-fbi-release-updated-guidance-product-security-bad-practices) - CISA and the FBI identify practices software makers should avoid.
* [FTC Equifax Data Breach Settlement](https://www.ftc.gov/enforcement/refunds/equifax-data-breach-settlement) - The FTC summarizes the breach settlement and consumer relief.
* [ACM Code of Ethics and Professional Conduct](https://www.acm.org/about-acm/code-of-ethics) - ACM principles 2.1 and 2.5 address quality and system risk evaluation.
## Looking Ahead ⏩

In Chapter 8, you will shift from the obligations of those who build software to the role of governments and professional groups in regulating IT. You will examine major regulations such as GDPR, CCPA, COPPA, and HIPAA, evaluate the tension between government regulation and industry self-regulation, and explore the ethical dimensions of H-1B visa programs and offshore outsourcing. The question changes from "What should developers do?" to "What should society require?"
