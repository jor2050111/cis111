# CIS111 Textbook: Session Handoff

**Last updated:** 2026-07-12

**Repository:** [GitHub repository](https://github.com/jor2050111/cis111)

**Live site:** [CIS111 textbook](https://jor2050111.github.io/cis111/)

**Task list:** `CLAUDE_CODE_TASK_LIST_ID=cis111`, pinned in
`.claude/settings.json`

## Current Status

The new CIS111 textbook repository is scaffolded and contains a complete
12-chapter legacy conversion. The book is schedule-neutral. It does not
assign chapters to weeks, terms, exams, or due dates. An instructor can
later map the same chapters into a 9-, 12-, 14-, or 16-week course.

The imported content has received a first standards pass, but it is not
yet the final publication edition. Chapters 1-11 have completed their
full plain-language and instructional reviews. Chapter 12 remains.

## What Was Built

* Configured the Zensical site for CIS111: Ethics in Information
  Technology.
* Created the four-Part navigation for all 12 chapters.
* Added the official district competencies, elevated CLOs, CLO mapping,
  and district course outline in `docs/CIS111_CLOs.md`.
* Created the schedule-neutral Part plan in `docs/part-structure.md`.
* Added the student home page, course tools, full CLO list, and four-Part
  book map.
* Converted all 12 legacy modules into numbered textbook chapters.
* Added three MLOs and a verbatim CLO alignment block to each chapter.
* Added four Predict-Run-Explain activities and four Quick Checks to each
  chapter.
* Added one three-Part Skills Lab, two Questions & Analysis prompts, and
  four review questions to each chapter.
* Added 12 fictional evidence packets under `assets/code/chapter-NN/`.
* Built `build/cis111-evidence-pack.zip` and verified the archive.
* Created a 218-entry glossary. Every chapter Key Terms entry resolves to
  one glossary definition.
* Replaced old or weak source links with current primary sources from
  NIST, HHS, CISA, the FTC, the European Commission, the US Copyright
  Office, and professional bodies.
* Updated AI Act, NIST incident response, copyright, privacy, healthcare,
  and secure software claims that had changed since the legacy draft.

## Verified Gates

* All uppercase template tokens are replaced.
* All 12 chapter pages appear in the built site and navigation.
* `zensical build --clean` reports no issues.
* Every chapter has zero prose sentences at or above 35 words.
* Student-facing Markdown has zero em dashes, prose semicolons, and banned
  wording.
* Every chapter has exactly one Skills Lab goal and one evidence packet.
* Every chapter has exactly two Questions & Analysis prompts and four
  review questions.
* All chapter Key Terms entries resolve to the glossary.
* All evidence packet paths exist.
* Chapter 1 measures Flesch 60.4 with a grade estimate of 7.8.
* Chapter 1 reports zero Markdown lint errors and zero sentence-length
  flags.
* Chapter 2 measures Flesch 60.1 with a grade estimate of 7.8.
* Chapter 2 reports zero Markdown lint errors and zero sentence-length
  flags.
* Chapter 3 measures Flesch 60.1 with a grade estimate of 7.7.
* Chapter 3 reports zero Markdown lint errors and zero sentence-length
  flags.
* Chapter 3 covers the five AI ethics principles, public governance
  approaches from eight major AI labs, the EU AI Act, NIST AI RMF,
  OECD AI Principles, and IEEE Ethically Aligned Design.
* Chapter 3 source claims were checked against current primary sources
  on 2026-07-12. Its source links were also tested.
* Chapter 4 measures Flesch 66.5 with a grade estimate of 6.9.
* Chapter 4 reports zero Markdown lint errors and zero sentence-length
  flags.
* Chapter 4 includes current FTC guidance on COPPA, paid posts, the
  impersonation rule, and the Take It Down Act. It also uses current
  DSA, EEOC, DOJ, HHS, HUD, and legal scholarship sources.
* Chapter 4 source claims were checked on 2026-07-12. Its source links
  were also tested.
* Chapter 5 measures Flesch 63.2 with a grade estimate of 7.4.
* Chapter 5 reports zero Markdown lint errors and zero sentence-length
  flags.
* Chapter 5 distinguishes ethical justification from legal protection,
  applies fiduciary-style data duties, and gives safe evidence-handling
  guidance without presenting legal advice.
* Chapter 5 legal claims were checked against current primary sources
  from OSHA, the SEC, the Supreme Court, DOJ, the NLRB, the EEOC, and
  the European Commission on 2026-07-12. Its source links were also
  tested. The ACM and SEC pages reject command-line checks, so their
  content was confirmed through indexed or browser-rendered copies.
* Chapter 6 measures Flesch 60.4 with a grade estimate of 7.8.
* Chapter 6 reports zero Markdown lint errors and zero sentence-length
  flags.
* Chapter 6 separates HIPAA scope from FDA and FTC scope. It adds a
  mobile data map, a clinical safety loop, an AI release gate, and a
  contract-focused MedPredict Skills Lab.
* Chapter 6 health data, telehealth, and AI claims were checked against
  current primary sources from HHS, the FTC, ONC, FDA, and the original
  healthcare-bias study on 2026-07-12. Its source links were also
  tested. Several government pages reject command-line checks, so their
  content was confirmed through browser-rendered copies.
* Chapter 7 measures Flesch 65.6 with a grade estimate of 7.2.
* Chapter 7 reports zero Markdown lint errors and zero sentence-length
  flags.
* Chapter 7 separates ethical responsibility from legal liability. It
  adds a six-line claim map, the four NIST SSDF areas, secure-by-design
  duties, release gates, current OWASP 2025 risks, and safety stop rules.
* Chapter 7 legal and security claims were checked against current
  primary sources from Arizona, the EU, NIST, CISA, OWASP, the FTC,
  Microsoft, and ACM on 2026-07-12. Its source links were also tested.
  The ACM and FTC pages reject command-line checks, so their content was
  confirmed through browser-rendered copies.
* Chapter 8 measures Flesch 61.2 with a grade estimate of 7.6.
* Chapter 8 reports zero Markdown lint errors and zero sentence-length
  flags.
* Chapter 8 adds a six-question regulation scope map, audit and sanction
  tests, a fair-work transition test, and a rule-and-control record for
  AI systems.
* Chapter 8 privacy, labor, and AI claims were checked against current
  primary sources from the EU, California, the FTC, DOL, the EEOC, and
  NIST on 2026-07-12. Its source links were also tested. The ACM and FTC
  pages reject command-line checks, so their content was confirmed
  through browser-rendered copies.
* Chapter 9 measures Flesch 61.5 with a grade estimate of 7.8.
* Chapter 9 reports zero Markdown lint errors and zero sentence-length
  flags.
* Chapter 9 adds a six-line IP card, a four-factor fair use sheet, a
  license and source log, a reverse-engineering source test, and separate
  records for human work and AI training.
* Chapter 9 copyright, patent, trademark, trade-secret, licensing, and AI
  claims were checked against current primary sources from the USPTO,
  the U.S. Copyright Office, and the Open Source Initiative on
  2026-07-12. All nine source links returned successful responses.
* Chapter 10 measures Flesch 64.8 with a grade estimate of 7.1.
* Chapter 10 reports zero Markdown lint errors and zero sentence-length
  flags.
* Chapter 10 adds a six-line speech map, an eight-line defamation record,
  a five-step content review, an eight-part monitoring need test, and a
  worker-monitoring release gate.
* Chapter 10 speech, defamation, Section 230, deepfake, worker-rights,
  interception, and AI monitoring claims were checked against current
  primary sources from Congress, the House, the NLRB, DOL, the FTC, and
  the EU on 2026-07-12. All ten links were tested. Five government pages
  reject command-line checks, so their content was confirmed through
  browser-rendered or indexed copies.
* Chapter 11 measures Flesch 60.7 with a grade estimate of 7.9.
* Chapter 11 reports zero Markdown lint errors and zero sentence-length
  flags.
* Chapter 11 adds a seven-line incident map, a six-line identity harm
  map, a nine-column risk register, a policy record, a live response
  board, an evidence log, and an AI security action gate.
* Chapter 11 cybercrime, identity theft, risk, incident response, and
  digital-forensics claims were checked against current primary sources
  from NIST, CISA, the FTC, DOJ, the House, and the Supreme Court on
  2026-07-12. All nine source links returned successful responses.

## Remaining Work

1. Rewrite Chapter 12 in plain language until it reaches the
   approved Flesch Reading Ease band of 60-70.
2. Run a chapter-by-chapter factual and legal review against primary
   sources. Recheck changeable laws and enforcement details near the
   publication date.
3. Run the full instructional review for MLO alignment, Bloom's level,
   retrieval practice, lab authenticity, and WCAG language.
4. Review Markdown formatting warnings inherited from the legacy files.
   The site builds cleanly, but blank lines, table separator style, and
   continued numbering need a deliberate formatting pass.
5. Inspect the live site on desktop and mobile after the first Pages
   deployment.
6. Create the final whole-book evaluation only after all 12 chapters pass
   the publication gates.

## Stable Design Decisions

* The textbook task list is `cis111`, not a term-specific list.
* The textbook has 12 chapters in four Parts.
* Chapter content does not prescribe pacing.
* Timing and course-shell mapping will be designed later.
* The official 18 district CLOs remain verbatim in the student-facing
  alignment blocks.
* Chapter scenarios may use dates or time spans as case facts. Those facts
  do not establish course pacing.

## Start Here Next Time

Begin with Chapter 12. Run the sentence-length check, readability score,
Markdown lint, style sweep, glossary check, link check, and clean build
after each chapter. Do not add weeks, due dates, exams, or term labels
to chapter content.
