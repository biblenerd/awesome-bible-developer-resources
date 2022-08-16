# Awesome Bible Developer Resources

![Awesome](https://awesome.re/badge.svg)  [![License: CC0-1.0](https://licensebuttons.net/l/zero/1.0/80x15.png)](http://creativecommons.org/publicdomain/zero/1.0/)  [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)

A curated list of awesome resources for developers (and other nerds) working with biblical texts and related tools.

For **non-specialist enthusiasts** (like myself), it can be challenging to get started and understand what types of formats and datasets are available. This awesome list will (hopefully) assist folks in *getting started* and identifying helpful biblical resources. For **specialists**, sometimes it can be hard to find links to relevant resources and associated tools and documentation (not least because so many links become dead over time)&mdash;this can help find available resource information and serve as a reference for onboarding colleagues to projects working with biblical corpora.

| :memo: :copyright: :registered: :tm:        | I've attempted to include badges for licenses for resources where known. When no badge is shown, assume the resource is copyright &copy; its respective author. The underlying corpora within resources may have separate licensing terms.       |
|---------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

## Contents

- [Formats](#Formats)
  - [Comparisons](#comparisons)
  - [Conversion Tools](#conversion-tools)
  - [CES](#ces)
  - [OSIS](#osis)
  - [TEI](#tei)
  - [Text-Fabric](#text-fabric)
  - [USFM](#usfm)
  - [USFX](#usfx)
  - [USX](#usx)
  - [Zefania](#zefania)
- [Biblical Corpora](#biblical-corpora)
  - [Hebrew](#hebrew)
  - [Greek](#greek)
  - [English Translations](#english-translations)
- [Other Awesome Lists](#other-awesome-lists)


## Formats

*Formats / encodings used specifically for storing biblical texts and/or associated metadata (e.g., commentary, footnotes, annotations, tags, references, etc.).*

### Comparisons

Which format(s) should you use for your next project?

*It depends* on your goals and requirements. Here is some (hopefully) helpful information as you deliberate:

- Most biblical texts / translations used in the Bible translation field are distributed in [USFM](#usfm) and [USX](#usx) formats ([USFM](#usfm) is one of the oldest SFM formats used to digitally store biblical translations).
- Many biblical primary source texts made available from academic centers/projects use [USFM](#usfm), [TEI](#tei), [Text-Fabric](#text-fabric), or plain text formats.
- Some formats are only intended for biblical texts, whereas others can store texts themselves along with additional metadata, and others still are only for metadata, linguistic tagging, other annotations, etc. Be sure to review documentation for what each format supports.
- Article: [Bible File Encoding for Bible Translators, Publishers, and Software Developers](https://ebible.org/usfx/Bible-encoding.htm) by Kahunapule Michael Johnson

### Conversion Tools

- [Haiola](https://haiola.org) &mdash; Accepts [USFM](#usfm), [USFX](#usfx), and [DBL](https://thedigitalbiblelibrary.org) [USX](#usx) file(s) input and outputs to a variety of user-friendly formats including (but not limited to) HTML, EPUB3, [SWORD Project](https://crosswire.org/sword/index.jsp) modules, Microsoft Word XML, and PDF.
  - [Haiola GitHub Repository](https://github.com/kahunapule/haiola) &mdash; Haiola GitHub repo.
- [Converting SFM Bibles to OSIS](https://wiki.crosswire.org/Converting_SFM_Bibles_to_OSIS) &mdash; Wiki page discussing the conversion of [USFM](#usfm) to [OSIS](#osis) format.

### CES

The Corpus Encoding Standard (CES) is in a SGML format (`ISO 8879:1986, Information Processing--Text and Office Systems--Standard Generalized Markup Language`) that is [TEI-compliant](#tei) and which is also available in XML format (XCES). CES is hosted by the Vassar College Department of Computer Science.

- [CES Documentation](https://www.cs.vassar.edu/CES/) &mdash; Main CES docs.
- [XML CES (XCES) Schema Documenation](https://www.cs.vassar.edu/XCES/schema/) &mdash; Main docs for XCES schema.

### OSIS

Open Scripture Information Standard (OSIS) XML format by CrossWire Bible Society. Used in [SWORD Project](https://crosswire.org/sword/index.jsp) (along with [TEI](#tei)).

- [CrossWire Bible Society OSIS page](https://crosswire.org/osis/) &mdash; Contains schema, manual, documentation, and tutorial.
- [OSIS Tutorial](https://wiki.crosswire.org/OSIS_Tutorial) &mdash; Walks through creation of a basic OSIS XML document.
- [eBible.org OSIS page](https://ebible.org/osis/) &mdash; Documentation of older version (2.1) of OSIS along with XSEM (precursor to OSIS) and OXES (closely-related format).
- [SIL XML Scripture Encoding Model (XSEM)](https://scripts.sil.org/XSEM) ![Deprecated](https://img.shields.io/badge/-DEPRECATED-red) &mdash; Docs for XML format that was a precursor to OSIS.
- [Open XML for Editing Scripture (OXES)](https://ebible.org/osis/oxes-documentation-2.0.3.pdf) ![Deprecated](https://img.shields.io/badge/-DEPRECATED-red) &mdash; Docs for OXES XML format which was closely related to OSIS.

### TEI

The Text Encoding Initiative (TEI) is a consortium which collectively develops and maintains guidelines for the representation of texts in digital form. The TEI guidelines are used by several notable content-based projects including:

- [British National Corpus](http://www.natcorp.ox.ac.uk)
- [Perseus Project](http://www.perseus.tufts.edu/)
- [Oxford Text Archive](http://ota.ox.ac.uk/)

List of TEI resources:

- [Text Encoding Initiative (TEI) main page](https://tei-c.org) &mdash; Main website for TEI.
- [TEI Guidelines GitHub Repository](https://github.com/TEIC/TEI) [![License: CC+BY 3.0](https://licensebuttons.net/l/by/4.0/80x15.png)](https://creativecommons.org/licenses/by/3.0/) *and* [![License](https://img.shields.io/badge/License-BSD_2--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause) &mdash; GitHub repo for TEI guidelines.
- [TEI XSL Stylesheets GitHub Repository](https://github.com/TEIC/Stylesheets) &mdash; GitHub repo with XSLT stylesheets to transform TEI XML documents to various formats, including XHTML, LaTeX, XSL Formatting Objects, ePub, plain text, RDF, JSON; and to/from Word OOXML (docx) and OpenOfice (odt).
- [TEI by Example](https://teibyexample.org) &mdash; Free tutorials for learning TEI XML.

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

- [ETCBC Biblia Hebraica Stuttgartensia Amstelodamensis (BHSa)](https://etcbc.github.io/bhsa/) [![License: CC BY-NC 4.0](https://licensebuttons.net/l/by-nc/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc/4.0/) &mdash; A [Text-Fabric](#text-fabric) version of the Hebrew Bible Database, containing the BHS text of the Hebrew Bible augmented with linguistic annotations compiled by the [Eep Talstra Centre for Bible and Computer (ETCBC), VU University Amsterdam](http://etcbc.nl). Available in [source repo](https://github.com/ETCBC/bhsa). The ETCBC has also shared a number of other great biblical and extrabiblical texts such as the [Peshitta](https://github.com/ETCBC/peshitta) (Syriac OT) along with the [Syriac NT](https://github.com/ETCBC/syrnt) and the [Dead Sea Scrolls (DSS)](https://github.com/ETCBC/dss).
- [MACULA Hebrew Linguistic Datasets](https://github.com/Clear-Bible/macula-hebrew/) [![License: CC BY 4.0](https://licensebuttons.net/l/by/4.0/80x15.png)](https://creativecommons.org/licenses/by/4.0/) &mdash; Syntax trees, morphology, and linguistic annotations for the Hebrew Bible based on the Westminster Leningrad Codex.
- [Open Bibles Hebrew Leningrad Codex](https://github.com/seven1m/open-bibles) [![License: CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/) *or* ![Public Domain](https://img.shields.io/badge/Public-Domain-brightgreen) &mdash; GitHub repository of public domain and freely (libre) licensed Bibles in XML formats (including [USFX](#usfx), [OSIS](#osis), and [Zefania](#zefania)). Hebrew Leningrad Codex available in [USFX](#usfx) format.
- [Open Scriptures Hebrew Bible (OSHB)](https://hb.openscriptures.org) [![License: CC BY 4.0](https://licensebuttons.net/l/by/4.0/80x15.png)](https://creativecommons.org/licenses/by/4.0/) &mdash; An open-licensed Hebrew Bible based on the [Westminster Leningrad Codex](http://www.tanach.us/Tanach.xml). Available in [OSIS](#osis) format in [source repo](https://github.com/openscriptures/morphhb).
- [OSIS Bibles](https://github.com/gratis-bible/bible) &mdash; A collection of freely licensed translations of biblical text in [OSIS format](#osis). Licensing varies per corpus. [Available Hebrew Bibles](https://github.com/gratis-bible/bible/tree/master/he) include Aleppo Codex, Biblia Hebraica Stuttgartensia (BHS), Open Scriptures Hebrew Bible (OSHB) tagged with Strong's numbers, and Westminster Leningrad Codex (WLC).
- [STEPBible Data](https://github.com/STEPBible/STEPBible-Data) [![License: CC BY 4.0](https://licensebuttons.net/l/by/4.0/80x15.png)](https://creativecommons.org/licenses/by/4.0/) &mdash; Numerous open-licensed datasets containing tagged Hebrew and Greek biblical texts saved as tab-separated value (TSV) files.
- [unfoldingWord&reg; Hebrew Bible (UHB)](https://www.unfoldingword.org/for-translators/content#UHB) [![License: CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/) &mdash; An open-licensed, lexically tagged, morphologically parsed Hebrew Old Testament. Based on the [Open Scriptures Hebrew Bible](https://hb.openscriptures.org). Available in [USFM](#usfm) format in [source repo](https://git.door43.org/unfoldingWord/hbo_uhb/src/branch/master). Lots of [additional great resources for Bible translators](https://www.unfoldingword.org/for-translators/content) including comprehensive [translation notes](https://www.unfoldingword.org/for-translators/content#UTN), lexical resources, etc.
- [Westminster Leningrad Codex (UXLC)](http://tanach.us) ![Public Domain](https://img.shields.io/badge/Public-Domain-brightgreen) &mdash; Unicode/XML Leningrad Codex (UXLC). Available in XML format with [TEI](#tei) header [at tanach.us website](http://tanach.us/Pages/XMLFiles.html), along with [plain text](http://tanach.us/Pages/TextFiles.html), [HTML](http://tanach.us/Pages/HTMLFiles.html), and [other formats](http://tanach.us/Pages/About.html).

### Greek

- [Greek Learner Texts Project](https://greek-learner-texts.org) &mdash; A collaborative effort to produce openly-licensed, annotated texts in Ancient Greek for extensive reading. Has a section for [Biblical and Early Christian Texts](https://greek-learner-texts.org/texts/#biblical-and-early-christian-texts).

#### LXX

- [Computer Assisted Tools for Septuagint Studies (CATSS) page](http://ccat.sas.upenn.edu/rak//catss.html) &mdash; Main page for CATSS with links to project's history, modules, bibliography, and related links. By [The International Organization for Septuagint and Cognate Studies (IOSCS)](http://ccat.sas.upenn.edu/ioscs/) at University of Pennsylvania. The [CATSS Biblical Texts](http://ccat.sas.upenn.edu/gopher/text/religion/biblical/) are available in the CCAT Gopher text archives. 
  - [Morphological Analysis of the LXX](http://ccat.sas.upenn.edu/gopher/text/religion/biblical/lxxmorph/).
  - [LXX Greek Textual Variants](http://ccat.sas.upenn.edu/gopher/text/religion/biblical/lxxvar/) (and [format explanation](http://ccat.sas.upenn.edu/gopher/text/religion/biblical/lxxvar/0-Explan.htm)).
  - [Parallel Hebrew // Greek Text Module](http://ccat.sas.upenn.edu/gopher/text/religion/biblical/parallel/).
- [Swete LXX Text](https://github.com/sleeptillseven/LXX-Swete/) :construction: [![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/) &mdash; *Partially-completed* Swete's LXX text from [First1KGreek Project](https://opengreekandlatin.github.io/First1KGreek/) (with corrections against manuscripts).

#### New Testament

- [STEPBible Data](https://github.com/STEPBible/STEPBible-Data) [![License: CC BY 4.0](https://licensebuttons.net/l/by/4.0/80x15.png)](https://creativecommons.org/licenses/by/4.0/) &mdash; Numerous open-licensed datasets containing tagged Hebrew and Greek biblical texts saved as tab-separated value (TSV) files.
- [unfoldingWord&reg; Greek New Testament (UGNT)](https://www.unfoldingword.org/for-translators/content#UGNT) [![License: CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/) &mdash; An open-licensed, lexically tagged, morphologically parsed critical Greek New Testament with full apparatus. Based on the [Bunning Heuristic Prototype (BHP)](https://github.com/greekcntr/BHP) Greek NT from the [Center for New Testament Restoration (CNTR)](https://greekcntr.org/home/index.htm). Available in [USFM](#usfm) format in [source repo](https://git.door43.org/unfoldingWord/el-x-koine_ugnt/src/branch/master). Lots of [additional great resources for Bible translators](https://www.unfoldingword.org/for-translators/content) including comprehensive [translation notes](https://www.unfoldingword.org/for-translators/content#UTN), lexical resources, etc.

### English Translations

- [Multilingual Parallel Bible Corpus](https://github.com/christos-c/bible-corpus) [![License: CC0-1.0](https://licensebuttons.net/l/zero/1.0/80x15.png)](http://creativecommons.org/publicdomain/zero/1.0/) &mdash; A multilingual parallel corpus (aligned by verse) created from over 100 translations of the Bible intended for linguistic research and natural language processing (NLP) applications (e.g., statistical machine translation (SMT) training data, linguistic structure projected learning, etc.). There is also [a repo with associated tools](https://github.com/christos-c/bible-corpus-tools).
- [New English Translation of the Septuagint (NETS)](https://ccat.sas.upenn.edu/nets/) &mdash; Translation of LXX under Computer Assisted Tools for Septuagint Studies (CATSS) Project. Distributed as [PDF files](https://ccat.sas.upenn.edu/nets/edition/) and also available in print.
- [Open Bibles](https://github.com/seven1m/open-bibles) [![License: CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/) *or* ![Public Domain](https://img.shields.io/badge/Public-Domain-brightgreen) &mdash; GitHub repository of public domain and freely (libre) licensed Bibles in XML formats (including [USFX](#usfx), [OSIS](#osis), and [Zefania](#zefania)). Available English translations include KJV, BBE, OEB, and WEB. Also contains Hebrew Leningrad Codex, Clementine Latin Vulgate, and translations in other languages.
- [Open English Bible](https://openenglishbible.org) [![License: CC0-1.0](https://licensebuttons.net/l/zero/1.0/80x15.png)](http://creativecommons.org/publicdomain/zero/1.0/) &mdash; A public domain revision of [the Twentieth Century New Testament](https://github.com/openenglishbible/usfm-bibles/tree/master/Twentieth%20Century%20New%20Testament), which was a translation of the New Testament published in the early twentieth century based on the Greek text of Westcott and Hort. Available in [USFM](#usfm) and user-friendly format; has associated [GitHub repo](https://github.com/openenglishbible/Open-English-Bible).
- [OSIS Bibles](https://github.com/gratis-bible/bible) &mdash; A collection of freely licensed translations of biblical text in [OSIS format](#osis). Licensing varies per corpus.
- [unfoldingWord&reg; Literal Text (ULT)](https://www.unfoldingword.org/for-translators/content#ULT) [![License: CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/) &mdash; An open-licensed update of the ASV, intended to provide a ‘form-centric’ understanding of the Bible. It increases the translator’s understanding of the lexical and grammatical composition of the underlying text by adhering closely to the word order and structure of the originals. Available in [USFM](#usfm) format in [source repo](https://git.door43.org/unfoldingWord/en_ult/src/branch/master).
- [unfoldingWord&reg; Simplified Text (UST)](https://www.unfoldingword.org/for-translators/content#UST) [![License: CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/) &mdash; An open-licensed translation, intended to provide a ‘functional’ understanding of the Bible. It increases the translator’s understanding of the text by translating theological terms as descriptive phrases. Available in [USFM](#usfm) format in [source repo](https://git.door43.org/unfoldingWord/en_ult/src/branch/master).


## Other Awesome Lists

- [Awesome Bible Data](https://github.com/jcuenod/awesome-bible-data) &mdash; List of biblical data including translations, tagged original language texts, second temple literature, early church writings, dictionaries, and cross references.
- [Awesome Bible NLP](https://github.com/BibleNLP/awesome-bible-nlp) &mdash; A curated list of resources dedicated to Biblical Natural Language Processing (NLP).
