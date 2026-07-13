# Chapter 12: Professional Codes of Ethics and Capstone

In 2018, thousands of Google staff signed a petition demanding the firm withdraw from Project Maven, a U.S. Department of Defense contract that used AI to analyze drone surveillance footage. The staff argued that building tools to improve military targeting violated Google's own stated principle of "Don't be evil." Google eventually chose not to renew the contract. But the controversy raised a question that no worker handbook fully answered: when your employer asks you to build something you believe causes harm, what should you do? The professional codes of ethics that guide IT workers offer some answers, but as you will see in this chapter, those answers are not always as clear or as complete as the situations demand.

This is the final chapter in the CIS111 textbook. Across the first eleven chapters, you built an ethical reasoning toolkit with moral frameworks, law, stakeholder analysis, and professional judgment. You applied those tools to corporate governance, social media, healthcare, intellectual property, cybersecurity, and other IT topics. Now you will examine the formal codes that guide IT workers. You will study the ACM, IEEE, and (ISC)² codes. You will compare their common ground, differences, and limits when applied to emerging technology such as AI.

This chapter also includes a capstone Skills Lab. It brings ideas from all twelve chapters into one original ethical analysis. You can complete it whenever you are ready to combine the book's reasoning tools.

## Module Overview 🧭

* **Estimated time:** 5-6 hours (reading + activities + capstone)
* **Prerequisites:** Chapters 1-11
* **Deliverables:** Try It Yourself activities, Quick Checks, Skills Lab 12A

## Learning Objectives 🎯

By the end of this chapter, you will be able to:

* **MLO-12.1 (Analyze):** Analyze the key principles, obligations, and enforcement mechanisms of the ACM, IEEE, and (ISC)² codes of ethics
* **MLO-12.2 (Evaluate):** Evaluate the strengths and gaps of professional codes of ethics when applied to emerging technology challenges including AI
* **MLO-12.3 (Create):** Synthesize ethical theories, professional obligations, legal frameworks, and AI ethics concepts from across the course into an original ethical analysis of an industry-relevant IT scenario

### This chapter aligns with the following Course Learning Outcomes

* **CLO XVII.** Critique professional codes of ethics for Information Technology professionals.

---

## 12.1 Professional Codes of Ethics in IT

When you become a doctor, you take the Hippocratic Oath. When you pass the bar exam, you swear to uphold professional conduct rules. But when you start working in IT, there is no single oath, no universal licensing requirement, and no one code that every practitioner must follow. Instead, IT professionals look to voluntary codes published by professional groups. These codes define what ethical practice looks like and set expectations for how members should behave.

In this section, you will examine the three most influential professional codes in IT and cybersecurity.

### The ACM Code of Ethics and Professional Conduct

The **ACM Code of Ethics and Professional Conduct** was most recently updated in 2018. The ACM is the world's largest computing society, with over 100,000 members, and its code applies broadly to anyone working in computing, from software developers to data scientists to IT managers.

The code is organized around four sections:

* **General Ethical Principles (Section 1):** These address fundamental obligations. Members should support human well-being, avoid harm, act honestly, treat people fairly, respect intellectual work, protect privacy, and honor confidentiality.
* **Professional Responsibilities (Section 2):** These focus on how computing professionals should work. Members should pursue quality, maintain competence, respect rules, accept professional review, evaluate systems and their effects, and work only within their competence. They should also support public understanding and access computing resources only with authorization.
* **Professional Leadership Principles (Section 3):** These apply to members in leadership roles. Leaders should center the public good, protect user dignity, support a healthy working life, and establish processes that enable ethical work.
* **Compliance with the Code (Section 4):** This section addresses how the code should be upheld, such as that members should treat violations as inconsistent with membership in the ACM.

What makes the ACM code distinctive is its breadth. It does not limit itself to technical matters. It explicitly addresses social harm, discrimination, privacy, and the public good. It also requires members to consider the full impact of their systems on all stakeholders, not just the people who pay for the work.

### The IEEE Code of Ethics

The **IEEE Code of Ethics** comes from the world's largest technical professional group, with over 400,000 members across engineering, computing, and related fields. The IEEE's roots are in electrical engineering, so its code reflects an engineering mindset focused on safety, competence, and honest representation.

