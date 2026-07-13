# Chapter 9: Intellectual Property and Fair Use

In January 2023, three visual artists filed a class-action lawsuit against Stability AI, Midjourney, and DeviantArt. They claimed the firms trained image generators on copyrighted work without permission or compensation. The firms raised defenses that include fair use. The dispute shows why AI training requires both legal and ethical analysis. Courts must apply existing law to specific evidence, while creators and developers argue about consent, markets, and innovation.

This chapter examines the legal and ethical foundations of **intellectual property (IP)**, the body of law that protects creative and innovative works. You will learn the four main types of IP protection, how **fair use** works, and why open source licensing represents a different philosophy about ownership. You will also confront hard questions in current IT ethics: Is downloading a movie without paying the same as theft? Can a firm reverse-engineer a competitor's product legally? Who, if anyone, owns the output of an AI system?

Whether you work in software development, IT support, web design, or data analytics, you will encounter IP choices regularly. Understanding the rules, and knowing where they are genuinely unclear, will help you make informed choices in your career.

## Module Overview 🧭

* **Estimated time:** 4-5 hours (reading + practice + Skills Lab)
* **Prerequisites:** Chapters 1-8
* **Deliverables:** Try It Yourself activities, Quick Checks, Skills Lab 9A

## Learning Objectives 🎯

By the end of this chapter, you will be able to:

* **MLO-9.1 (Apply):** Apply the principles of copyright, patent, trademark, and trade secret law to classify industry-relevant IP scenarios
* **MLO-9.2 (Analyze):** Analyze how fair use doctrine applies to digital content, open source licensing, and competitive intelligence practices
* **MLO-9.3 (Evaluate):** Evaluate the ethical and legal arguments surrounding AI-generated works and the use of copyrighted training data

### This chapter aligns with the following Course Learning Outcomes

* **CLO XI.** Interpret intellectual property, copyright laws, and fair use doctrine.

---

## 9.1 The Four Types of Intellectual Property

Intellectual property law grants creators and inventors certain exclusive rights over their work. Unlike physical property, IP protects intangible things: ideas expressed in a particular form, inventions, brand identities, and confidential business information. There are four main types of IP protection, each designed for a different kind of work. Understanding the differences matters because using the wrong framework, or ignoring these protections entirely, can have serious legal and ethical effects.

### Copyright

**Copyright** protects original works of authorship that are fixed in a tangible form. This includes books, music, software code, photographs, videos, website content, and architectural designs. Copyright protection is automatic: the moment you write a poem, take a photograph, or commit code to a repository, you own the copyright. You do not need to register it, though registration provides additional legal benefits if you ever need to enforce your rights in court.

Copyright gives the owner several exclusive rights: to reproduce the work, distribute copies, create derivative works, and publicly display or perform it. For works created by people, protection lasts the author's lifetime plus 70 years. For **works for hire**, such as software written by a worker as part of the job, the employer owns the copyright. Protection lasts 95 years from publication or 120 years from creation, whichever is shorter.

One point matters for IT professionals: **copyright protects an idea's expression, not the idea itself.** You can write your own sorting algorithm, but you cannot copy someone else's implementation. Two people can independently write programs that do the same thing, and both programs are separately copyrightable. The protection covers the specific expression in code.

### Patents

A **patent** gives an inventor the exclusive right to make, use, and sell an invention for a limited time, typically 20 years from the filing date. Unlike copyright, patents require a formal application process through the United States Patent and Trademark Office (USPTO) or equivalent agencies in other countries. The invention must be novel, non-obvious, and useful.

In IT, patents cover hardware inventions, manufacturing processes, and sometimes software-related innovations. **Software patents** have been controversial for decades. Critics argue that many software patents are too broad or too obvious, and that they stifle innovation instead of encourage it. A single smartphone may involve thousands of patents held by dozens of firms, and patent disputes in the tech industry have produced massive lawsuits and complex licensing agreements that can take years to resolve.

### Trademarks

A **trademark** protects words, phrases, symbols, logos, or designs that identify the source of goods or services. The Apple logo, the Nike swoosh, and the phrase "Just Do It" are all trademarks. Trademarks prevent consumer confusion by ensuring that when you see a particular brand name or logo, you know who made the product.

