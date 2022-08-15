# Awesome Bible Developer Resources  ![Awesome](https://awesome.re/badge.svg)  [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)

A curated list of awesome resources for developers (and other nerds) working with biblical texts and related tools.

| :memo: :copyright: :registered: :tm:        | I've attempted to include badges for licenses for resources where known. When no badge is shown, assume the resource is copyright &copy; its respective author. The underlying corpora within resources may have separate licensing terms.       |
|---------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## Contents

- [Formats](#Formats)
  - [Comparisons](#comparisons)
  - [Conversion Tools](#conversion-tools)
  - [OSIS](#osis)
  - [Text-Fabric](#text-fabric)
  - [USFM](#usfm)
  - [USFX](#usfx)
  - [USX](#usx)
  - [Zefania](#zefania)
- [Biblical Corpora](#biblical-corpora)
  - [Hebrew](#hebrew)
  - [Greek](#greek)
  - [Mixed Repositories](#mixed-repositories)
- [Other Awesome Lists](#other-awesome-lists)


## Formats

*Formats / encodings used specifically for storing biblical texts and/or associated metadata (e.g., commentary, footnotes, annotations, tags, references, etc.). Does not include common technical formats/types used in multiple domains that are sufficiently documented elsewhere (e.g., CSV, XML, JSON, SQLite, LaTeX, etc.).*

### Comparisons

Which format(s) should you use for your next project?

- Most biblical texts / translations are distributed in USFM and USX formats.
- Some formats are only intended for biblical texts, whereas others can store texts themselves along with additional metadata, and others still are only for metadata, linguistic tagging, other annotations, etc. Be sure to review documentation for what each format supports.
- Article: [Bible File Encoding for Bible Translators, Publishers, and Software Developers](https://ebible.org/usfx/Bible-encoding.htm) by Kahunapule Michael Johnson

### Conversion Tools

- [Haiola](https://haiola.org) &mdash; Accepts [USFM](#usfm), [USFX](#usfx), and [DBL](https://thedigitalbiblelibrary.org) [USX](#usx) file(s) input and outputs to a variety of user-friendly formats including (but not limited to) HTML, EPUB3, [SWORD Project](https://crosswire.org/sword/index.jsp) modules, Microsoft Word XML, and PDF.
  - [Haiola GitHub Repository](https://github.com/kahunapule/haiola) &mdash; Haiola GitHub repo.

### OSIS

Open Scripture Information Standard (OSIS) XML format by CrossWire Bible Society. Used in [SWORD Project](https://crosswire.org/sword/index.jsp).

- [CrossWire Bible Society OSIS page](https://crosswire.org/osis/) &mdash; Contains schema, manual, documentation, and tutorial.
- [OSIS Tutorial](https://wiki.crosswire.org/OSIS_Tutorial) &mdash; Walks through creation of a basic OSIS XML document.
- [eBible.org OSIS page](https://ebible.org/osis/) &mdash; Documentation of older version (2.1) of OSIS along with XSEM (precursor to OSIS) and OXES (closely-related format).
- [SIL XML Scripture Encoding Model (XSEM)](https://scripts.sil.org/XSEM) ![Deprecated](https://img.shields.io/badge/-DEPRECATED-red) &mdash; Docs for XML format that was a precursor to OSIS.
- [Open XML for Editing Scripture (OXES)](https://ebible.org/osis/oxes-documentation-2.0.3.pdf) ![Deprecated](https://img.shields.io/badge/-DEPRECATED-red) &mdash; Docs for OXES XML format which was closely related to OSIS.

### Text-Fabric

Text-Fabric is a format and accompanying Python library / API for working with ancient texts and associated linguistic annotations as annotated graphs. It can accept corpora in a variety of formats and convert these to TF format.

- [Main GitHub repository](https://github.com/annotation/text-fabric) &mdash; Main repository for file format and API.
- [`tf` package documentation](https://annotation.github.io/text-fabric/tf/index.html) &mdash; Docs for `tf` Python package.

### USFM

Unified Standard Format Markers (USFM) was developed within [Paratext](https://paratext.org/) for Bible translations.

- [Paratext USFM page](https://paratext.org/usfm/) &mdash; Main Paratext web page for USFM with a brief history of the format and links to its documentation and Paratext stylesheets.
- [USFM GitHub Repository](https://github.com/ubsicap/usfm) &mdash; Main USFM GitHub repo.
- [USFM Documentation](http://ubsicap.github.io/usfm/) &mdash; USFM docs.
- [USFM Tools](https://github.com/openenglishbible/USFM-Tools) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) &mdash; Python tools for parsing and rendering USFM files.

### USFX

Unified Scripture Format XML (USFX) is an XML format that was derived from [USFM](#usfm). 

[![License: LGPL v2,1+](https://img.shields.io/badge/License-LGPL_v2.1-blue.svg)](https://www.gnu.org/licenses/old-licenses/lgpl-2.1.html) *or* [![License: Common Public License 0.5+](https://img.shields.io/badge/License-CPL_0.5-red.svg)](https://www.eclipse.org/legal/cpl-v05.html) (see [LICENSING.txt](https://ebible.org/usfx/LICENSING.txt)).

- [USFX eBible.org main page](https://ebible.org/usfx/) &mdash; Main USFX page describing what it is, links to its schema and documentation, and how it differs from [USFM](#usfm), [USX](#usx), and [OSIS](#osis).
- [USFX Schema Documentation](https://ebible.org/usfx/usfx.htm) &mdash; USFX schema docs.

### USX

Unified Scripture XML (USX) is an XML format that is closely related to [USFM](#usfm). Used by [Paratext](https://paratext.org/) and the [DBL](https://thedigitalbiblelibrary.org).

- [USX GitHub Repository](https://github.com/ubsicap/usx) &mdash; Main USX GitHub repo.
- [USX Documentation](https://ubsicap.github.io/usx/) &mdash; USX docs.
- [Paratext USX page](https://markups.paratext.org/usx/) &mdash; Main Paratext web page for USFM with links to its documentation.
- [Digital Bible Library (DBL)](https://thedigitalbiblelibrary.org) &mdash; United Bible Societies (UBS) online digital asset and licensing management platform. DBL gathers, validates, and safeguards a large collection of quality, standardized, digital Scripture texts and publication assets in hundreds of languages that are predominantly in USX format.

### Zefania

Simplistic XML format for Bible translations.

- [Zefania Bible Modules SourceForge Repository](https://sourceforge.net/projects/zefania-sharp/) &mdash; SourceForge repo of Zefania Bible translations in a variety of languages.


## Biblical Corpora

*Biblical corpora (i.e., bible translations and primary source texts) in various formats.*

### Hebrew

TODO

### Greek

- [Computer Assisted Tools for Septuagint Studies (CATSS) page](http://ccat.sas.upenn.edu/rak//catss.html) &mdash; Main page for CATSS with links to project's history, modules, bibliography, and related links. By [The International Organization for Septuagint and Cognate Studies (IOSCS)](http://ccat.sas.upenn.edu/ioscs/) at University of Pennsylvania. The [CATSS Biblical Texts](http://ccat.sas.upenn.edu/gopher/text/religion/biblical/) are available in the CCAT Gopher text archives. 
  - [Morphological Analysis of the LXX](http://ccat.sas.upenn.edu/gopher/text/religion/biblical/lxxmorph/).
  - [LXX Greek Textual Variants](http://ccat.sas.upenn.edu/gopher/text/religion/biblical/lxxvar/) (and [format explanation](http://ccat.sas.upenn.edu/gopher/text/religion/biblical/lxxvar/0-Explan.htm)).
  - [Parallel Hebrew // Greek Text Module](http://ccat.sas.upenn.edu/gopher/text/religion/biblical/parallel/).

### English Translations

- [New English Translation of the Septuagint (NETS)](https://ccat.sas.upenn.edu/nets/) &mdash; Translation of LXX under Computer Assisted Tools for Septuagint Studies (CATSS) Project. Distributed as [PDF files](https://ccat.sas.upenn.edu/nets/edition/) and also available in print.

### Mixed Repositories

Repositories of multiple biblical corpora (i.e., doesn't fit into a single subcategory).

- [Open Bibles](https://github.com/seven1m/open-bibles) [![License: CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/) *or* ![Public Domain](https://img.shields.io/badge/Public-Domain-brightgreen) &mdash; GitHub repository of public domain and freely (libre) licensed Bibles in XML formats (including [USFX](#usfx), [OSIS](#osis), and [Zefania](#zefania)). Available English translations include KJV, BBE, OEB, and WEB. Also contains Hebrew Leningrad Codex, Clementine Latin Vulgate, and translations in other languages (e.g., several in Spanish, others in Cherokee, Dutch, Czech, Japanese, Portuguese, and Romanian).

## Other Awesome Lists

- [Awesome Bible Data](https://github.com/jcuenod/awesome-bible-data) &mdash; List of biblical data including translations, tagged original language texts, second temple literature, early church writings, dictionaries, and cross references.