The IEEE code consists of ten commitments that members pledge to uphold. These include commitments to:

* Hold paramount the safety, health, and welfare of the public
* Avoid real or perceived conflicts of interest whenever possible
* Be honest and realistic in stating claims or estimates based on available data
* Reject bribery in all its forms
* Improve the understanding of technology and its appropriate application
* Maintain and improve technical competence
* Treat all persons fairly and not engage in acts of discrimination or harassment
* Avoid injuring others, their property, reputation, or employment by false or malicious action
* Assist colleagues in their professional development and support them in following the code

The IEEE code is shorter and more principle-based than the ACM code. It reads more like a set of professional pledges than a detailed guideline. Its strength is clarity: the commitments are direct and easy to remember. Its limitation is that it provides less specific guidance for the kinds of complex cases you have studied throughout this book, such as algorithmic bias, surveillance, or AI governance.

### The (ISC)² Code of Ethics

The **(ISC)² Code of Ethics** serves cybersecurity professionals, such as those who hold the Certified Information Systems Security Professional (CISSP) certification. Unlike the ACM and IEEE codes, which are voluntary for members, the (ISC)² code is a condition of certification. If you violate it, you can lose your CISSP credential.

The (ISC)² code is built on four mandatory canons, listed in order of priority:

1. **Protect society, the common good, necessary public trust and confidence, and the infrastructure.** This canon comes first because security professionals hold positions of significant trust. Your choices affect whether systems stay secure and whether people's data stays protected.
2. **Act honorably, honestly, justly, responsibly, and legally.** This covers personal integrity and compliance with laws and regulations.
3. **Provide diligent and competent service to principals.** "Principals" means the people and groups you work for. This canon obligates you to perform your duties competently and faithfully.
4. **Advance and protect the profession.** Members should maintain and expand their skills, and avoid actions that damage the reputation of the security profession.

The priority ordering is critical. When canons conflict, you resolve the conflict by following the higher-ranked canon. For example, if your employer asks you to cover up a data breach (Canon 3: serve your principal), the (ISC)² code says you must prioritize Canon 1 (protect society and public trust) instead. This gives security professionals explicit authorization to push back against unethical instructions.


### Try It Yourself 12.1: Test Your First Judgment 🛠️

**Predict:** Imagine you hold a CISSP certification and your employer tells you to delay notifying customers about a data breach until after a major product launch. The (ISC)² code ranks protecting society above serving your employer. How does having that explicit priority ordering change how you would handle the situation compared to not having a code at all?

**Run:** Apply the main framework or choice test from Section 12.1. Identify the stakeholder whose interest carries the most weight.

**Explain:** In 1-2 sentences, state whether the structured test confirmed or changed your first judgment.

### Quick Check 12.1 ✅

1. What are the four main sections of the ACM Code of Ethics? Briefly describe the focus of each. *(Remember)*

2. How does the (ISC)² code's priority ordering of its four canons help resolve conflicts between a security professional's obligations to different stakeholders? *(Understand)*

3. The IEEE code commits members to "hold paramount the safety, health, and welfare of the public." Give an specific IT case where following this commitment would require an engineer to push back against a business choice. *(Apply)*

---

## 12.2 Comparing and Critiquing Professional Codes

Now that you are familiar with the three major codes, the next step is to put them side by side. Understanding what these codes share helps you identify the core values of the IT profession. Understanding where they differ reveals the priorities and blind spots of each approach.

### What the Codes Share

Despite their different structures and audiences, the ACM, IEEE, and (ISC)² codes share several core commitments:

* **Public welfare comes first.** All three codes prioritize the well-being of the public over the interests of employers, clients, or the profession itself. This is the foundational principle of professional ethics: the people affected by your work matter more than the people paying for it.
* **Honesty and integrity.** Every code requires truthfulness in professional dealings. You should not misrepresent your qualifications, hide defects in your work, or deceive the people who depend on your systems.
* **Competence.** All three codes require professionals to maintain their skills and work within their areas of expertise. In a field that changes as fast as IT, this is both an ethical obligation and a practical necessity.
* **Avoiding harm.** Whether stated as "avoid harm" (ACM), "hold paramount safety" (IEEE), or "protect society" ((ISC)²), each code recognizes that IT professionals can cause significant damage and must work actively to prevent it.