Trademark protection can last indefinitely, as long as the mark is actively used in commerce and the owner takes steps to defend it. For IT professionals, trademarks matter in web development, app design, domain name registration, and anywhere brand identity intersects with technology.

### Trade Secrets

A **trade secret** is confidential business information that provides a competitive advantage. The classic example is the Coca-Cola formula, but in IT, trade secrets more commonly include proprietary algorithms, customer databases, pricing strategies, and internal business processes. Unlike patents, trade secrets have no expiration date and require no registration. The catch is that the owner must take reasonable steps to keep the information secret. If a trade secret is publicly disclosed, whether through a leak, reverse engineering, or carelessness, the protection is lost.

The **Defend Trade Secrets Act (DTSA)** of 2016 created a federal cause of action for trade secret theft. For IT workers, this is especially relevant: the code you write, the systems you build, and the data you access at work may all be classified as trade secrets by your employer.


### Try It Yourself 9.1: Test Your First Judgment 🛠️

**Predict:** You create a mobile app on your own time using your own equipment. Your employer claims it belongs to them because it is related to the firm's business. What type of IP protection is most relevant here, and who do you think should own the app? What facts would you need to know to decide?

**Run:** Apply the main framework or choice test from Section 9.1. Identify the stakeholder whose interest carries the most weight.

**Explain:** In 1-2 sentences, state whether the structured test confirmed or changed your first judgment.

### Quick Check 9.1 ✅

1. What is the key difference between copyright and patent protection? Give an example of something protected by each. *(Understand)*
2. A software firm keeps its recommendation algorithm confidential and requires all staff to sign nondisclosure agreements. What type of IP protection applies, and what could cause the firm to lose that protection? *(Apply)*
3. Explain why copyright protects the expression of an idea but not the idea itself. Why does this distinction matter for software developers? *(Analyze)*

---

## 9.2 Fair Use, Open Source, and Digital Licensing

Understanding IP types is only half the picture. Equally important is knowing when and how others can legally use protected works. This section covers three frameworks that define the boundaries of legitimate use: fair use doctrine, open source licensing, and the broader ethics of digital content sharing.

### Fair Use Doctrine

**Fair use** is a legal doctrine built into U.S. copyright law (Section 107 of the Copyright Act) that allows limited use of copyrighted material without permission. Fair use exists because rigid copyright enforcement could stifle criticism, education, commentary, and creativity. A book reviewer needs to quote passages. A teacher needs to share excerpts with students. A comedian needs to parody a popular song. Fair use makes these activities possible.

Courts evaluate fair use claims using four factors:

1. **The purpose and character of the use.** Is the use commercial or nonprofit/educational? Is it "transformative," meaning it adds new meaning, expression, or purpose to the original? Transformative uses are more likely to qualify as fair use.
2. **The nature of the copyrighted work.** Using factual works (like news articles) is more likely to be considered fair use than using highly creative works (like novels or music).
3. **The amount used.** Using a small portion of a work is more defensible than using the entire thing. However, even a small amount can fail the fair use test if it represents the "heart" of the original work.
4. **The effect on the market.** Does the use substitute for the original, potentially reducing sales or licensing revenue? If so, it is less likely to qualify as fair use.

No single factor is decisive. Courts weigh all four together, which makes fair use inherently unpredictable, and that ambiguity is one of the biggest challenges for IT professionals and content creators who want to stay within the law.

### Fair Use in Digital Contexts

Digital technology has made copying trivially easy and distribution instantaneous, which puts enormous pressure on fair use boundaries. Consider a few common cases:

* **Search engines** display thumbnail images and text snippets from websites. Courts have generally ruled this is fair use because it is transformative (helping users find information) and does not replace the original content.
* **Memes** often incorporate copyrighted images with new captions or contexts. Most memes probably qualify as fair use due to their transformative nature, though this has not been definitively tested in court.
* **Educational use** is often assumed to be automatically fair use, but that is a misconception. Photocopying an entire textbook chapter for a class, or uploading a full copyrighted article to a course website, may exceed fair use limits even in educational settings.

### Case Study 9.1 - The Google Books Scanning Project 📋

