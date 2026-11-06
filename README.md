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
## Development environment
- **[Visual Studio Code](https://code.visualstudio.com/)**: editor
- **[XML](https://marketplace.visualstudio.com/items?itemName=redhat.vscode-xml) (Red Hat)**: schema validation and content completion
- **[DitaCraft](https://github.com/jyjeanne/ditacraft)**: DITA-aware navigation, link checking, live preview and publishing
- **[DITA Open Toolkit](https://www.dita-ot.org/) 4.4.1**: publishing engine (PDF, HTML5)
- **Java 17 or later**: runtime required by DITA-OT
- **Git and [GitHub](https://github.com/)**: version control and hosting

## Building the manual
 
**Requirements:** Java 17 or later and [DITA-OT](https://www.dita-ot.org/download) 4.x, with its `bin` folder on the `PATH`.
 
```bash
# PDF
dita --input=map.ditamap --format=pdf
 
# HTML5
dita --input=map.ditamap --format=html5
```
 
The output is written to the `out/` folder, which Git ignores because generated files are not stored in the repository.
 
---
## About the author
 
Electrical engineer with **15+ years in marine and offshore power systems**: 15 years at sea
with Maersk, Rigel and Royal Caribbean, followed by design work onshore.
Today I am a **Senior Design Engineer** on offshore wind substation projects, where I verify
wiring diagrams against FAT, HIT and SAT/HAT procedures and **develop O&M manuals** for complex systems.

As 1st Electrical Engineer at Royal Caribbean I led a team of seven and was responsible for
the 6.6 kV power plant, propulsion, navigation and communication systems, including upgrade
projects such as a full radio-navigation replacement.

I bring two perspectives to documentation: the **operator** who has to live with a system,
and the **designer** who has to document it right. This project is part of my move into
**structured technical writing** with DITA and docs-as-code workflows.
 
📫 Connect with me on [LinkedIn](https://www.linkedin.com/in/grzegorz-trzeciak/)