### Where the Codes Differ

The differences are just as instructive as the similarities.

| Feature | ACM | IEEE | (ISC)² |
|---------|-----|------|--------|
| **Scope** | All computing professionals | Engineers and technologists | Cybersecurity professionals |
| **Structure** | 4 sections, 25 principles | 10 commitments | 4 canons (priority-ranked) |
| **Specificity** | Highly detailed with explanations | Brief and principle-based | Concise with enforcement teeth |
| **Enforcement** | Membership revocation (rare) | Limited formal enforcement | Certification revocation (active) |
| **Emerging tech** | Updated 2018 with AI awareness | General principles only | Focused on security domain |

The enforcement question matters. A code with no enforcement mechanism is aspirational: it describes what professionals *should* do. A code with real effects, like the (ISC)² code's ability to revoke your certification, is regulatory: it describes what professionals *must* do or face professional penalties.

### Gaps in Current Codes

As comprehensive as these codes are, they were not written for every challenge you will face. Several gaps are worth noting:

* **AI and algorithmic accountability.** The ACM's 2018 update references computing's impact on society broadly, but none of the three codes provide detailed guidance for professionals building, deploying, or maintaining AI systems. What is your obligation when you know an algorithm produces biased outcomes? The codes point toward "avoid harm," but they do not spell out what that means for machine learning pipelines or training data curation.
* **Global applicability.** These codes were developed primarily in a U.S. and European context. As you learned in Chapter 8, different countries have different regulatory philosophies. A professional working across borders may find that following one code conflicts with legal requirements in another jurisdiction.
* **Gig and contract workers.** In Chapter 3, you studied the gig economy and contingent workers. Most professional codes assume a traditional employment relationship. They are less clear about the obligations of freelance developers, independent consultants, or contractors who may not be ACM or IEEE members.
* **Whistleblowing guidance.** In Chapter 5, you learned about whistleblower protections and the ethical justifications for reporting wrongdoing. The codes encourage integrity and honesty but provide limited practical guidance for professionals who witness misconduct internally.

### Case Study 12.1 - The Autonomous Vehicle Ethics Board 📋

**The Situation:** Priya Sharma is a senior software engineer at AutoDrive Technologies, a firm developing autonomous vehicle software. She holds both ACM membership and a CISSP certification through (ISC)². AutoDrive has been testing its self-driving system in several U.S. cities.

During internal testing, Priya's team discovers that the vehicle's object-detection algorithm performs significantly worse in low-light conditions, particularly when identifying pedestrians with darker skin tones. The error rate for detecting light-skinned pedestrians is 2%, but for darker-skinned pedestrians it is 11%. The lead product manager, David Chen, acknowledges the disparity but argues that the overall safety record is still better than human drivers. He wants to proceed with a planned public launch in three months. "We'll patch it in a future update," he says. "If we delay, our competitor launches first and we lose our market position."

Priya raises the issue at a team meeting, citing the ACM code's principle to avoid harm and its requirement to be fair and nondiscriminatory. David responds that the (ISC)² code requires her to provide competent service to her principal, meaning AutoDrive. Another engineer, Marcus Williams, suggests they bring the issue to AutoDrive's newly formed AI Ethics Board, but notes that the board is advisory and its recommendations are not binding.

**Stakeholders:**

* **Priya Sharma** wants to ensure the system is safe and nondiscriminatory before launch, even if it means delaying the product
* **David Chen** wants to meet the launch timeline and maintain AutoDrive's competitive position, planning to address the disparity in future updates
* **Marcus Williams** hopes the Ethics Board can mediate, but is unsure whether a non-binding recommendation will change anything
* **Pedestrians and the public** are the people most directly affected, particularly those in communities where the detection gap poses a greater safety risk
* **AutoDrive investors and leadership** have financial interests tied to the launch timeline

**Questions to Consider:**

1. Priya holds membership in both ACM and (ISC)². How would each code guide her in this situation? Where do the codes agree, and is there any point where following one might create tension with the other?