**The Situation:** Beginning in 2004, Google partnered with major research libraries to scan millions of books and make them searchable through Google Books. Users could search the full text of books and view short snippet results showing a few sentences around their search terms. For books still under copyright, Google displayed only these limited snippets, not the full text. Google did not obtain permission from the authors or publishers before scanning their works.

The Authors Guild filed a lawsuit in 2005 and argued that Google's mass scanning infringed copyright. The case moved through courts for more than a decade. Google argued that its searchable index was transformative. It helped readers find books and gave visually impaired users new access through text-to-speech tools. The Authors Guild countered that Google profited from unauthorized copies and could reduce incentives for authors.

In 2015, the Second Circuit Court of Appeals ruled in Google's favor, finding that the project qualified as fair use. The court emphasized the transformative purpose of the search function, the limited amount of text displayed to users, and evidence that the project increased book sales instead of undermining them. The Supreme Court declined to hear the case, leaving the ruling in place.

**Stakeholders:**

* **Google** gained a massive searchable database and increased traffic to its platform, reinforcing its position as the world's information gateway
* **Authors and publishers** lost control over how their copyrighted works were used and received no direct compensation from the scanning
* **Researchers and the public** gained the ability to search millions of books instantly, a capability that previously did not exist
* **Libraries** preserved fragile collections digitally and expanded access to rare works
* **Visually impaired readers** gained access to books through text-to-speech features enabled by the digital scans

**Questions to Consider:**

1. The court found Google's use "transformative" because it created a new functionality (search) instead of substituting for the original books. Do you agree with this reasoning? Where would you draw the line between a transformative use and simple copying?
2. Consider this case from the perspective of a midlist author who earns modest royalties. Does the fact that the project may increase overall book sales adequately address the ethical concern of using their work without permission?
3. How might this ruling affect future cases involving large-scale data collection, such as the AI training data disputes described later in this chapter?

### Open Source Licensing

Not everyone believes in restricting access to creative works. The **open source** movement represents a fundamentally different philosophy: that software (and increasingly other creative works) should be freely available for anyone to use, modify, and distribute. Open source is not the absence of licensing. It is a specific set of licensing models that define how freely shared works can be used.

The most common open source licenses fall into two categories:

* **Permissive licenses** (such as the MIT License and Apache License) allow nearly unrestricted use, such as incorporating open source code into commercial products. The main requirement is attribution: you must credit the original creators.
* **Copyleft licenses** (such as the GNU General Public License, or GPL) require that any derivative work be released under the same license. This means that if you use GPL-licensed code in your software, your software must also be open source. This "viral" quality is intentional: it ensures that improvements to the codebase remain freely available.

Open source software can accelerate innovation and reduce barriers for new developers. Public source code also supports transparency because anyone can audit it for security flaws.

However, open source raises its own ethical questions. Firms sometimes build profitable products on top of free open source code without contributing back to the community. Volunteer open source developers often burn out maintaining critical infrastructure that millions depend on. The **Creative Commons (CC)** licensing system extends similar principles to non-software works like textbooks (such as this one), photographs, and music.


### Try It Yourself 9.2: Test Your First Judgment 🛠️

**Predict:** Many of the tools you use every day, from web browsers to operating systems to programming languages, are built on open source code. Should firms that profit from open source software be ethically obligated to contribute back to the projects they depend on? Why or why not?

**Run:** Apply the main framework or choice test from Section 9.2. Identify the stakeholder whose interest carries the most weight.

**Explain:** In 1-2 sentences, state whether the structured test confirmed or changed your first judgment.

### Quick Check 9.2 ✅

1. List the four factors courts use to evaluate a fair use claim. Which factor do you think is most important in digital contexts, and why? *(Understand)*
2. A student uploads a full copyrighted documentary to a class discussion board so classmates can watch it for an assignment. Analyze whether this qualifies as fair use by applying the four-factor test. *(Analyze)*
3. What is the key difference between a permissive open source license (like MIT) and a copyleft license (like GPL)? Why does this distinction matter for a firm building commercial software? *(Apply)*

---

## 9.3 Plagiarism, Piracy, and Competitive Intelligence

IP law sets legal boundaries, but many IT choices fall in gray areas. The law may be unclear, vary by location, or lag behind current practice. This section examines plagiarism, digital piracy, reverse engineering, and competitive intelligence.

### Plagiarism in IT Contexts

