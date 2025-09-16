# Ukrainian Drama Corpus (UDraCor)

This repository contains texts of Ukrainian plays from the 19th and early 20th centuries. All plays are encoded in [TEI/XML](https://tei-c.org/). The TEI documents included here originate from a variety of sources, namely:

* ukrlib.com.ua
* litopys.org.ua
* myslenedrevo.com.ua
* l-ukrainka.name
* i-franko.name

… plus some others. The list of plays selected for encoding is curated by Dr. Bohdan Tokarskyi and Daniil Skorinkin. The current catalogue (153 plays), along with the status of their encoding, is available [here](https://docs.google.com/spreadsheets/d/1jVHVsWkMYdiwu1N3me-QpboGPDEKb7RiYaL2Y1SwhvE/edit?usp=sharing).

This work is supported by Mark Schwindt and Frank Fischer, who contributed to consistency checking, metadata enrichment, and the integration of Wikidata IDs.

## Filename Conventions

* All filenames in this corpus follow DraCor's standard lowercase naming convention.
* Author names: We use the last name as listed in the author's English-language Wikipedia entry.
* Titles of plays: We transliterate them using the Python package [transliterate](https://pypi.org/project/transliterate/) with the Ukrainian language code (uk).
* Example: "shevchenko-nazar-stodolja.xml"
