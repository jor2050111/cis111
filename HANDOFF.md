# CIS111 Textbook: Session Handoff

**Last updated:** 2026-07-12

**Repository:** https://github.com/jor2050111/cis111

**Live site:** https://jor2050111.github.io/cis111/

**Task list:** `CLAUDE_CODE_TASK_LIST_ID=cis111`, pinned in
`.claude/settings.json`

## Current Status

The new CIS111 textbook repository is scaffolded and contains a complete
12-chapter legacy conversion. The book is schedule-neutral. It does not
assign chapters to weeks, terms, exams, or due dates. An instructor can
later map the same chapters into a 9-, 12-, 14-, or 16-week course.

The imported content has received a first standards pass, but it is not
yet the final publication edition. Chapter 1 has completed its full
plain-language and instructional review. Chapters 2-12 remain.

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
* Created a 201-entry glossary. Every chapter Key Terms entry resolves to
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

## Remaining Work

1. Rewrite Chapters 2-12 in plain language until each reaches the
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

Begin with Chapter 2. Run the sentence-length check, readability score,
Markdown lint, style sweep, glossary check, link check, and clean build
after each chapter. Do not add weeks, due dates, exams, or term labels
to chapter content.