**Plagiarism** is presenting someone else's work, ideas, or expressions as your own without proper attribution. In academic settings, plagiarism is a serious integrity violation. In professional IT settings, it takes different forms: copying code from Stack Overflow without attribution, reusing a colleague's design in a portfolio, or submitting vendor documentation as your own analysis.

Plagiarism and copyright infringement overlap but are not identical. You can plagiarize an uncopyrighted idea by presenting it without credit. You can also infringe copyright while naming the creator if you lack the right to copy or distribute the work. Plagiarism is dishonest because it misrepresents the source and weakens trust.

For IT professionals, code plagiarism raises particular concerns. Open source code is meant to be reused, but even open source licenses typically require attribution. Copying proprietary code from a previous employer into a new project can violate trade secret protections and employment agreements. Knowing what you can reuse and how to credit it is a practical skill every IT worker needs.

### Digital Piracy

**Digital piracy** refers to the unauthorized copying, distribution, or use of copyrighted digital content, such as software, music, movies, games, and e-books. The scale of digital piracy is enormous. Industry groups estimate billions of dollars in annual losses, though the specific figures are debated because not every pirated copy represents a lost sale.

The ethical arguments around piracy are complex. Opponents argue that creators deserve payment and that piracy weakens incentives to create. Others note that copying a digital file does not remove the owner's original. They also question whether every unauthorized copy represents a lost sale. Restrictive prices and regional limits may further shape consumer choices.

The **Digital Millennium Copyright Act (DMCA)** of 1998 is the primary U.S. law addressing digital piracy. It criminalizes the circumvention of **digital rights management (DRM)** technologies and provides a "notice and takedown" process for copyright holders to request removal of infringing content. Critics argue the DMCA is overly broad, chilling legitimate uses like security research and archival preservation.

### Reverse Engineering and Competitive Intelligence

**Reverse engineering** is the process of analyzing a product to understand how it works, often to build a competing product or ensure compatibility. In IT, this might mean decompiling software, analyzing network protocols, or studying how a competitor's system handles data.

The legal status of reverse engineering depends heavily on context. U.S. courts have generally allowed it for achieving interoperability or conducting security research. However, the DMCA's anti-circumvention provisions create complications: if reverse engineering requires bypassing DRM or other technical protections, it may violate the law even if the underlying purpose is legitimate.

**Competitive intelligence** is the practice of gathering information about competitors to inform business strategy. Most of it is perfectly legal: reading public filings, attending trade shows, analyzing publicly available products, and monitoring news coverage. The line gets crossed when firms use deceptive practices to obtain information, recruit staff primarily to extract trade secrets, or access proprietary systems without authorization.

### Trademark Infringement and Cybersquatting

While copyright and patent disputes get more attention, trademark violations are common online. **Trademark infringement** occurs when someone uses a confusingly similar mark that may mislead consumers. Examples include domain names, app names, or website designs that imitate established brands.

**Cybersquatting** is the practice of registering domain names that incorporate well-known trademarks with the intent to profit from them, typically by selling the domain back to the trademark holder at an inflated price. The **Anticybersquatting Consumer Protection Act (ACPA)** of 1999 and the **Uniform Domain-Name Dispute-Resolution Policy (UDRP)** administered by ICANN provide legal remedies for affected trademark holders.


### Try It Yourself 9.3: Test Your First Judgment 🛠️

**Predict:** A friend tells you they pirate all their software because they cannot afford to buy it. They argue that they are not hurting anyone since they would never have paid for it anyway. How would you respond? Does it matter whether the software is made by a large corporation or an independent developer?

**Run:** Apply the main framework or choice test from Section 9.3. Identify the stakeholder whose interest carries the most weight.

**Explain:** In 1-2 sentences, state whether the structured test confirmed or changed your first judgment.

### Quick Check 9.3 ✅

1. Explain the difference between plagiarism and copyright infringement. Can you commit one without the other? Give an example of each. *(Understand)*
2. A startup reverse-engineers a competitor's file format so that its own product can import the competitor's files. Analyze whether this practice is ethical by considering the interests of all stakeholders involved. *(Analyze)*
3. Apply the ethical frameworks from Chapter 1 (utilitarianism and deontology) to the debate over digital piracy. What does each framework say about the ethics of downloading copyrighted content without paying? *(Apply)*

