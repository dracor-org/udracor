# Ukrainian Drama Corpus (UDraCor)

This repository contains texts of Ukrainian plays from the 19th and early 20th centuries. All plays are encoded in [TEI/XML](https://tei-c.org/).

Texts are drawn from various digital sources, including:

* ukrlib.com.ua
* litopys.org.ua
* myslenedrevo.com.ua
* l-ukrainka.name
* i-franko.name
* uk.wikisource.org

The selection of plays is curated by Bohdan Tokarskyi, Daniil Skorinkin and Frank Fischer. The [corpus catalogue](https://docs.google.com/spreadsheets/d/1jVHVsWkMYdiwu1N3me-QpboGPDEKb7RiYaL2Y1SwhvE/edit?usp=sharing) lists 153 plays and their encoding status.

## Naming Conventions

Filenames and character IDs follow the Ukrainian National Transliteration standard ([KMU 2010](https://zakon.rada.gov.ua/laws/show/55-2010-%D0%BF)), using lowercase Latin letters without diacritics.

### Filenames

* Format: `{author-surname}-{title}.xml`
* Only the author's surname and the main title are used.
* Subtitles and bracketed alternative titles are omitted.
* Example: `shevchenko-nazar-stodolia.xml`

### Character IDs

* Applies to `xml:id` values on `<person>` and `<personGrp>`.
* Multi-word names use underscores; punctuation and quotation marks are omitted.
* Example: «Той, що греблі рве» → `toi_shcho_hrebli_rve`

### Transliteration and Reversibility

KMU 2010 is not reversible; different Cyrillic letters may map to the same Latin letter, the soft sign (ь) and apostrophe are dropped, and some mappings depend on word position. For example, Мокій → `mokii`, Аренський → `arenskyi`.

IDs serve as technical identifiers, not authoritative name forms. The original Cyrillic names are preserved in `<persName>` (or `<name>` for groups) within `<listPerson>`.
