# Chapter 6: Healthcare IT Ethics

In February 2024, a ransomware attack struck Change Healthcare, a major US health technology firm. Its systems support insurance claims, pharmacy work, and payments for hospitals and clinics. The attack shut down claims processing for weeks. Physicians could not get paid. Pharmacies could not verify insurance coverage. Small practices faced a cash crisis. By January 2025, [HHS reported that the breach affected about 190 million people](https://www.hhs.gov/hipaa/for-professionals/special-topics/change-healthcare-cybersecurity-incident-frequently-asked-questions/index.html). One attack on one firm disrupted care across the country.

That incident exposed something about modern healthcare: it runs on information technology. EHRs, mobile health apps, telemedicine, clinical choice support tools, and AI-assisted diagnostics are woven into how care is delivered, documented, and paid for. Each of those systems creates ethical questions IT professionals face every day. Who has access to your health data? What happens when a clinical system gives a wrong recommendation? Is it ethical to use AI for treatment choices when the algorithm may perform differently for different populations?

This chapter examines those ethical challenges. You will learn the legal foundations of health data privacy and evaluate mobile and wireless risks in clinical settings. You will also analyze clinical IT, telemedicine, and AI in healthcare. The frameworks from Part I will help you weigh patient safety, privacy, equity, and innovation.

## Module Overview 🧭

* **Estimated time:** 4-5 hours (reading + practice + Skills Lab)
* **Prerequisites:** Chapters 1-5
* **Deliverables:** Try It Yourself activities, Quick Checks, Skills Lab 6A

## Learning Objectives 🎯

By the end of this chapter, you will be able to:

* **MLO-6.1 (Understand):** Explain the key provisions of HIPAA and the ethical foundations of health data privacy, including Protected Health Information, the Privacy Rule, and the Security Rule
* **MLO-6.2 (Apply):** Apply ethical frameworks to evaluate industry-relevant healthcare IT scenarios involving mobile health technologies, telemedicine, and clinical information systems
* **MLO-6.3 (Analyze):** Analyze the ethical challenges of operating mobile and wireless technologies in healthcare environments, including AI-assisted diagnostics and algorithmic bias in clinical settings

### This chapter aligns with the following Course Learning Outcomes

* **CLO VI.** Analyze the major ethical challenges of operating in a healthcare environment using mobile and wireless technologies.

---

## 6.1 HIPAA and the Foundations of Health Data Privacy

Health data is uniquely sensitive. Your medical records reveal diagnoses, mental health treatment, prescription medications, genetic test results, reproductive choices, and substance use history. When that information is exposed, the effects can include discrimination, stigma, job loss, and insurance denial. That sensitivity is why the United States created a specific legal framework for protecting it.

### The Health Insurance Portability and Accountability Act (HIPAA)

Congress passed the **Health Insurance Portability and Accountability Act (HIPAA)** in 1996. Its privacy and security provisions have a major impact on IT professionals. They set national standards for health data access, protection, and breach response.

HIPAA applies to **covered entities**, which include healthcare providers (hospitals, clinics, physicians), health plans (insurance firms, HMOs), and healthcare clearinghouses. It also applies to **business associates**, firms that handle health data on behalf of covered entities. Cloud storage providers, software vendors, billing firms, and IT service firms that work with healthcare groups are all business associates. If you work in IT and your firm touches health data, HIPAA applies to you.

### Protected Health Information (PHI)

**Protected Health Information (PHI)** is the core concept in HIPAA's privacy framework: any individually identifiable health information created, received, maintained, or transmitted by a covered entity or business associate. PHI includes obvious identifiers (name, address, date of birth, Social Security number) and less obvious ones (medical record numbers, health plan beneficiary numbers, biometric identifiers, photographs).

When PHI exists in electronic form, it is **electronic Protected Health Information (ePHI)**. Most health data today is ePHI, which puts IT systems directly responsible for its storage, transmission, and security.

**De-identified data** is health information stripped of HIPAA's 18 identifiers.  HIPAA does not restrict it because it cannot be traced to a specific person. However, research has shown that supposedly de-identified data can sometimes be re-identified by combining it with other sources, raising its own ethical concerns.

### The Privacy Rule

The **HIPAA Privacy Rule** governs who can access PHI and when. Its core principle is the **minimum necessary standard**: covered entities should access, use, or disclose only the minimum PHI needed for a specific purpose. A billing clerk does not need a patient's full medical history to process a claim. A researcher studying treatment outcomes does not need patient names.

The Privacy Rule grants patients specific rights:

* **Right to access:** Patients can request copies of their own records.
* **Right to amendment:** Patients can ask for corrections to inaccurate information.
* **Right to an accounting of disclosures:** Patients can find out who has accessed their records and why.
* **Right to restrict disclosures:** Patients can request limits on how their information is shared.

For IT professionals, the Privacy Rule means system design matters. Access controls, role-based permissions, audit logs, and data segmentation are the mechanisms through which patient rights are protected or violated.

### The Security Rule

Where the Privacy Rule focuses on who can access PHI, the **HIPAA Security Rule** focuses on how ePHI must be protected. It requires three categories of safeguards:

* **Administrative safeguards:** Policies, procedures, and training, such as a designated security officer, risk assessments, and staff training.
* **Physical safeguards:** Protecting the infrastructure where ePHI is stored: facility access controls, workstation security, device disposal.
* **Technical safeguards:** Technology-based protections: access controls, audit controls, integrity controls, and transmission security (encryption).

The Security Rule does not prescribe specific technologies. It requires groups to assess risks and choose "reasonable and appropriate" safeguards. The flexibility lets the rule cover everything from massive hospital systems to two-person clinics, but it also lets groups treat HIPAA as a checkbox instead of a genuine commitment to patient protection.

### Breach Notification

When PHI is compromised, HIPAA's **Breach Notification Rule** requires covered entities to notify affected people, HHS, and (for breaches affecting 500 or more) the media, within 60 days.

Penalties can be severe. Civil fines range from $100 to $50,000 per violation, up to $1.5 million per category annually. Criminal penalties include fines up to $250,000 and prison time for people who knowingly obtain or disclose PHI. The HHS Office for Civil Rights maintains a public portal of breaches affecting 500 or more, and the list has grown rapidly as healthcare has become a frequent cyberattack target.


### Try It Yourself 6.1: Test Your First Judgment 🛠️

**Predict:** You work as an IT support technician at a small medical clinic. While troubleshooting a printer issue, you see a patient's lab results on a screen. The patient is someone you know personally. HIPAA's minimum necessary standard says you should not have seen that information at all. But you did. What are your ethical obligations at this point? Does it matter whether you tell anyone what you saw?

**Run:** Apply the main framework or choice test from Section 6.1. Identify the stakeholder whose interest carries the most weight.

**Explain:** In 1-2 sentences, state whether the structured test confirmed or changed your first judgment.

### Quick Check 6.1 ✅

1. A cloud storage firm hosts patient records for a hospital. Is the cloud storage firm subject to HIPAA? Explain why or why not. *(Understand)*

2. Explain the difference between the HIPAA Privacy Rule and the HIPAA Security Rule. How do they complement each other? *(Understand)*

3. A medical researcher wants to study treatment outcomes for diabetes patients across five hospitals. The researcher does not need to know patients' names or addresses. Using the concept of the minimum necessary standard, explain how this research could be conducted in a way that respects patient privacy. *(Apply)*

---

## 6.2 Mobile Health and Wireless Technology Ethics

Healthcare is no longer confined to hospitals and clinics. **Mobile health (mHealth)** technology has expanded where and how health data is collected. The convenience brings real benefits and real ethical challenges.

### Types of mHealth Tools

mHealth runs from **consumer health apps** (the kind you download to track steps, sleep, or meals) to **regulated medical devices** (continuous glucose monitors, cardiac implants, post-surgery remote monitoring). Regulated devices meet FDA standards and generally fall under HIPAA when connected to a provider's systems. Consumer apps often fall outside both categories. A fitness tracker may collect sensitive heart-rate data around the clock. If it is not connected to a covered entity, HIPAA may not apply. The app's terms of service then govern its data practices.

The gap is large. Apps can legally sell aggregated data to insurers, employers, or advertisers. Store data on weakly secured servers. Or share with third parties, as long as the practice is disclosed somewhere in the terms.

### Wearables and Continuous Monitoring

**Wearable devices**, smartwatches, fitness bands, biosensors, are a rapidly growing category. Modern smartwatches detect irregular heart rhythms, estimate blood oxygen, track menstrual cycles, and identify falls, and have alerted users to atrial fibrillation before symptoms appeared.

Continuous monitoring means continuous data collection. A wearable that tracks location, heart rate, sleep, and activity creates a detailed picture of daily life. Shared with an employer, it could shape job choices. Shared with an insurer, premiums. The question is whether users understand what they have agreed to.

### BYOD in Clinical Settings

**Bring Your Own Device (BYOD)** policies let healthcare workers use personal smartphones and tablets for work: a nurse looking up drug interactions, a physician accessing an EHR from home. BYOD improves efficiency but creates serious security and privacy risks.

Personal devices often lack the encryption, passcode strength, or remote-wipe capability required for ePHI. They connect to unsecured Wi-Fi, are shared with family, and are lost or stolen more easily than group-issued devices. Each case is a potential HIPAA violation.

Groups balance BYOD productivity against the duty to protect patient data. Some hospitals ban personal devices entirely. Others allow BYOD with mobile device management (MDM) software that controls work-related data on the device. Bans slow care delivery.  MDM raises its own privacy concerns, since staff may object to employer control over a personal device.

### Patient Consent for Health Data Collection

Consent is foundational to healthcare ethics and data privacy, but in mHealth it is complicated by the volume of data collected and the difficulty of explaining its possible uses.

A patient agreeing to a doctor-prescribed monitoring device understands the data will go to their care team. But do they understand the manufacturer may also access it, a third-party analytics firm may process it, or that de-identified versions may be sold for research? Meaningful consent requires understanding and a genuine choice. Patients often feel they cannot refuse a technology their doctor recommends, and that power imbalance makes consent more ethically charged than in other contexts.

### Case Study 6.1 - Wellness Program Wearables at Midland Manufacturing 📋

**The Situation:** Midland Manufacturing, a firm with 2,200 staff, launches a voluntary corporate wellness program in partnership with a wearable device firm called VitaTrack. Staff who participate receive a free VitaTrack smartwatch that monitors steps, heart rate, sleep quality, and stress levels. In exchange, participating staff receive a $50 monthly reduction in their health insurance premium.

The program is framed as a benefit. Midland's HR director, Sarah Chen, promotes it at a firm meeting: "This is about helping our staff live healthier lives. The data stays with VitaTrack. We only see aggregate reports, never individual data."

Six months into the program, problems surface. Three staff report that their managers have made comments suggesting they know about specific health data. One worker, a warehouse worker named Darnell Washington, is told by his supervisor that he "might want to get more sleep" after a week of low sleep scores. Darnell did not share his sleep data with his supervisor. He files a complaint with HR.

An internal investigation reveals that VitaTrack's "aggregate reports" include department-level breakdowns with groups as small as four people. In a department with only four staff, individual data is easy to link to a person. VitaTrack's terms also allow the firm to share "anonymized insights" with Midland's HR department. The terms permit VitaTrack to use health data for "product improvement and research partnerships." This includes selling de-identified data to insurance analytics firms.

**Stakeholders:**

* **Staff who participated** expect their health data to be private and voluntarily joined based on assurances about data separation
* **Midland Manufacturing** wants to reduce healthcare costs and promote worker wellness, but faces liability for the data exposure
* **VitaTrack** profits from both the corporate contract and the secondary data market, and designed the program's data-sharing structure
* **Managers who received department reports** may have acted on health data without realizing they were violating worker privacy
* **Staff who declined to participate** may face implicit pressure to join or may be viewed as less committed to wellness

**Questions to Consider:**

1. Apply the HIPAA framework you learned in Section 6.1 to this case. Is the VitaTrack data subject to HIPAA? Why or why not? What does this tell you about the gap between legal compliance and ethical responsibility?

2. Evaluate the consent process in this case. Did the staff give meaningful, informed consent to how their data would be used? Consider the concept of power imbalance: can a wellness program offered by your employer ever be truly voluntary?

3. You are an IT professional advising Midland's leadership after the complaint. What changes would you recommend to the program's data practices, and what ethical framework supports each recommendation?

### Quick Check 6.2 ✅

1. Explain the key ethical difference between a consumer fitness app and an FDA-regulated medical device in terms of data protection. *(Understand)*

2. A hospital allows nurses to use personal smartphones to access patient records through a secure app. The hospital requires encryption and a strong passcode on any device used for this purpose. A nurse's phone is stolen from a gym locker. Apply the concept of the minimum necessary standard to evaluate this situation. *(Apply)*

3. A firm offers staff a $100 monthly bonus for sharing data from their personal fitness trackers with the firm's insurance provider. Analyze the ethical concerns with this arrangement from two stakeholder perspectives: the worker and the insurance provider. *(Analyze)*

---

## 6.3 Clinical IT Systems and Patient Safety

Inside hospitals and clinics, IT systems play a direct role in patient care. When they work, they reduce errors and save lives. When they fail, the effects fall on patients. Three clinical-IT categories carry the heaviest ethical weight, and telemedicine is rapidly expanding the reach of all three.

### Electronic Health Records (EHRs)

**Electronic Health Records (EHRs)** are digital versions of a patient's medical chart. Unlike paper charts confined to one office, EHRs can be shared across providers, pharmacies, labs, and insurance firms. A primary care physician in Phoenix can see lab results ordered by a specialist in Tucson. An ER doctor treating an unconscious patient can pull a medication list and allergy history.

EHRs reduce duplicate tests, catch dangerous drug interactions, and give providers a more complete picture of a patient's history. The federal government invested heavily through the HITECH Act of 2009, which offered financial incentives for adoption, and most hospitals and physician practices now use EHRs.

Adoption created problems. **Interoperability** is the ability of different EHR systems to exchange data. It remains a challenge. A hospital and clinic using different vendors may not share records smoothly. Patients who see several providers may still find their records fragmented.

EHRs also create **alert fatigue**. Systems generate so many drug-interaction and allergy alerts that providers override 50% to 90% of them, and the safety system itself becomes a source of risk. IT professionals who design and configure EHRs must keep alerts clinically meaningful, not so frequent they are tuned out.

### Clinical Choice Support Systems (CDSS)

A **Clinical Choice Support System (CDSS)** helps providers make clinical choices with evidence-based recommendations. It may flag lab results that suggest a condition, recommend a dose based on patient factors, or alert a provider to an updated protocol.

CDSS reduces errors and improves consistency but raises three issues. First, accountability: when CDSS gives a wrong recommendation and the provider follows it, the provider is responsible, but if the software presented inaccurate information, the vendor shares responsibility. Second, the data and rules underneath: a CDSS trained primarily on adult male patients gives less accurate recommendations for women or children. Third, **automation complacency**: heavy reliance erodes independent clinical judgment, and providers may miss what the system does not flag. CDSS supplements clinical expertise. It does not replace it.

### Computerized Provider Order Entry (CPOE)

**Computerized Provider Order Entry (CPOE)** systems let physicians enter medical orders electronically: prescriptions, labs, imaging, and treatment instructions. Before CPOE, illegible handwriting was a documented source of medication errors. CPOE eliminates that and adds safety checks for dosage, interactions, and allergies.

CPOE has reduced some medication errors and introduced new ones. Similar drug names can cause incorrect menu selections. Copy-and-paste can carry forward outdated information. Documentation time also remains a source of physician frustration. IT professionals must monitor for unintended effects and design interfaces that support quality care.

### Telemedicine Ethics

**Telemedicine** delivers healthcare through telecommunications technology. Video consultations, remote monitoring, and digital health platforms expanded dramatically during the COVID-19 pandemic and now let patients in rural areas see distant specialists, reduce travel for elderly and disabled patients, and lower costs.

Telemedicine raises four ethical issues:

* **Access and equity.** It requires reliable internet, a camera-equipped device, and digital literacy. Older adults, low-income patients, and those in rural areas with limited broadband may be excluded from the highly technology built to reach them, the **digital divide** in healthcare.

* **Informed consent.** A physician cannot examine a patient through a video call, and some conditions require in-person evaluation. Consent must be specific to the remote format.

* **Privacy and security.** Sessions transmit sensitive health data over the internet. Inadequate encryption or a household where others can overhear compromises patient privacy. The pandemic-era HHS relaxation of HIPAA enforcement for FaceTime and Zoom increased access and increased risk.

* **Cross-state licensing.** Licenses are issued by individual states, so a physician licensed in Arizona generally cannot treat a patient in California without a California license. Telemedicine complicates this. Long-term solutions are still developing.


### Try It Yourself 6.2: Test Your First Judgment 🛠️

**Predict:** Imagine you are a patient living in a rural community 90 miles from the nearest specialist. Your doctor recommends a telemedicine consultation with a cardiologist. You have a slow internet connection and share your home with family members. What concerns would you have about this arrangement? How would you want the healthcare system to address them?

**Run:** Apply the main framework or choice test from Section 6.2. Identify the stakeholder whose interest carries the most weight.

**Explain:** In 1-2 sentences, state whether the structured test confirmed or changed your first judgment.

### Quick Check 6.3 ✅

1. Explain what alert fatigue is and why it represents both a safety problem and an ethical problem in EHR systems. *(Understand)*

2. A small-town physician relies heavily on a CDSS to make prescribing choices because the clinic cannot afford to hire additional specialists. Analyze the ethical risks and benefits of this level of reliance on a clinical choice support tool. *(Analyze)*

3. A 78-year-old patient with limited internet access is told that her follow-up appointment will be conducted via telemedicine. She has never used a video calling platform. Apply the concept of informed consent to evaluate this situation. What obligations does the healthcare provider have? *(Apply)*

---

## 6.4 AI in Healthcare: Promise, Risk, and Accountability

AI is entering healthcare rapidly. Systems analyze medical images, predict patient deterioration, recommend treatments, accelerate drug discovery, and identify patterns clinicians might miss. The sections that follow build on the Chapter 3 AI ethics principles, fairness, transparency, accountability, explainability, and human oversight.

### AI-Assisted Diagnostics

Diagnostic AI is among the most visible uses. Systems have detected certain cancers in medical images with accuracy matching or exceeding human radiologists, analyzed retinal scans for diabetic retinopathy, read pathology slides, and identified suspicious skin lesions. They train on labeled image datasets and return probability-based assessments such as "this mammogram has a 94% probability of malignant lesion in a specific quadrant." AI processes images faster than humans, does not tire, and serves as a second set of eyes. In communities with physician shortages, it could extend specialist reach.

But when AI is wrong, the patient bears it. A **false negative** can delay treatment. A **false positive** triggers unnecessary anxiety, testing, and procedures with their own risks.

### Algorithmic Bias in Healthcare AI

**Algorithmic bias** is the tendency of AI systems to perform differently for different populations based on the data they trained on, and it is one of the largest ethical challenges in healthcare AI.

Healthcare AI bias is not hypothetical. A 2019 study (Obermeyer et al.) found that a widely used U.S. hospital algorithm flagging patients for extra care used healthcare spending as a proxy for need. Because Black patients historically had lower spending than white patients with the same illness severity, the algorithm underestimated Black patients' needs. Correcting it would have more than doubled the number flagged.

Bias enters at three points:

* **Training data.** If the dataset underrepresents racial, ethnic, age, or gender groups, the system performs less accurately for them.
* **Feature selection.** Zip code can act as a proxy for race or socioeconomic status even when race is not explicitly included.
* **Outcome definitions.** How the algorithm defines "success" or "need" shapes recommendations, as the spending example shows.

Healthcare AI must be tested across diverse populations before deployment, monitored after, and corrected when bias is found. Chapter 3's fairness and accountability principles apply directly.

### Liability When AI Causes Patient Harm

Medical malpractice frameworks require showing the physician deviated from the standard of care and that the deviation caused harm. AI complicates this. An AI analyzes a chest X-ray and reports no abnormalities. The radiologist, trusting the AI, spends less time reviewing and agrees. Six months later, the patient is diagnosed with lung cancer visible on the original X-ray. Who is responsible?

* **The physician** remains responsible for the final clinical choice. AI is a tool. The physician has a duty of independent judgment.
* **The AI developer** shares responsibility if the system was marketed for a purpose it was not validated for, or if known limitations were not disclosed.
* **The healthcare group** is responsible for deployment choices, clinician training, and ongoing performance monitoring.

A deontological view holds the duty of care cannot be delegated to a machine. A utilitarian view asks whether AI-assisted reading, even with errors, produces better aggregate outcomes than human-only reading. Both point to **human oversight**: AI supports clinical choices. It does not replace the judgment behind them.

### Informed Consent for AI-Assisted Treatment

Should patients be told when AI is involved in their care? The question matters more as AI integrates into diagnostic and treatment workflows.

One side argues patients have a right to know. Informed consent is a cornerstone of medical ethics. If a patient consents to a radiologist reviewing a scan but an algorithm did the analysis, the consent may not cover what happened, and a deontological view treats nondisclosure as a violation of honesty.

The other side argues disclosing every tool is impractical and may cause unnecessary anxiety. Patients are not told which lab machine processed their blood work.  AI is just another tool.

No consensus yet. What is clear: **transparency** and **human oversight** point toward giving patients meaningful information about how care choices get made when AI plays a major role.

### Clinical AI, Privacy, and Change Control

The FDA maintains resources for [AI-enabled medical devices](https://www.fda.gov/medical-devices/software-medical-device-samd/artificial-intelligence-enabled-medical-devices). Device oversight must account for performance, later changes, and the evidence supporting a safe use. A model that changes after release raises a practical question: can clinicians tell what changed and whether the new version still fits their patients?

The EU AI Act places many medical-device AI systems in a high-risk category. The specific application date depends on the system and follows the [European Commission's current timeline](https://digital-strategy.ec.europa.eu/en/policies/regulatory-framework-ai).

Ambient AI scribes listen to clinical conversations and draft notes. They raise consent and PHI questions about recording, processing, storage, access, and deletion. [HHS telehealth guidance](https://www.hhs.gov/hipaa/for-professionals/special-topics/telehealth/index.html) offers a useful privacy and security baseline for remote communication tools.

When a clinical system produces a note, triage score, or diagnostic suggestion, ask whether a clinician can review the result, see its limits, correct an error, and explain its role to the patient.

### Green Computing and Healthcare AI

Training and running AI models takes enormous compute. Large language models and complex imaging algorithms consume energy and rely on hardware with environmental costs. As healthcare adopts more AI, the footprint is an ethical concern.

Per Chapter 3's green-computing principles, healthcare groups must weigh environmental impact alongside clinical benefit: efficient models, renewable-powered data centers, and avoiding AI when simpler tools work.


### Try It Yourself 6.3: Test Your First Judgment 🛠️

**Predict:** You learn that the AI system your hospital uses to prioritize patients in the emergency department was trained primarily on data from suburban hospitals. Your hospital serves a predominantly low-income, urban community with high rates of chronic disease. What concerns would you raise about this system, and who should you raise them with? Think about the AI ethics principles of fairness and accountability from Chapter 3.

**Run:** Apply the main framework or choice test from Section 6.3. Identify the stakeholder whose interest carries the most weight.

**Explain:** In 1-2 sentences, state whether the structured test confirmed or changed your first judgment.

### Try It Yourself 6.4: Test the Boundary 🛠️

**Predict:** Which option in this section creates the least ethical risk?

**Run:** Apply one ethical framework and one stakeholder test from Section 6.4.

**Explain:** Defend your result with one fact from the section.

### Quick Check 6.4 ✅

1. Explain how algorithmic bias can enter a healthcare AI system through training data. Give one specific example of how this might affect patient care. *(Understand)*

2. A hospital begins using an AI tool that reads mammograms and flags potential cancers for radiologist review. The vendor claims the system reduces missed cancers by 20%. Analyze the ethical responsibilities of three parties: the AI developer, the hospital administration, and the radiologist using the system. *(Analyze)*

3. A patient asks you, an IT administrator at a clinic, whether AI is involved in reading their lab results. The clinic's pathology department recently integrated an AI screening tool. Should the patient be told? Apply the ethical principle of transparency to support your answer. *(Apply)*

---

## 6.5 Summary and Retrieval 💡

### Key Concepts

* **HIPAA is the legal foundation for U.S. health data privacy.** The Privacy Rule governs PHI access. The Security Rule requires administrative, physical, and technical safeguards for ePHI. The Breach Notification Rule requires disclosure when PHI is compromised.

* **mHealth creates a gap between legal protection and ethical responsibility.** Consumer health apps and wearables often fall outside HIPAA. Meaningful patient consent is hard to achieve when data collection is continuous and downstream uses are opaque.

* **Clinical IT systems improve safety but introduce new risks.** EHRs raise interoperability and alert-fatigue issues. CDSS and CPOE reduce some errors and create others. IT professionals must design and maintain these systems with patient safety as the primary concern.

* **Telemedicine expands access but raises equity, consent, and privacy concerns.** The digital divide can exclude the patients who could benefit most. Consent must cover remote-format limitations. Cross-state licensing remains unresolved.

* **AI in healthcare requires careful ethical oversight.** Algorithmic bias causes disparate performance for underrepresented populations. Liability is shared among developers, groups, and clinicians. Informed consent, transparency, and human oversight are essential safeguards.

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
* BYOD
* Consumer health app

#### Section 6.3

* Electronic Health Record (EHR)
* Interoperability
* Alert fatigue
* Clinical Decision Support System (CDSS)
* Computerized Provider Order Entry (CPOE)
* Telemedicine
* Digital divide

#### Section 6.4

* AI-assisted diagnostics
* Algorithmic bias
* False negative
* False positive
* Automation complacency

### Retrieval Practice

Try to answer these from memory before looking back at the chapter.

1. Name the three categories of safeguards required by the HIPAA Security Rule and give one specific example of each.

2. Explain why a consumer fitness app might collect sensitive health data without being subject to HIPAA. What ethical problem does this gap create for users?

3. A hospital is considering deploying an AI system trained on data from a patient population that does not reflect its own community. Using the concepts from this chapter, describe two specific risks and two steps the hospital should take before deployment.

---

## 6.6 Skills Lab 6A: Ethical Analysis of a Healthcare AI Deployment

**Goal:** Evaluate a healthcare AI deployment and advise hospital leadership.

**Evidence packet:** `assets/code/chapter-06/healthcare-ai-case.md`, a fictional case and evidence packet created for this textbook.

**Estimated time:** 90-120 minutes

### Case: AI-Powered Sepsis Prediction at Valley Regional Medical Center

Valley Regional Medical Center (VRMC), a 350-bed community hospital serving a diverse urban population, is considering a contract with a fictional firm called MedPredict AI. MedPredict offers an AI-powered sepsis prediction system. It monitors vital signs, lab results, and EHR data to identify patients at risk of sepsis. Sepsis is a life-threatening response to infection.

MedPredict's system was developed using data from 12 academic medical centers across the eastern United States. In fictional trials at those institutions, the system identified sepsis six hours before traditional screening methods on average. It had 82% sensitivity and 95% specificity. The firm projects that early detection could reduce sepsis mortality at VRMC by up to 15%.

However, VRMC's medical staff has raised several concerns:

* **Population mismatch.** The 12 academic medical centers that provided training data serve a patient population that is predominantly white and privately insured. VRMC's patient population is 45% Hispanic, 20% Black, and 15% uninsured or on Medicaid. Several physicians worry that the system may perform differently for their patients.

* **Alert burden.** With a 95% specificity rate, the system will generate about 5 false alerts for every 100 patients screened. VRMC's nurses, who are already managing heavy patient loads, express concern about alert fatigue. They worry that frequent false alarms will lead staff to ignore real alerts.

* **Data integration.** MedPredict's system requires access to real-time EHR data, lab results, and vital signs. This means patient data will flow through MedPredict's cloud servers for processing. MedPredict is a HIPAA-compliant business associate, but some physicians are uncomfortable with the volume of patient data leaving the hospital's network.

* **Cost.** The three-year contract costs $1.8 million. VRMC's administration argues that if the system prevents even a fraction of the sepsis deaths that currently occur, the cost is justified. The chief financial officer notes that sepsis patients who survive often require extended ICU stays costing $50,000 or more per case.

* **Transparency.** MedPredict's algorithm is proprietary. The firm provides overall performance statistics but will not share the model's architecture, feature weights, or training methodology. An independent audit of the algorithm is not possible under the proposed contract terms.

### Part 1: Foundation (Aligns with MLO-6.1)

1. Identify all stakeholders in this case. For each stakeholder, describe their primary interest and what they stand to gain or lose from the deployment choice.

2. Identify which HIPAA provisions are relevant to MedPredict's system. Specifically address: Is MedPredict a covered entity or a business associate? What Security Rule safeguards should VRMC require in the contract? How does the data flow between VRMC and MedPredict's cloud servers affect ePHI protection?

3. Define three key ethical issues raised by this case. For each, identify the competing values or rights in tension.

### Part 2: Application (Aligns with MLO-6.1, MLO-6.2)

4. Apply the utilitarian framework to evaluate whether VRMC should deploy MedPredict's system. Identify the potential benefits and harms to each stakeholder group. What does a utilitarian analysis recommend?

5. Apply the deontological framework to evaluate the same choice. Focus specifically on: the duty of care to patients, the transparency concerns around a proprietary algorithm, and the consent implications of routing patient data through an external cloud server.

6. MedPredict's training data underrepresents the demographic groups that make up the majority of VRMC's patient population. Apply the concept of algorithmic bias to explain why this matters. What specific risks does this create, and how should VRMC address them before deploying the system?

### Part 3: Extension (Aligns with MLO-6.2, MLO-6.3)

7. Write a recommendation to VRMC's administration (200-300 words). Should they sign the contract as proposed, negotiate modifications, or decline? Support your recommendation by referencing at least two ethical frameworks and specific concerns from the case.

8. Propose three specific contract modifications that would address the ethical concerns you identified. For each modification, explain which ethical principle it protects and why it matters for patient care.

### Questions & Analysis 🤔

1. Which risk should hospital leaders address before deployment, and why?
2. How does your recommendation balance patient privacy with access to care?

### Rubric: Skills Lab 6A

This lab is graded with the standard
[Skills Lab Rubric](../skills-lab-rubric.md): four criteria at
4 points each, 16 points total. The criteria are Technical Accuracy
and Efficiency, Output Quality, Documentation Quality, and Analysis,
Interpretation, and Response to QUESTION(s).

### Submission Guidelines

* **Length:** 800-1,200 words total across all parts
* **Format:** Submit as a single document organized by part number. Use clear headings for each section.

---

## 6.7 Review Questions 🔄️

1. Explain the difference between the HIPAA Privacy Rule and Security Rule.
2. Apply the minimum necessary standard to an IT support incident.
3. Analyze how telemedicine can improve access while increasing privacy risk.
4. When may emergency access justify weaker privacy controls? Defend a limit using two stakeholder perspectives.

## Further Reading 📖

* [HHS Health Information Privacy](https://www.hhs.gov/hipaa/index.html) - HHS provides the official entry point for HIPAA rights, rules, and guidance.
* [HHS: HIPAA and Telehealth](https://www.hhs.gov/hipaa/for-professionals/special-topics/telehealth/index.html) - HHS explains current privacy and security duties for telehealth.
* [FDA Artificial Intelligence-Enabled Medical Devices](https://www.fda.gov/medical-devices/software-medical-device-samd/artificial-intelligence-enabled-medical-devices) - The FDA lists authorized AI-enabled devices and regulatory resources.
* [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework) - NIST provides tools for evaluating AI reliability, bias, transparency, and accountability.
## Looking Ahead ⏩

In Chapter 7, you turn from healthcare to software liability and secure coding. When software defects cause harm, who bears responsibility, the developer, the firm, or the user? You will examine product-liability frameworks for software, learn secure coding as an ethical obligation, and apply cost/benefit analysis to IT choices.