---

## 9.4 AI and Intellectual Property: Uncharted Territory

The rise of generative AI has created some of the most challenging IP questions the legal system has ever faced. When an AI system produces a painting, writes a poem, or generates code, who owns the result? When AI firms train their models on billions of copyrighted works scraped from the internet, did they infringe copyright or engage in fair use? These questions are being fought in courtrooms right now, and the answers will shape the future of creative work, software development, and the technology industry.

### Who Owns AI-Generated Works?

Under current U.S. copyright law, only works created by human beings can be copyrighted. The U.S. Copyright Office has consistently held that the human mind's connection to creative expression is a fundamental requirement. In 2023, the Copyright Office issued guidance clarifying that purely AI-generated content cannot be registered. If you type a prompt into an image generator and it produces a picture, you do not own the copyright because you did not create the expressive elements yourself.

However, the situation becomes more complex when humans and AI collaborate. If a human author makes substantial creative choices, such as selecting, arranging, and editing AI-generated elements into a larger work, those human-authored elements may be copyrightable. The Copyright Office has handled these cases individually, and the boundary between "human-authored with AI assistance" and "AI-generated" is not yet clearly defined.

This creates practical problems for IT professionals and businesses. If AI-generated code cannot be copyrighted, can competitors freely copy it? If a marketing team uses AI to produce advertising images, does the firm have any IP protection for those images? These uncertainties are already affecting business choices.

### AI Training Data and Copyright

The other side of the AI-IP debate concerns the data used to train AI systems. Large language models and image generators are trained on enormous datasets that typically include copyrighted material: books, articles, photographs, artwork, and source code scraped from the internet. AI firms argue this training process is fair use because models learn patterns instead of storing or reproducing specific works. Critics argue that training on copyrighted material without permission is infringement, regardless of how the data is processed internally.

Several major lawsuits are testing these arguments. The *New York Times v. Microsoft and OpenAI* case, filed in late 2023, alleges that ChatGPT can reproduce substantial portions of Times articles verbatim. Other cases brought by authors, visual artists, and music publishers raise similar claims against various AI firms, and Getty Images sued Stability AI for training on millions of its copyrighted photographs.

The outcome of these cases will have enormous effects. If courts rule that training on copyrighted data is not fair use, AI firms may need to license training data, fundamentally changing the economics of AI development. If courts rule that training is fair use, creators may lose meaningful control over how their works are used.

### The Global Dimension

Different countries are taking different approaches. The European Union's AI Act includes provisions about transparency in training data, requiring firms to disclose what copyrighted material was used. Japan has taken a more permissive stance, generally allowing AI training on copyrighted works for the purpose of information analysis. These differences create challenges for global technology firms that must comply with varying legal frameworks across jurisdictions.

As you learned in Chapter 8, different regulatory philosophies reflect different ethical values. The EU's precautionary approach prioritizes creator rights and transparency. Japan's permissive approach prioritizes innovation and competitiveness. The United States is relying on a case-by-case judicial approach, letting courts decide instead of enacting comprehensive legislation. Each reflects a different assumption about how to balance innovation against the rights of existing creators.

### Current U.S. Copyright Office Guidance on AI