2. David argues that the system is still safer than human drivers overall. Using the utilitarian and deontological frameworks from Chapter 1, evaluate whether this argument justifies launching with the known detection disparity.

3. If you were Priya, what would you do next? Identify which professional code principles and which ethical frameworks from this book support your choice.


### Try It Yourself 12.2: Test Your First Judgment 🛠️

**Predict:** Advisory ethics boards are becoming common at tech firms. If an ethics board has no authority to block a product launch, does it serve a meaningful purpose? What would make an internal ethics review process genuinely effective?

**Run:** Apply the main framework or choice test from Section 12.2. Identify the stakeholder whose interest carries the most weight.

**Explain:** In 1-2 sentences, state whether the structured test confirmed or changed your first judgment.

### Quick Check 12.2 ✅

1. Name two ethical commitments that appear in all three major IT professional codes (ACM, IEEE, (ISC)²). *(Remember)*

2. The (ISC)² code has active enforcement through certification revocation, while the ACM code relies primarily on membership expectations. Explain how this difference in enforcement affects the practical impact of each code. *(Analyze)*

3. Identify one gap in current professional codes that you believe is most significant for IT professionals entering the workforce today. Explain why this gap matters. *(Evaluate)*

---

## 12.3 IT Licensing, Certification, and Professional Accountability

Engineers who design bridges must be licensed. Doctors must pass board exams. Lawyers must pass the bar. But the software engineer who builds the banking app on your phone, the database administrator who manages your health records, and the network engineer who secures your firm's infrastructure? In most cases, they need no license at all. This section examines the ongoing debate about whether IT professionals should be subject to licensing requirements and how certification currently fills part of that gap.

### The Case for IT Licensing

Advocates for **professional licensing** in IT argue that the stakes are now too high for self-regulation alone. Consider the systems that IT professionals build and maintain:

* Healthcare systems where errors can lead to misdiagnosis or incorrect medication
* Financial systems that process billions of dollars in transactions daily
* Critical infrastructure such as power grids, water treatment facilities, and transportation networks
* AI systems that make consequential choices about hiring, lending, criminal sentencing, and medical treatment

When a bridge collapses, we hold the licensed engineer accountable. When a software failure causes comparable harm, the accountability structure is less clear. Licensing advocates argue that requiring IT professionals to meet minimum competency standards, pass examinations, and maintain their credentials through continuing education would strengthen public protection.

In Chapter 7, you studied software liability and the question of who bears responsibility when software fails. Licensing would create a clearer chain of accountability. A licensed professional who acts negligently could face effects beyond just losing a job.

### The Case Against IT Licensing

Critics of IT licensing raise several practical and philosophical objections:

* **The field changes too fast.** A licensing exam reflects knowledge at a single point in time. In IT, tools, languages, and best practices shift rapidly. A license earned five years ago may not reflect current competence.
* **Barriers to entry.** IT is one of the few high-paying fields that remains accessible to people without traditional four-year degrees. Licensing requirements could create barriers that disproportionately affect self-taught professionals, career changers, and people from lower-income backgrounds.
* **Scope is too broad.** "IT professional" covers everything from help desk support to machine learning research. Creating a single licensing framework for such a diverse field is impractical. Medicine and law have clearer boundaries around what practitioners do.
* **Innovation could slow.** Some argue that licensing creates bureaucratic overhead that slows the pace of innovation. Open source software, for example, thrives on contributions from people with diverse backgrounds and training, many of whom would not hold traditional credentials.

### Certification as Professional Accountability

In the absence of licensing, **professional certifications** serve as the primary mechanism for demonstrating competence and commitment to ethical standards. Unlike licenses, certifications are voluntary (though many employers require them). Unlike academic degrees, certifications typically require periodic renewal, which ensures ongoing competence.

Some of the most recognized IT certifications include:

