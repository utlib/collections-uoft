---
layout: default
title: Metadata Elements
nav_order: 20
parent: Documentation
description: "Collections U of T Metadata Elements"
permalink: /documentation/metadata_elements
---
# Collections U of T Metadata Elements

 > **DRAFT: further edits and instructions forthcoming.**

This page provides information about Collections U of T metadata and element details.

The [Collections U of T Metadata Spreadsheet Template](https://docs.google.com/spreadsheets/d/1PMtZt5CzkidIXbTBUaoi8Qg7kBU-m9RzeM-lBMORPks/edit?usp=sharing) is currently stored in Google Drive for easiest access (U of T OneDrive all-staff links have an expiry date).

# Collections U of T Metadata Profile - Element Details
_Draft - still working on this page._

## alma_record

* **Data Type:** URL
* **Input Guidelines:** Enter the full URL for the Alma MMS ID permalink. When converting from MARC, you will need to manually enter the Alma Record's Permalink URL.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/location.html#url](https://www.loc.gov/standards/mods/userguide/location.html#url) - with displayLabel="Alma Record" attribute
* **Controlled Vocabulary:** none
* **Obligation:** Optional
* **Repeatable?:** No

## alternate_identifier

* **Data Type:** string
* **Input Guidelines:** Use for Alternate Identifiers. Currently used by KCHA and USMC. Formerly usmc_pid in spreadsheet column.
* **MODS Input Guidelines:** none
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## call_number
* **Data Type:** string
* **Input Guidelines:** Enter the Call Number of the resource.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/identifier.html#url](https://www.loc.gov/standards/mods/userguide/identifier.html) with type="callnumber" attribute
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** Yes

## coordinates
* **Data Type:** string
* **Input Guidelines:** Enter coordinates information.
* **MODS Input Guidelines:** [[https://www.loc.gov/standards/mods/userguide/identifier.html](https://www.loc.gov/standards/mods/userguide/identifier.html) with type="callnumber" attribute](https://www.loc.gov/standards/mods/userguide/subject.html#coordinates)
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## creator_contributor
* **Data Type:** string
* **Input Guidelines:** Use to include the name of the creator or contributor to the resource. Do not break up name - include full name in the column. Separate multiple creator(s)/contributor(s) by pipe, including translations of names. 
If adding translations for names, separate by pipe. Indicate language per name value in Creator_Contributor_lang
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/name.html#namepart](https://www.loc.gov/standards/mods/userguide/name.html#namepart)
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** yes

## creator_contributor_lang
* **Data Type:** string
* **Input Guidelines:** "Enter the 2 character ISO 639-2 code for the language of the Creator_Contributor_lang value.

Note: this is not the language of the resource - it is the language of the Creator_Contributor_lang value.  This field is included in our metadata for accessibility purposes - it helps screenreaders understand the language of the value in the creator field. See [https://connect.library.utoronto.ca/display/DP/How+to+represent+languages+and+scripts+across+MODS+fields](https://connect.library.utoronto.ca/display/DP/How+to+represent+languages+and+scripts+across+MODS+fields) for background documentation. 

If multiple Creator_Contributor_lang values, enter language code within pipes in the same order that uniform titles appear in Creator_Contributor_lang. 

For transliterated names, include the language that will result in the screenreader reading the name correctly. 

If the value(s) is(are) multiple languages do not enter any value, leave blank. Default value is none."
* **MODS Input Guidelines:** Does not map according to MODS guidelines.
* **Controlled Vocabulary:** [https://www.loc.gov/standards/iso639-2/php/code_list.php](https://www.loc.gov/standards/iso639-2/php/code_list.php)

Look into internationalization use cases: [https://www.w3.org/2013/dwbp/wiki/RDF_AND_JSON-LD_UseCases](https://www.w3.org/2013/dwbp/wiki/RDF_AND_JSON-LD_UseCases)

See also [https://www.w3.org/International/questions/qa-choosing-language-tags](https://www.w3.org/International/questions/qa-choosing-language-tags)
* **Obligation:** optional
* **Repeatable?:** yes

## element
* **Data Type:**
* **Input Guidelines:** 
* **MODS Input Guidelines:** 
* **Controlled Vocabulary:** 
* **Obligation:** 
* **Repeatable?:** 

_Draft - still working on this page._
## element
* **Data Type:**
* **Input Guidelines:** 
* **MODS Input Guidelines:** 
* **Controlled Vocabulary:** 
* **Obligation:** 
* **Repeatable?:** 




