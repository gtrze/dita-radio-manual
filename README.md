# Radio User Manual — DITA XML Portfolio Project
 
A complete user manual for a portable AM/FM radio, written in **DITA 1.3** and published to **PDF** and **HTML5** with the **DITA Open Toolkit**.
 
The project shows a structured authoring workflow: separating content by information type, writing task-oriented instructions, linking topics instead of duplicating them, and keeping documentation under version control like source code (docs-as-code).
 
---
 
## Highlights
 
- **Topic-based authoring.** Every topic answers one question for the reader and lives in its own file.
- **Information typing.** Content is separated into *concept* (what it is), *task* (how to do it) and *reference* (what the values are).
- **Task-oriented writing.** Imperative, one action per step, with prerequisites, expected results and follow-up actions.
- **Single source of truth.** Information is written once and linked from other topics instead of being copied.
- **Validated content.** All topics are validated against the DITA 1.3 XML Schemas.
- **Docs-as-code.** Plain-text sources in Git and command-line builds, with no proprietary tools required.
---
## Building the manual
 
**Requirements:** Java 17 or later and [DITA-OT](https://www.dita-ot.org/download) 4.x, with its `bin` folder on the `PATH`.
 
```bash
# PDF
dita --input=radio.ditamap --format=pdf
 
# HTML5
dita --input=radio.ditamap --format=html5
```
 
The output is written to the `out/` folder, which Git ignores because generated files are not stored in the repository.
 
---
## About the author
 
Electronics engineer (B.Eng. in marine radio electronics) developing skills in **structured technical writing** and **docs-as-code** workflows. This project is part of a hands-on study of the DITA standard, from the first topic to a complete, linked and version-controlled manual.
 
📫 Connect with me on [LinkedIn](https://www.linkedin.com/in/grzegorz-trzeciak/)