* **CompTIA A+, Network+, Security+:** Entry-level and mid-level certifications covering hardware, networking, and cybersecurity fundamentals. You may already be familiar with these from other courses at Phoenix College.
* **CISSP (Certified Information Systems Security Professional):** An advanced cybersecurity certification from (ISC)² that requires both passing an exam and agreeing to the (ISC)² Code of Ethics. As you learned in Section 12.1, violating the code can result in losing the certification.
* **Certified Ethical Hacker (CEH):** A certification focused on penetration testing and security assessment, which explicitly ties ethical behavior to professional practice.
* **AWS, Azure, and Google Cloud certifications:** Vendor-specific certifications that validate cloud computing skills, increasingly important as groups migrate to cloud infrastructure.
* **Project Management Professional (PMP):** While not IT-specific, this certification is widely held by IT project managers and includes its own code of ethics.

Certifications create a form of **professional accountability** that sits between voluntary codes and mandatory licensing. If you hold a CISSP and act unethically, you can lose your credential, which has real career effects. But certifications do not carry the legal weight of a license, and many IT workers hold no certifications at all.


### Try It Yourself 12.3: Test Your First Judgment 🛠️

**Predict:** In Chapter 2, you learned about the ethical responsibilities of IT workers across six professional relationships. Do you think a formal licensing requirement would make IT professionals more accountable in those relationships, or would it simply add bureaucracy without changing behavior? What evidence from your own experience supports your view?

**Run:** Apply the main framework or choice test from Section 12.3. Identify the stakeholder whose interest carries the most weight.

**Explain:** In 1-2 sentences, state whether the structured test confirmed or changed your first judgment.

### Quick Check 12.3 ✅

1. List two arguments in favor of IT professional licensing and two arguments against it. *(Remember)*

2. How does the CISSP certification create a form of professional accountability that goes beyond a voluntary code of ethics? *(Understand)*

3. A state legislature is debating whether to require licensing for any IT professional who works on healthcare systems. Using concepts from this chapter and Chapter 6 (Healthcare IT Ethics), evaluate whether this proposal would improve patient safety. *(Evaluate)*

---

## 12.4 Ethics for Emerging Technologies and AI

Throughout this book, you have encountered AI in many settings. Examples include algorithmic bias, recommendation systems, clinical tools, software liability, regulation, intellectual property, synthetic media, and cyberattacks. This final content section connects those topics. You will examine professional ethics for people who build, deploy, and maintain AI systems.

### Applying Ethical Frameworks to Emerging Technologies

The ethical frameworks you learned in Chapter 1 were developed long before anyone imagined autonomous vehicles, gene editing, or large language models. But that is precisely their value. Ethical theories give you tools for reasoning about problems that have not been solved yet. Here is how each framework applies to emerging technologies:

* **Utilitarianism** asks: Does this technology produce more benefit than harm? For whom? This is the framework behind cost-benefit analyses of AI deployment, the same kind of analysis you practiced in Chapter 7 when studying software liability.
* **Deontology** asks: Does this technology respect people's rights and dignity? Are we treating people as ends in themselves, or merely as means? This framework challenges practices like collecting training data without consent or using AI to make choices that should require human judgment.
* **Virtue ethics** asks: What kind of professionals and groups are we becoming? Are we building technology that reflects integrity, fairness, and responsibility? This framework is especially relevant for organizational culture and the character of technical teams.
* **Social contract theory** asks: Would the people affected by this technology agree to its use if they had a voice? Use Chapter 1's veil of ignorance to test an AI system. Would you approve the design without knowing whether you would be its user, subject, or displaced worker?

### Applying Professional Codes to AI

