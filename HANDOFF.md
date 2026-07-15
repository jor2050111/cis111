# CIS111 Textbook: Session Handoff

**Last updated:** 2026-07-15 (family template alignment)

**Repository:** [GitHub repository](https://github.com/jor2050111/cis111)

**Live site:** [CIS111 textbook](https://jor2050111.github.io/cis111/)

**Task list:** `CLAUDE_CODE_TASK_LIST_ID=cis111`, pinned in
`.claude/settings.json`

## What was done (2026-07-15): family template alignment

* zensical.toml dropped repo_url/repo_name/edit_uri and the
  content.action.edit/view features, so the header "Go to repository"
  link and the per-page view/edit icons are gone, matching CIS215.
* Chapter 12 now ends with "Course Conclusion: Where You Go from
  Here" (no icon) instead of "Looking Ahead".
* The conclusion gained a short next-steps paragraph (carry the
  five-move method into later courses and work).
* Converted the published glossary to definition lists with a
  student-facing preamble. Terms now render in canyon terracotta
  (light) and Phoenix Gold (dark) through synced brand.css.
* Chapters 2-12 rubric link blocks now tell students that instructors
  set the point weights per course. The synced rubric page carries a
  matching "A note on points" paragraph inside the transcluded block.
* Learning objectives dropped the MLO- prefix (entries now read
  `**N.Y (Level):**`), and Skills Lab parts read "Aligns with
  Objective(s) N.Y". CLAUDE.md, chapter templates, and the
  consistency-checker agent teach the new format.
* Left-nav Part labels now render as small uppercase headings (not
  links) in both color schemes, via synced brand.css.
* Rebuilt with `zensical build --clean`: No issues found.

## Current Status

The new CIS111 textbook repository is scaffolded and contains a complete
12-chapter legacy conversion. The book is schedule-neutral. It does not
assign chapters to weeks, terms, exams, or due dates. An instructor can
later map the same chapters into a 9-, 12-, 14-, or 16-week course.

All 12 chapters have completed their plain-language, source,
instructional, and whole-book reviews. The clean build and desktop and
mobile browser checks passed. The textbook is publication-ready.

The final evidence record is
`docs/FINAL-PUBLICATION-REVIEW.md`.

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
* Created a 221-entry glossary. Every chapter Key Terms entry resolves to
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
* The whole-book structural audit reports zero failures.
* Markdown lint reports zero errors across 47 authored files.
* The rendered site passes 2,090 internal-link and anchor checks.
* All 89 external links were checked. Seventy-two returned successful
  direct responses, and 17 official pages were confirmed in a browser
  or official indexed copy.
* The student home page reproduces all 18 district CLOs verbatim.
* Four Parts, 12 chapters, and all 12 navigation titles match.
* The 221 glossary definitions are unique.
* Desktop and mobile checks pass at 1440 by 900 and 390 by 844 pixels.
* No page-wide horizontal overflow appears. Wide rubric tables remain
  usable inside a horizontal scroll container.
* Every chapter has zero prose sentences at or above 35 words.
* Student-facing Markdown has zero em dashes, prose semicolons, and banned
  wording.
* Every chapter has exactly one Skills Lab goal and one evidence packet.
* Every chapter has exactly two Questions & Analysis prompts and four
  review questions.
* All chapter Key Terms entries resolve to the glossary.
* All evidence packet paths exist.
* Chapter 1 measures Flesch 60.1 with a grade estimate of 7.8.
* Chapter 1 reports zero Markdown lint errors and zero sentence-length
  flags.
* Chapter 2 measures Flesch 60.1 with a grade estimate of 7.7.
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
* Chapter 10 measures Flesch 66.2 with a grade estimate of 7.0.
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
* Chapter 11 measures Flesch 61.6 with a grade estimate of 7.8.
* Chapter 11 reports zero Markdown lint errors and zero sentence-length
  flags.
* Chapter 11 adds a seven-line incident map, a six-line identity harm
  map, a nine-column risk register, a policy record, a live response
  board, an evidence log, and an AI security action gate.
* Chapter 11 cybercrime, identity theft, risk, incident response, and
  digital-forensics claims were checked against current primary sources
  from NIST, CISA, the FTC, DOJ, the House, and the Supreme Court on
  2026-07-12. All nine source links returned successful responses.
* Chapter 12 measures Flesch 62.5 with a grade estimate of 7.6.
* Chapter 12 reports zero Markdown lint errors and zero sentence-length
  flags.
* Chapter 12 adds a six-line code record, five code critique tests, a
  licensing scope test, a credential card, a duty-to-control record, and
  an eight-step concern path.
* Chapter 12 professional-code, enforcement, credential, and AI risk
  claims were checked against current primary sources from ACM, IEEE,
  ISC2, and NIST on 2026-07-12. All five links were tested. The two ACM
  pages reject command-line checks, so their content was confirmed
  through browser-rendered or indexed copies.

## Remaining Work

No textbook build work remains. Course timing and course-shell mapping
remain separate future projects.

## Stable Design Decisions

* The textbook task list is `cis111`, not a term-specific list.
* The textbook has 12 chapters in four Parts.
* Chapter content does not prescribe pacing.
* Timing and course-shell mapping will be designed later.
* The official 18 district CLOs remain verbatim in the student-facing
  alignment blocks.
* Chapter scenarios may use dates or time spans as case facts. Those facts
  do not establish course pacing.

## Future Maintenance

Keep the book schedule-neutral. Do not add weeks, due dates, exams, or
term labels to chapter content. Re-run the final publication review after
any substantial legal, standards, source, navigation, or chapter change.