The [U.S. Copyright Office AI initiative](https://www.copyright.gov/ai/) separates three questions. Part 1 of its report addresses digital replicas. Part 2 addresses whether AI-assisted outputs contain enough human authorship for copyright protection. Part 3 examines the use of copyrighted works in generative AI training.

The Office states that prompts alone do not make a person the author of every expressive element in an output. Human-created selection, arrangement, or modification may receive protection when it meets normal copyright standards. Training disputes still require fact-specific legal analysis, such as the fair use factors and the evidence in a case.

When you use AI-generated material, record what the tool produced and what a person selected, changed, arranged, or wrote. Check for recognizable third-party material and confirm license duties. Do not promise a client exclusive ownership until the authorship and source questions have been reviewed.

### Try It Yourself 9.4: Test the Boundary 🛠️

**Predict:** Which option in this section creates the least ethical risk?

**Run:** Apply one ethical framework and one stakeholder test from Section 9.4.

**Explain:** Defend your result with one fact from the section.

### Quick Check 9.4 ✅

1. Under current U.S. law, can a work generated entirely by AI receive copyright protection? Explain the reasoning behind this position. *(Understand)*
2. Compare the arguments made by AI firms (that training on copyrighted data is fair use) with the arguments made by copyright holders (that training without permission is infringement). Which of the four fair use factors supports each side? *(Analyze)*
3. A software developer uses an AI coding assistant to generate a function, then significantly modifies and integrates it into a larger program. Evaluate whether the developer should be able to claim copyright on the final product. What factors would you consider? *(Evaluate)*

---

## 9.5 Summary and Retrieval 💡

### Key Concepts

* **Intellectual property law protects intangible creative and innovative works** through four mechanisms: copyright (original expression), patents (inventions), trademarks (brand identity), and trade secrets (confidential business information). Each type covers different kinds of work and has different requirements and durations.

* **Fair use allows limited use of copyrighted material without permission**, but its boundaries are unpredictable. Courts weigh four factors: purpose and character of use, nature of the copyrighted work, amount used, and effect on the market. Digital technology has intensified these debates because copying and distribution have become effortless.

* **Open source licensing represents an alternative to traditional IP restrictions**, with permissive licenses (like MIT) allowing broad reuse and copyleft licenses (like GPL) requiring that derivative works remain open source. The open source philosophy prioritizes collaborative innovation and transparency.

* **Digital piracy, reverse engineering, and competitive intelligence** occupy gray areas where legal rules, ethical principles, and practical considerations do not always align. Knowing where the lines fall, and where they remain genuinely uncertain, is essential for IT professionals.

* **AI has disrupted traditional IP frameworks.** Under current U.S. law, purely AI-generated works cannot be copyrighted. The legality of training AI models on copyrighted data is being tested in multiple high-profile lawsuits, and countries are adopting widely different approaches.

### Key Terms

#### Section 9.1

* Intellectual property (IP)
* Copyright
* Work for hire
* Patent
* Software patent
* Trademark
* Trade secret
* Defend Trade Secrets Act (DTSA)

#### Section 9.2

* Fair use
* Open source
* Permissive license
* Copyleft license
* Creative Commons (CC)

#### Section 9.3

* Plagiarism
* Digital piracy
* Digital Millennium Copyright Act (DMCA)
* Digital rights management (DRM)
* Reverse engineering
* Competitive intelligence
* Cybersquatting
* Anticybersquatting Consumer Protection Act (ACPA)
* Uniform Domain-Name Dispute-Resolution Policy (UDRP)

#### Section 9.4

* AI-generated works
* Training data

### Retrieval Practice

Try to answer these from memory before looking back at the chapter.

1. Name the four types of intellectual property and state what each one protects. Which type requires a formal application, and which is automatic?
2. What are the four factors courts consider when evaluating a fair use claim? Give a brief example of how one factor might weigh in favor of fair use and how the same factor might weigh against it.
3. Explain the current legal status of AI-generated works under U.S. copyright law. Why does this matter for businesses using AI tools to create content?

---

## 9.6 Skills Lab 9A: Intellectual Property Analysis

**Goal:** Classify intellectual property issues and recommend a fair platform policy.

**Evidence packet:** `assets/code/chapter-09/intellectual-property-case.md`, a fictional case and evidence packet created for this textbook.

**Estimated time:** 90-120 minutes

### Case: TechCanvas and the AI Art Platform

TechCanvas is a mid-sized software firm that has launched an AI-powered design platform called ArtForge. The platform allows users to type text prompts and receive AI-generated images, logos, and design layouts. ArtForge has become popular with small businesses, freelance designers, and marketing teams who use it to quickly produce visual content.

Several issues have emerged since ArtForge's launch. First, a fictional independent investigation found that TechCanvas trained ArtForge on 400 million images scraped from the internet. The dataset included copyrighted photographs, illustrations, and stock images. TechCanvas did not seek permission or pay the creators. The firm argues that using public images for AI training is transformative fair use.

Second, a freelance graphic designer named Maria Delgado discovered that when she types her own name as part of a prompt, ArtForge generates images that closely resemble her distinctive illustration style. Maria has built her career and reputation on that style over fifteen years. She argues that ArtForge is effectively allowing anyone to produce knockoffs of her work. TechCanvas responds that artistic styles are not copyrightable and that ArtForge is simply a tool that learned general visual patterns.

Third, several small businesses that created logos and marketing materials using ArtForge are now discovering that they may not have clear copyright protection over the AI-generated designs. A competitor copied one firm's ArtForge-generated logo almost exactly, and the firm found it had limited legal recourse because the logo was generated by AI instead of created by a human designer.

### Part 1: Foundation (Aligns with MLO-9.1)

1. Identify each type of intellectual property relevant to this case (copyright, patent, trademark, trade secret). For each type, explain specifically how it applies to the situation described.
2. List all the stakeholders in this case. For each stakeholder, describe what they stand to gain or lose and which IP protections are most relevant to their interests.
3. The freelance designer Maria argues her illustration style is being copied. Under current IP law, is an artistic "style" protectable? Explain which type of IP protection (if any) might apply and why styles are treated differently from specific works.

### Part 2: Application (Aligns with MLO-9.1, MLO-9.2)

4. Apply the four-factor fair use test to TechCanvas's choice to train ArtForge on 400 million scraped images. Analyze each factor separately and then state your overall conclusion about whether the training qualifies as fair use.
5. The small businesses that used ArtForge to create logos are discovering they lack copyright protection. Analyze the ethical responsibilities TechCanvas has to its users. Should the firm have disclosed the IP limitations of AI-generated content before users relied on it for business purposes?
6. Compare this case to the Google Books case discussed earlier in this chapter. What similarities and differences do you see? Does the Google Books ruling support or undermine TechCanvas's fair use argument?

### Part 3: Extension (Aligns with MLO-9.2, MLO-9.3)

7. Evaluate the competing interests in this case and propose a policy framework that balances the rights of original creators, AI firms, and end users of AI-generated content. Your proposal should address training data, generated output, and disclosure requirements.
8. Consider this case from an international perspective. If TechCanvas operates globally, how might the different approaches taken by the U.S., the EU, and Japan (as discussed in Section 9.4) affect the firm's obligations? Evaluate whether a single global standard for AI and IP is desirable or whether regional differences serve an important purpose.

### Questions & Analysis 🤔

1. Which fair use factor carries the most weight in your recommendation?
2. How would your policy affect an individual creator differently from a large publisher?

### Rubric: Skills Lab 9A

This lab is graded with the standard
[Skills Lab Rubric](../skills-lab-rubric.md): four criteria at
4 points each, 16 points total. The criteria are Technical Accuracy
and Efficiency, Output Quality, Documentation Quality, and Analysis,
Interpretation, and Response to QUESTION(s).

### Submission Guidelines

* **Length:** 800-1,200 words total across all parts
* **Format:** Submit as a single document organized by part number. Use clear headings for each section.

---

## 9.7 Review Questions 🔄️

1. Distinguish copyright, patent, trademark, and trade secret protection.
2. Apply the four fair use factors to a digital remix.
3. Analyze how open source duties differ from public-domain use.
4. Should commercial AI developers license copyrighted training material? Defend your answer and address the strongest counterargument.

## Further Reading 📖

* [U.S. Copyright Office: Copyright and Artificial Intelligence](https://www.copyright.gov/ai/) - The Office publishes its reports on digital replicas, AI outputs, and training.
* [U.S. Copyright Office Fair Use Index](https://www.copyright.gov/fair-use/) - The index explains the four factors and summarizes federal choices.
* [USPTO Intellectual Property Basics](https://www.uspto.gov/learning-and-resources/inventors-and-entrepreneurs/ip-basic-toolkits) - The USPTO introduces patents, trademarks, copyright, and trade secrets.
* [Open Source Initiative Licenses](https://opensource.org/licenses) - OSI lists approved open source licenses and review standards.
## Looking Ahead ⏩

In Chapter 10, you will shift from questions of ownership to questions of expression. Who gets to say what online, and what happens when speech causes harm? Chapter 10 examines the boundaries of the First Amendment in digital spaces, the classification of hate speech and defamation, the ethics of internet anonymity, and the growing tension between worker monitoring and workplace privacy. You will also explore how AI-generated deepfakes and automated content moderation systems are complicating these debates in ways the law was never designed to handle.