The [ACM Code of Ethics](https://www.acm.org/about-acm/code-of-ethics) requires professionals to support the public good, avoid harm, be honest, respect privacy, and evaluate system risks. The [IEEE Code of Ethics](https://www.ieee.org/about/corporate/governance/p7-8.html) emphasizes public safety, honest claims, fairness, and disclosure of conflicts. The [ISC2 Code of Ethics](https://www.isc2.org/Ethics) places protection of society and public trust before service to a principal.

These codes do not need to name every AI tool to apply. They give you duties that can be tested against a system's purpose, evidence, limits, and effects. NIST's AI framework adds a process for governing, mapping, measuring, and managing risk.

For AI work, apply the codes through four professional obligations:

* **Transparency.** Tell affected people when AI has a meaningful role and explain the choice at a useful level. Legal disclosure duties depend on the system and jurisdiction. Professional honesty may require more than the legal minimum.
* **Bias testing and fairness.** Test outcomes across affected groups and document the evidence. The [EEOC](https://www.eeoc.gov/newsroom/us-eeoc-and-us-department-justice-warn-against-disability-discrimination) explains that employment software can create unlawful disability barriers.
* **Human oversight.** For consequential choices (hiring, lending, medical treatment, criminal justice), professional ethics requires that humans remain in the choice loop. AI can inform choices, but removing human judgment from high-stakes outcomes raises serious ethical concerns. Your obligation as a professional includes designing workflows that preserve meaningful human review, not just nominal sign-off.
* **Accountability and documentation.** Record what the system was meant to do, how it was tested, who approved it, and who can stop it. When harm occurs, the group needs enough evidence to reconstruct the choice and correct the process.

### AI Touchpoint: What to Do When Asked to Build Something Harmful

This is the question that the Google Project Maven staff faced, and it is a question you may face in your own career. Professional codes provide some guidance. The ACM code says to avoid harm. The IEEE code says to hold paramount the safety of the public. The (ISC)² code prioritizes protecting society over serving your employer. But codes are general. Real situations are specific and messy.

Here is a practical framework for IT professionals who find themselves asked to build or maintain something they believe causes harm:

1. **Clarify the concern.** Make sure your objection is based on a genuine ethical issue, not just personal discomfort or disagreement with a business strategy. Use the ethical frameworks from Chapter 1 to articulate what principle is at stake.
2. **Raise the issue internally.** Start with your direct supervisor or team lead. Document your concern in writing. Reference specific provisions of your professional code if you hold one. In Chapter 2, you studied the importance of the relationship between IT workers and employers. Raising concerns through proper channels respects that relationship.
3. **Escalate if necessary.** If your concern is dismissed, escalate to higher management, an ethics officer, or an internal review board. Many groups now have AI ethics committees or responsible-AI teams.
4. **Consult external resources.** If internal escalation fails, consider consulting your professional group, a trusted mentor, or a legal advisor. Chapter 5 covered whistleblower protections. Those protections may apply depending on the nature of the harm.
5. **Make a choice you can stand behind.** In some cases, you may decide that the group's direction is incompatible with your professional and ethical obligations. Resignation is always an option, and in extreme cases, external disclosure may be justified under the whistleblowing frameworks you studied in Chapter 5.

This is not a clean, comfortable process. Ethical dilemmas in professional life rarely are. But having a structured approach, grounded in professional codes and ethical frameworks, is far better than improvising under pressure.


### Try It Yourself 12.4: Test Your First Judgment 🛠️

**Predict:** The practical framework above describes raising ethical concerns internally before considering external action. What factors might make a professional decide to skip internal escalation and go directly to external disclosure? Under what circumstances would that be ethically justified?

**Run:** Apply the main framework or choice test from Section 12.4. Identify the stakeholder whose interest carries the most weight.

**Explain:** In 1-2 sentences, state whether the structured test confirmed or changed your first judgment.

### Quick Check 12.4 ✅

1. Choose one ethical framework from Chapter 1 and explain how it applies to the development of AI systems that make hiring choices. *(Apply)*

2. The ACM and IEEE have both issued statements on AI ethics. Why are group-specific AI ethics statements necessary if the general professional codes already require members to avoid harm? *(Analyze)*

3. A junior developer at a social media firm discovers that the firm's recommendation algorithm promotes content that increases user engagement but also increases anxiety and depression among teenage users. Using the five-step framework from this section, outline what this developer should do. *(Evaluate)*

---

## 12.5 Summary and Retrieval 💡

### Key Concepts

* **Professional codes of ethics** provide IT practitioners with formal guidance on ethical behavior. The ACM, IEEE, and (ISC)² codes share core commitments to public welfare, honesty, competence, and avoiding harm, but they differ in scope, structure, specificity, and enforcement.

* **Enforcement mechanisms** determine whether a code is aspirational or regulatory. The (ISC)² code carries real effects through certification revocation, while the ACM and IEEE codes rely more heavily on professional norms and peer expectations.

* **Gaps in current codes** include limited guidance on AI-specific challenges, global applicability, gig economy workers, and practical whistleblowing. As technology evolves, professional codes must evolve with it.

* **IT licensing versus certification** represents an ongoing debate. Licensing would create stronger accountability structures but could raise barriers to entry and slow innovation. Certifications like CISSP, CompTIA, and CEH provide a middle ground by tying professional credentials to ethical commitments.

* **Ethical obligations for emerging technologies** require IT professionals to apply the frameworks from Chapter 1 to new challenges. Transparency, bias testing, human oversight, and accountability are core obligations for professionals working with AI systems.

* **When asked to build something harmful,** IT professionals can follow a structured approach: clarify the concern, raise it internally, escalate if needed, consult external resources, and make a principled choice.

### Key Terms

#### Section 12.1

* ACM Code of Ethics
* IEEE Code of Ethics
* (ISC)² Code of Ethics
* Canon

#### Section 12.2

* Aspirational code
* Regulatory code
* Algorithmic transparency

#### Section 12.3

* Professional licensing
* Professional certification
* CISSP

#### Section 12.4

* AI ethics
* Human oversight
* Responsible AI

### Retrieval Practice

Try to answer these from memory before looking back at the chapter.

1. Name the three professional codes of ethics discussed in this chapter and identify one key structural difference between them.
2. What are the four canons of the (ISC)² Code of Ethics, and why does their priority ordering matter?
3. Describe three arguments for and against licensing IT professionals. Which side do you find more persuasive, and why?
4. If an IT professional is asked to build a system they believe causes harm, what five steps should they consider?

---

## 12.6 Skills Lab 12A: Capstone Project

**Goal:** Create a defensible ethical analysis that integrates frameworks from across the book.

**Evidence packet:** `assets/code/chapter-12/capstone-case-builder.md`, a case-planning guide created for this textbook.

This capstone draws on all twelve chapters. Other Skills Labs focus on one chapter. This one asks you to find ethical issues, apply several frameworks, consider stakeholder views, and defend a recommendation.

### Choosing Your Case

Select one of the following cases, or propose your own (subject to instructor approval):

**Case A: The Predictive Healthcare AI**
A large hospital network is deploying an AI system that predicts which patients are most likely to miss follow-up appointments. The system flags these patients for additional outreach, such as automated phone calls and text reminders. Early results show the system improves follow-up rates by 25%. However, an internal audit reveals that the system disproportionately flags patients from low-income zip codes and patients of color, resulting in those groups receiving significantly more automated contacts. Some patients report feeling surveilled and harassed. The hospital must decide whether to continue, modify, or discontinue the system.

**Case B: The AI-Powered Hiring Platform**
A mid-size technology firm adopts an AI hiring tool that screens resumes and conducts initial video interviews. The tool scores facial expressions, vocal tone, and word choice. The hiring manager says it cuts time-to-hire by 40%. Several rejected candidates describe the system as dehumanizing. An external researcher also reports that similar tools may underrate candidates with disabilities or those who speak English as a second language. The firm must decide how to respond.

**Case C: The Smart City Surveillance System**
A city government proposes installing an integrated "smart city" system that combines traffic cameras, license plate readers, environmental sensors, and public Wi-Fi location tracking. The system would improve traffic flow, reduce emergency response times, and monitor air quality. A technology firm would build and maintain the system in exchange for access to anonymized data for product development. Civil liberties groups argue the system creates a mass surveillance infrastructure that could be misused by future administrations. The city council is voting next month.

**Case D: Your Own Case (Instructor Approval Required)**
Propose a complex IT ethics case based on current events or emerging technology. Your case must involve at least three stakeholder groups and concepts from at least four chapters. It must present a genuine ethical dilemma with no obvious answer.

### Part 1: Foundation (Aligns with MLO-12.1)

1. **Describe the ethical context.** In 300-400 words, summarize the case and identify its main ethical tension. What values or principles are in conflict?
2. **Identify stakeholders.** List all significant stakeholders and describe each one's interests, concerns, and what they stand to gain or lose.
3. **Map the case to book concepts.** Identify at least four relevant concepts, frameworks, or topics from the book. Explain why each one matters. Examples include ethical theories, professional obligations, corporate governance, privacy, software liability, regulation, intellectual property, free expression, cybersecurity, and professional codes.

### Part 2: Application (Aligns with MLO-12.1, MLO-12.2)

4. **Apply two ethical frameworks.** Choose two of the four ethical frameworks from Chapter 1 (utilitarianism, deontology, virtue ethics, social contract theory). Apply each to the case separately. What does each framework recommend? Where do they agree or disagree?
5. **Apply a professional code.** Choose one professional code (ACM, IEEE, or (ISC)²) and identify the specific provisions that apply to this case. How would a member of that group be expected to act?
6. **Conduct stakeholder analysis.** For at least three stakeholders, analyze the case from their perspective. What does each stakeholder value most? What trade-offs would each be willing to accept?

### Part 3: Extension (Aligns with MLO-12.2, MLO-12.3)

7. **Formulate a recommendation.** In 400-500 words, state and defend how the central choice should be resolved. Use at least two ethical frameworks, one professional code, and one legal or regulatory concept from the book. Address the strongest counterargument to your position.
8. **Professional reflection.** In 200-250 words, reflect on your growth as an ethical thinker while using this book. How has your approach to IT ethics changed? Which frameworks do you find most useful? What questions remain?

### Questions & Analysis 🤔

1. Which professional code offers the strongest guidance for your chosen case, and where does it fall short?
2. Which book concept changed your initial position most during the analysis?

### Rubric: Skills Lab 12A

This lab is graded with the standard
[Skills Lab Rubric](../skills-lab-rubric.md): four criteria at
4 points each, 16 points total. The criteria are Technical Accuracy
and Efficiency, Output Quality, Documentation Quality, and Analysis,
Interpretation, and Response to QUESTION(s).

### Submission Guidelines

* **Length:** 1,500-2,000 words total across all parts
* **Format:** Submit as a single document organized by part number (Part 1, Part 2, Part 3) with clear headings for each numbered item
* **Citations:** Reference specific chapter concepts, frameworks, and professional code provisions by name. Include any external sources you consult.

---

## 12.7 Review Questions 🔄️

1. Compare the public-interest duties in the ACM, IEEE, and (ISC)² codes.
2. Apply one code provision to an employer request that could harm users.
3. Evaluate one gap in current professional codes for an emerging technology.
4. Propose one code revision and explain how it would change a professional choice.

## Further Reading 📖

* [ACM Code of Ethics and Professional Conduct](https://www.acm.org/about-acm/code-of-ethics) - ACM provides principles, professional duties, leadership duties, and enforcement.
* [IEEE Code of Ethics](https://www.ieee.org/about/corporate/governance/p7-8.html) - IEEE states ethical duties for engineers and technology professionals.
* [ISC2 Code of Ethics](https://www.isc2.org/Ethics) - ISC2 lists four mandatory canons and its complaint process.
* [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework) - NIST offers a current benchmark for comparing professional-code guidance on AI.
## Looking Ahead ⏩

There is no Chapter 13. The book ends here, but your ethical reasoning does not.

Over these twelve chapters, you have built a substantial toolkit. You started in Chapter 1 by learning four ethical frameworks and the critical distinction between morals, ethics, and laws. You applied those frameworks to professional relationships in Chapter 2 and corporate governance in Chapter 3. You examined social media, whistleblowing, and healthcare privacy in Chapters 4 through 6. You analyzed software liability, government regulation, and intellectual property in Chapters 7 through 9. You evaluated free expression, workplace privacy, cybersecurity, and identity theft in Chapters 10 and 11. And here in Chapter 12, you studied the professional codes that formalize these commitments and critiqued their ability to address the technologies that are reshaping the world.

The IT field will keep changing. New technology will raise questions that no one has asked yet. Rules and professional codes will take time to catch up. The reasoning skills in this book matter more than any single rule. You can find stakeholders, apply frameworks, weigh competing values, and defend a position with facts and logic. Those skills do not expire.

Carry them with you into your career. The IT profession needs people who can write secure code and build reliable systems. It needs those people even more when they can also ask, "Should we build this?" and think carefully about the answer.
