# Awesome Bible Developer Resources

![Awesome](https://awesome.re/badge.svg)  [![License: CC0-1.0](https://licensebuttons.net/l/zero/1.0/80x15.png)](http://creativecommons.org/publicdomain/zero/1.0/)  [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)

A curated list of awesome resources for developers (and other nerds) working with biblical texts and related tools.

For **non-specialist enthusiasts** (like myself), it can be challenging to get started and understand what types of formats and datasets are available. This awesome list will (hopefully) assist folks in *getting started* and identifying helpful biblical resources. 

For **specialists**, sometimes it can be hard to find links to relevant resources and associated tools and documentation (not least because so many links become dead over time)&mdash;this can help find available resource information and serve as a reference for onboarding colleagues to projects working with biblical corpora.

| :memo: :copyright: :registered: :tm:        | I've attempted to include badges for licenses for resources where known. When no badge is shown, assume the resource is copyright &copy; its respective author(s). The underlying corpora within resources may have separate licensing terms.       |
|---------------------------------------------|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|

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
    - [LXX](#lxx)
    - [New Testament](#new-testament)
  - [English Translations](#english-translations)
- [APIs](#apis)
- [Other Awesome Lists](#other-awesome-lists)


## Formats

*Formats / encodings used specifically for storing biblical texts and/or associated metadata (e.g., commentary, footnotes, annotations, tags, references, etc.).*

### Comparisons

Which format(s) should you use for your next project?

*It depends* on your goals and requirements. Here is some (hopefully) helpful information as you deliberate:

- Many formats predate Unicode standards and so may require specific fonts to render primary source languages. Modern formats should be Unicode-compliant.
- Most biblical texts / translations used in the Bible translation field are distributed in [USFM](#usfm) and [USX](#usx) formats ([USFM](#usfm) is one of the oldest SFM formats used to digitally store biblical translations).
- Many biblical primary source texts made available from academic centers/projects use [USFM](#usfm), [TEI](#tei), [Text-Fabric](#text-fabric), or plaintext formats.
- Some formats are only intended for biblical texts, whereas others can store texts themselves along with additional metadata, and others still are only for metadata, linguistic tagging, other annotations, etc. Be sure to review documentation for what each format supports.
- Article: [Bible File Encoding for Bible Translators, Publishers, and Software Developers](https://ebible.org/usfx/Bible-encoding.htm) by Kahunapule Michael Johnson

### Conversion Tools

- [Converting SFM Bibles to OSIS](https://wiki.crosswire.org/Converting_SFM_Bibles_to_OSIS) &mdash; Wiki page discussing the conversion of [USFM](#usfm) to [OSIS](#osis) format.

- [Haiola](https://haiola.org) &mdash; Accepts [USFM](#usfm), [USFX](#usfx), and [DBL](https://thedigitalbiblelibrary.org) [USX](#usx) file(s) input and outputs to a variety of user-friendly formats including (but not limited to) HTML, EPUB3, [SWORD Project](https://crosswire.org/sword/index.jsp) modules, Microsoft Word XML, and PDF.
  - [Haiola GitHub Repository](https://github.com/kahunapule/haiola) &mdash; Haiola GitHub repo.

- [SWORD to JSON Converter](https://github.com/wasdin/SWORD-to-JSON) [![License](https://img.shields.io/badge/License-BSD_2--Clause-orange.svg)](https://opensource.org/licenses/BSD-2-Clause) &mdash; Tool to convert SWORD modules to JSON.

### CES

The Corpus Encoding Standard (CES) is in a SGML format ([ISO 8879:1986](https://www.iso.org/standard/16387.html)) that is [TEI-compliant](#tei) and which is also available in XML format (XCES). CES is hosted by the Vassar College Department of Computer Science.

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
- [TEI XSL Stylesheets GitHub Repository](https://github.com/TEIC/Stylesheets) &mdash; GitHub repo with XSLT stylesheets to transform TEI XML documents to various formats, including XHTML, LaTeX, XSL Formatting Objects, ePub, plaintext, RDF, JSON; and to/from Word OOXML (docx) and OpenOfice (odt).
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
- [Paratext USX page](https://markups.paratext.org/usx/) &mdash; Main Paratext web page for USX with links to its documentation.
- [Digital Bible Library (DBL)](https://thedigitalbiblelibrary.org) &mdash; United Bible Societies (UBS) online digital asset and licensing management platform. DBL gathers, validates, and safeguards a large collection of quality, standardized, digital Scripture texts and publication assets in hundreds of languages that are predominantly in USX format.
- [DBL USX Documentation](https://app.thedigitalbiblelibrary.org/static/docs/usx/index.html) &mdash; DBL docs for USX format.

### Zefania

Simplistic XML format for Bible translations.

- [(Archived) Zefania XML Schema Documentation](https://web.archive.org/web/20180730154206/http://bgfdb.de/zefaniaxml/bml/) &mdash; Most links are now dead. This is an archived version from archive.org.
- [Brief History of Zefania XML](https://memim.com/zefania-xml.html) &mdash; Brief discussion of the origins of Zefania XML with concise examples of it. The [German Wikipedia page](https://de.wikipedia.org/wiki/Zefania_XML) also has some helpful information including example XML&mdash;but it's in German (the maintainer of this list created an English Wikipedia page that is [still in Draft](https://en.wikipedia.org/wiki/Draft:Zefania_XML) awaiting approval).
- [Zefania Bible Reader](https://github.com/NothinRandom/Zefania-Bible) &mdash; Zefania Bible is a XML file reader program that reads XML files entering them into database, and then displaying it on a site. Accompanying website no longer appears available. [There is another online reader for German translations](http://www.mathertel.de/AJAXEngine/S03_AJAXControls/BiblePage.aspx#version=luther1912&book=1&chapter=1&vers=1) also.
- [Zefania Bible Modules SourceForge Repository](https://sourceforge.net/projects/zefania-sharp/) &mdash; SourceForge repo of Zefania Bible translations in a variety of languages.


## Biblical Corpora

*Biblical corpora (i.e., bible translations and primary source texts) and related resources available for **download and offline use** in various formats.*

### Hebrew

- [ETCBC Biblia Hebraica Stuttgartensia Amstelodamensis (BHSa)](https://etcbc.github.io/bhsa/) [![License: CC BY-NC 4.0](https://licensebuttons.net/l/by-nc/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc/4.0/) &mdash; A [Text-Fabric](#text-fabric) version of the Hebrew Bible Database, containing the BHS text of the Hebrew Bible augmented with linguistic annotations compiled by the [Eep Talstra Centre for Bible and Computer (ETCBC), VU University Amsterdam](http://etcbc.nl). Available in [source repo](https://github.com/ETCBC/bhsa). The ETCBC has also shared a number of other great biblical and extrabiblical texts such as the [Peshitta](https://github.com/ETCBC/peshitta) (Syriac OT) along with the [Syriac NT](https://github.com/ETCBC/syrnt) and the [Dead Sea Scrolls (DSS)](https://github.com/ETCBC/dss).

- [MACULA Hebrew Linguistic Datasets](https://github.com/Clear-Bible/macula-hebrew/) [![License: CC BY 4.0](https://licensebuttons.net/l/by/4.0/80x15.png)](https://creativecommons.org/licenses/by/4.0/) &mdash; Syntax trees, morphology, and linguistic annotations for the Hebrew Bible based on the Westminster Leningrad Codex.

- [Open Bibles Hebrew Leningrad Codex](https://github.com/seven1m/open-bibles) [![License: CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/) *or* ![Public Domain](https://img.shields.io/badge/Public-Domain-brightgreen) &mdash; GitHub repository of public domain and freely (libre) licensed Bibles in XML formats (including [USFX](#usfx), [OSIS](#osis), and [Zefania](#zefania)). Hebrew Leningrad Codex available in [USFX](#usfx) format.

- [Open Hebrew Bible](https://github.com/eliranwong/OpenHebrewBible) &mdash; This project aligned Biblia Hebraica Stuttgartensia (BHS) with the Westminster Leningrad Codex (WLC); bridging ETCBC, OpenScriptures, and Berean data for the Hebrew Bible.

- [Open Scriptures Hebrew Bible (OSHB)](https://hb.openscriptures.org) [![License: CC BY 4.0](https://licensebuttons.net/l/by/4.0/80x15.png)](https://creativecommons.org/licenses/by/4.0/) &mdash; An open-licensed Hebrew Bible based on the [Westminster Leningrad Codex](http://www.tanach.us/Tanach.xml). Available in [OSIS](#osis) format in [source repo](https://github.com/openscriptures/morphhb).

- [OSIS Bibles](https://github.com/gratis-bible/bible) &mdash; A collection of freely licensed translations of biblical text in [OSIS format](#osis). Licensing varies per corpus. [Available Hebrew Bibles](https://github.com/gratis-bible/bible/tree/master/he) include Aleppo Codex, Biblia Hebraica Stuttgartensia (BHS), Open Scriptures Hebrew Bible (OSHB) tagged with Strong's numbers, and Westminster Leningrad Codex (WLC).

- [STEPBible Data](https://github.com/STEPBible/STEPBible-Data) [![License: CC BY 4.0](https://licensebuttons.net/l/by/4.0/80x15.png)](https://creativecommons.org/licenses/by/4.0/) &mdash; Numerous open-licensed datasets containing tagged Hebrew and Greek biblical texts saved as tab-separated value (TSV) files.

- [unfoldingWord&reg; Hebrew Bible (UHB)](https://www.unfoldingword.org/for-translators/content#UHB) [![License: CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/) &mdash; An open-licensed, lexically tagged, morphologically parsed Hebrew Old Testament. Based on the [Open Scriptures Hebrew Bible](https://hb.openscriptures.org). Available in [USFM](#usfm) format in [source repo](https://git.door43.org/unfoldingWord/hbo_uhb/src/branch/master). Lots of [additional great resources for Bible translators](https://www.unfoldingword.org/for-translators/content) including comprehensive [translation notes](https://www.unfoldingword.org/for-translators/content#UTN), lexical resources, etc.

- [Westminster Leningrad Codex (UXLC)](http://tanach.us) ![Public Domain](https://img.shields.io/badge/Public-Domain-brightgreen) &mdash; Unicode/XML Leningrad Codex (UXLC). Available in XML format with [TEI](#tei) header [at tanach.us website](http://tanach.us/Pages/XMLFiles.html), along with [plaintext](http://tanach.us/Pages/TextFiles.html), [HTML](http://tanach.us/Pages/HTMLFiles.html), and [other formats](http://tanach.us/Pages/About.html).


### Greek

- [Greek Learner Texts Project](https://greek-learner-texts.org) &mdash; A collaborative effort to produce openly-licensed, annotated texts in Ancient Greek for extensive reading. Has a section for [Biblical and Early Christian Texts](https://greek-learner-texts.org/texts/#biblical-and-early-christian-texts).


#### LXX

- [Computer Assisted Tools for Septuagint Studies (CATSS)](http://ccat.sas.upenn.edu/rak//catss.html) &mdash; Main page for CATSS with links to project's history, modules, bibliography, and related links. By [The International Organization for Septuagint and Cognate Studies (IOSCS)](http://ccat.sas.upenn.edu/ioscs/) at University of Pennsylvania. The [CATSS Biblical Texts](http://ccat.sas.upenn.edu/gopher/text/religion/biblical/) are available in the CCAT Gopher text archives. 
  - [Morphological Analysis of the LXX](http://ccat.sas.upenn.edu/gopher/text/religion/biblical/lxxmorph/). There is also [a third-party tool](https://github.com/orenfromberg/lxxproject) that uses this data to generate a SQLite database with book, verse, and word number attributes as well as root and morphological data.
  - [LXX Greek Textual Variants](http://ccat.sas.upenn.edu/gopher/text/religion/biblical/lxxvar/) (and [format explanation](http://ccat.sas.upenn.edu/gopher/text/religion/biblical/lxxvar/0-Explan.htm)).
  - [Parallel Hebrew // Greek Text Module](http://ccat.sas.upenn.edu/gopher/text/religion/biblical/parallel/).

- [Rahlfs' Septuagint](https://github.com/eliranwong/LXX-Rahlfs-1935) [![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/) &mdash; 1935 edition of Rahlfs' Septuagint with Unicode characters, morphology tagging, and a variety of other integrated datasets. Based on CATSS LXX (and base text is subject to applicable copyright restrictions).

- [Swete LXX Text](https://github.com/sleeptillseven/LXX-Swete/) :construction: [![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/) &mdash; *Partially-completed* Swete's LXX text from [First1KGreek Project](https://opengreekandlatin.github.io/First1KGreek/) (with corrections against manuscripts).


#### New Testament

- [Berean Greek Bible](https://greekbible.org) &mdash; Critical Greek New Testament that used Nestle 1904 as its [base text](https://sites.google.com/site/nestle1904/downloads). Requires [licensing approval](https://berean.bible/licensing.htm). Numerous [available formats and related resources](https://berean.bible/downloads.htm), including [USFM](#usfm), spreadsheets, PDFs, plaintext, and other document and e-reader formats.

- [Nestle 1904 Greek NT](https://github.com/biblicalhumanities/Nestle1904/) &mdash; Eberhard Nestle's 1904 GNT with various formats including morphology, lemmatization, Strong's numbers, XML markup (appears to be [OSIS](#osis) format), and glosses. [Base text](https://sites.google.com/site/nestle1904/downloads).

- [Open Greek New Testament (OGNT)](https://opengnt.com) [![License: CC BY-NC-SA 4.0](https://licensebuttons.net/l/by-nc-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-nc-sa/4.0/) &mdash; The OGNT is a Nestle-Aland 28th edition (NA28) / NA27 equivalent text with numerous associated resources in the [GitHub repo](https://github.com/eliranwong/OpenGNT).

- [Robinson's Greek Texts](https://byzantinetext.com) ![Public Domain](https://img.shields.io/badge/Public-Domain-brightgreen) &mdash; Dr. Maurice A. Robinson's Greek texts (most with morphological parsing and Strong's numbers). Robinson uses his own format for text storage with custom parsing codes and tense-voice-mood numbers. [Documentation of this format is available](https://github.com/byztxt/robinson-documentation) along with [a library of Python tools for working with the format](https://github.com/byztxt/librobinson). Some of the notable Greek texts are listed in the below sublistings.
  - **Byzantine Texts**
    - [Antoniades Patriarchal Greek NT (PATr)](https://byzantinetext.com/study/editions/antoniades/) &mdash; The 1904 text authorized by the Eucumenical Patriarchate of Constantinople for Eastern Orthodox churches with the 1912 corrections by Professor Vasileios Antoniades of the Theological School of Chalki. [GitHub repo](https://github.com/byztxt/greektext-antoniades) contains plaintext and parsed versions with morphological parsing tags and Strong's numbers.
    - [Elzevir Greek NT](https://byzantinetext.com/study/editions/elzevir/) &mdash; 1624 Elzevir Textus Receptus GNT edition. [GitHub repo](https://github.com/byztxt/greektext-elzevir) contains plaintext and parsed versions with morphological parsing tags and Strong's numbers.
    - [Robinson-Pierpont Byzantine Majority Greek NT](https://byzantinetext.com/study/editions/robinson-pierpont/) &mdash; Robinson-Pierpont edition of the Greek New Testament in the Original Greek, Byzantine Majority Text. [GitHub repo](https://github.com/byztxt/byzantine-majority-text) and [ByzantineText.com](https://byzantinetext.com/study/editions/robinson-pierpont/) contain various formats including with morphological parsing and Strong's numbers, collations with other texts, and PDFs.
    - [Scrivener Greek NT](https://byzantinetext.com/study/editions/scrivener/) &mdash; Frederick Henry Ambrose Scrivener's 1894 edition of the Textus Receptus GNT in a few formats. [GitHub repo](https://github.com/byztxt/greektext-scrivener) contains the text.
    - [Stephanus Greek NT](https://byzantinetext.com/study/editions/stephanus/) &mdash; Stephanus 1550 edition of the Textus Receptus GNT published by Robert Estienne in a few formats. [GitHub repo](https://github.com/byztxt/greektext-stephens) contains the text.
    - [Textus Receptus Greek NT](https://github.com/byztxt/greektext-textus-receptus) &mdash; Dr. Maurice A. Robinson's Textus Receptus Greek NT with morphological parsing tags and Strong's numbers.
  - **Alexandrian Texts**
    - [Westcott-Hort Greek NT](https://byzantinetext.com/study/editions/westcott-hort/) &mdash; Westcott and Hort's 1881 GNT. [GitHub repo](https://github.com/byztxt/greektext-westcott-hort) contains plaintext and parsed versions with morphological parsing tags and Strong's numbers.

- [Society of Biblical Literature (SBL) Greek NT (SBLGNT)](https://sblgnt.com) &mdash; A freely-available (but [copyrighted](https://www.sblgnt.com/license/)) critically edited Greek New Testament encoded in a Unicode-compliant font. Made available by [Logos Bible Software](https://www.logos.com/product/8486/the-greek-new-testament-sbl-edition) and the SBL in [a variety of formats](https://sblgnt.com/download/) including XML, [OSIS](#osis), [SWORD module](https://www.crosswire.org/sword/modules/ModInfo.jsp?modName=SBLGNT), plaintext, PDF, and more.
  - [MorphGNT SBLGNT](https://github.com/morphgnt/sblgnt) [![License: CC BY-SA 3.0](https://licensebuttons.net/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/3.0/) &mdash; Project to merge the MorphGNT morphological tagging analysis with the SBLGNT text. The text itself is subject to the [SBLGNT EULA](https://www.sblgnt.com/license/).

- [STEPBible Data](https://github.com/STEPBible/STEPBible-Data) [![License: CC BY 4.0](https://licensebuttons.net/l/by/4.0/80x15.png)](https://creativecommons.org/licenses/by/4.0/) &mdash; Numerous open-licensed datasets containing tagged Hebrew and Greek biblical texts saved as tab-separated value (TSV) files.

- [unfoldingWord&reg; Greek New Testament (UGNT)](https://www.unfoldingword.org/for-translators/content#UGNT) [![License: CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/) &mdash; An open-licensed, lexically tagged, morphologically parsed critical Greek New Testament with full apparatus. Based on the [Bunning Heuristic Prototype (BHP)](https://github.com/greekcntr/BHP) Greek NT from the [Center for New Testament Restoration (CNTR)](https://greekcntr.org/home/index.htm). Available in [USFM](#usfm) format in [source repo](https://git.door43.org/unfoldingWord/el-x-koine_ugnt/src/branch/master). Lots of [additional great resources for Bible translators](https://www.unfoldingword.org/for-translators/content) including comprehensive [translation notes](https://www.unfoldingword.org/for-translators/content#UTN), lexical resources, etc.


### English Translations

- [Multilingual Parallel Bible Corpus](https://github.com/christos-c/bible-corpus) [![License: CC0-1.0](https://licensebuttons.net/l/zero/1.0/80x15.png)](http://creativecommons.org/publicdomain/zero/1.0/) &mdash; A multilingual parallel corpus (aligned by verse) created from over 100 translations of the Bible intended for linguistic research and natural language processing (NLP) applications (e.g., statistical machine translation (SMT) training data, linguistic structure projected learning, etc.). There is also [a repo with associated tools](https://github.com/christos-c/bible-corpus-tools).

- [New English Translation of the Septuagint (NETS)](https://ccat.sas.upenn.edu/nets/) &mdash; Translation of LXX under Computer Assisted Tools for Septuagint Studies (CATSS) Project. Distributed as [PDF files](https://ccat.sas.upenn.edu/nets/edition/) and also available in print.

- [Open Bibles](https://github.com/seven1m/open-bibles) [![License: CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/) *or* ![Public Domain](https://img.shields.io/badge/Public-Domain-brightgreen) &mdash; GitHub repository of public domain and freely (libre) licensed Bibles in XML formats (including [USFX](#usfx), [OSIS](#osis), and [Zefania](#zefania)). Available English translations include KJV, BBE, OEB, and WEB. Also contains Hebrew Leningrad Codex, Clementine Latin Vulgate, and translations in other languages.

- [Open English Bible](https://openenglishbible.org) [![License: CC0-1.0](https://licensebuttons.net/l/zero/1.0/80x15.png)](http://creativecommons.org/publicdomain/zero/1.0/) &mdash; A public domain revision of [the Twentieth Century New Testament](https://github.com/openenglishbible/usfm-bibles/tree/master/Twentieth%20Century%20New%20Testament), which was a translation of the New Testament published in the early twentieth century based on the Greek text of Westcott and Hort. Available in [USFM](#usfm) and user-friendly format; has associated [GitHub repo](https://github.com/openenglishbible/Open-English-Bible).

- [OSIS Bibles](https://github.com/gratis-bible/bible) &mdash; A collection of freely licensed translations of biblical text in [OSIS format](#osis). Licensing varies per corpus.

- [SWORD Project](https://crosswire.org/sword/index.jsp) ![License: GPL](https://img.shields.io/badge/License-GPL-blue.svg) &mdash; CrossWire Bible Society's free Bible software project. Many [modules containing Bible texts](https://crosswire.org/sword/modules/ModDisp.jsp?modType=Bibles) (and [other resources](https://crosswire.org/sword/modules/index.jsp)) are available.
  - [pysword library](https://gitlab.com/tgc-dk/pysword) [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) &mdash; A third-party native Python reader package for SWORD Project Bible modules. [Documentation](https://tgc-dk.gitlab.io/pysword/) available.

- [unfoldingWord&reg; Literal Text (ULT)](https://www.unfoldingword.org/for-translators/content#ULT) [![License: CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/) &mdash; An open-licensed update of the ASV, intended to provide a ‘form-centric’ understanding of the Bible. It increases the translator’s understanding of the lexical and grammatical composition of the underlying text by adhering closely to the word order and structure of the originals. Available in [USFM](#usfm) format in [source repo](https://git.door43.org/unfoldingWord/en_ult/src/branch/master).

- [unfoldingWord&reg; Simplified Text (UST)](https://www.unfoldingword.org/for-translators/content#UST) [![License: CC BY-SA 4.0](https://licensebuttons.net/l/by-sa/4.0/80x15.png)](https://creativecommons.org/licenses/by-sa/4.0/) &mdash; An open-licensed translation, intended to provide a ‘functional’ understanding of the Bible. It increases the translator’s understanding of the text by translating theological terms as descriptive phrases. Available in [USFM](#usfm) format in [source repo](https://git.door43.org/unfoldingWord/en_ult/src/branch/master).

- [World English Bible (WEB)](https://worldenglish.bible) ![Public Domain](https://img.shields.io/badge/Public-Domain-brightgreen) &mdash; WEB is a modern English translation that is based on the American Standard Version (ASV) of the Holy Bible first published in 1901, the Biblia Hebraica Stutgartensa (BHS) Old Testament, and the Greek Majority Text New Testament. The companion Deuterocanon/Apocrypha is derived from the Revised Version Apocrypha and the Brenton translation of the Septuagint into English. It is in draft form and is currently being edited for accuracy and readability (although the Protestant Christian canon is essentially complete). Available in numerous formats including [USFX](#usfx), [USFM](#usfm), SWORD modules, Microsoft Word XML, HTML, plaintext, PDF, e-reader formats, XeTeX, and more.


## APIs

*Biblical corpora (i.e., bible translations and primary source texts) and related resources available for **online** use via application programming interfaces (APIs).*

- [API.Bible](https://scripture.api.bible) &mdash; American Bible Society (ABS) API with approximately 2500 Bible versions available across over 1600 languages. Free for non-commercial usage with limitations.

- [bible-api.com](https://bible-api.com) &mdash; Freely-available JSON API to obtain Bible text with [open-sourced app](https://github.com/seven1m/bible_api) and [Bible texts](https://github.com/seven1m/open-bibles). No API key required.

- [Biblia.com API](https://bibliaapi.com/docs/) &mdash; Faithlife / Logos Bible Software API for Bible text (multiple editions available).

- [Bible Brain API](https://www.faithcomesbyhearing.com/audio-bible-resources/bible-brain) &mdash; Faith Comes By Hearing&reg; API providing Bible text, audio, and video.

- [ESV API](https://api.esv.org) &mdash; English Standard Version (ESV) Bible API. Free for non-commercial usage with limitations.

- [getBible API v2](https://github.com/getbible/v2) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) &mdash; getBible API V2. No API key required. You can [programatically obtain the list of available translations.](https://getbible.net/v2/translations.json)

- [jsonBible API](https://jsonbible.com) &mdash; Freely-available Bible text API. No API key required.

- [NET API](https://labs.bible.org/api_web_service) &mdash; New English Translation (NET) Bible API. Does not appear to require an API key. [NETBibleTagger tool](https://labs.bible.org/NETBibleTagger/) also available to enable Bible reference tagging for a website (converts plaintext Bible references into hyperlinks with [customizable styles](https://labs.bible.org/NETBibleTagger/configure)).

- [NLT API](https://api.nlt.to) &mdash; New Living Translation (NLT) Bible API. Free for non-commercial usage with limitations. Anonymous limited use also available (without an API key).


## Other Awesome Lists

- [Awesome Bible Data](https://github.com/jcuenod/awesome-bible-data) &mdash; List of biblical data including translations, tagged original language texts, second temple literature, early church writings, dictionaries, and cross references.

- [Awesome Bible NLP](https://github.com/BibleNLP/awesome-bible-nlp) &mdash; A curated list of resources dedicated to Biblical Natural Language Processing (NLP).

- [Hackathon.Bible](https://hackathon.bible) &mdash; A resource site with Bible texts and datasets for building apps and new innovations for Bible engagement.
