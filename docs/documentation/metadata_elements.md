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

  * Note: this is not the language of the resource - it is the language of the Creator_Contributor_lang value.  This field is included in our metadata for accessibility purposes - it helps screenreaders understand the language of the value in the creator field. See [https://connect.library.utoronto.ca/display/DP/How+to+represent+languages+and+scripts+across+MODS+fields](https://connect.library.utoronto.ca/display/DP/How+to+represent+languages+and+scripts+across+MODS+fields) for background documentation. If multiple Creator_Contributor_lang values, enter language code within pipes in the same order that uniform titles appear in Creator_Contributor_lang. For transliterated names, include the language that will result in the screenreader reading the name correctly. If the value(s) is(are) multiple languages do not enter any value, leave blank. Default value is none.
* **MODS Input Guidelines:** Does not map according to MODS guidelines.
* **Controlled Vocabulary:** [https://www.loc.gov/standards/iso639-2/php/code_list.php](https://www.loc.gov/standards/iso639-2/php/code_list.php)

  * Look into internationalization use cases: [https://www.w3.org/2013/dwbp/wiki/RDF_AND_JSON-LD_UseCases](https://www.w3.org/2013/dwbp/wiki/RDF_AND_JSON-LD_UseCases)

  * See also [https://www.w3.org/International/questions/qa-choosing-language-tags](https://www.w3.org/International/questions/qa-choosing-language-tags)
* **Obligation:** optional
* **Repeatable?:** yes

## creator_contributor_role
* **Data Type:** string
* **Input Guidelines:** Default is none. Use from list of controlled values selected from [https://id.loc.gov/vocabulary/relators.html](https://id.loc.gov/vocabulary/relators.html)

  * If multiple names, enter roles within pipes in the same order that names appear in Creator_Contributor. 

  * If multiple roles per name, separate with a comma. Note that all roles will display beside the name except ""none"" (i.e. don't add too many roles, it will display strangely).

  * Custom terms not on MARC relators list: 
    * none
    * autograph (not in MODS role term - ""autographer"" is, but Fisher use ""autograph"")
    * book label (not in MODS role term)
    * bookstamp (not in MODS role term)
    * stenographer (not in MODS role terms)

  * Track additional _role terms in https://git.library.utoronto.ca/utl-its/digital-collections/collections-mods-generator/-/blob/main/src/config/roleCodes.js and https://git.library.utoronto.ca/utl-its/digital-collections/collections-lookup/-/blob/main/src/__generated__/relators.js"
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/name.html#role](https://www.loc.gov/standards/mods/userguide/name.html#role )
* **Controlled Vocabulary:** Selected term values taken from [https://www.loc.gov/marc/relators/relaterm.html](https://www.loc.gov/marc/relators/relaterm.html)
* **Obligation:** optional
* **Repeatable?:** yes

## credit
* **Data Type:** string
* **Input Guidelines:** Enter the Credit information. 
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/accesscondition.html](https://www.loc.gov/standards/mods/userguide/accesscondition.html) with type="credit" attribute
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## date_facet
* **Data Type:** string
* **Input Guidelines:** "Date used for facets. For the <dateOther> tag, when converting from MARC, you will likely need to manually enter the dateOther tag. This field is used to record the decade of the date for simple facets by either:

  * a) decade - i.e. 1900s, 1910s, 1950s

  * or b) century - i.e. 15th century, 13th century, 20th century. Use decades unless collection/object spans over 4 decades. For Fisher manuscripts, use Century. 

  * For objects that fall within a range of dates, add multiple decades or centuries."
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/origininfo.html#dateother](https://www.loc.gov/standards/mods/userguide/origininfo.html#dateother)
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** yes

## date_full
* **Data Type:** string
* **Input Guidelines:** Date used for display.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/origininfo.html#dateissued](https://www.loc.gov/standards/mods/userguide/origininfo.html#dateissued)
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** yes

## description
* **Data Type:** string
* **Input Guidelines:** A summary of the content of the resource - i.e. the abstract, description, or scope and content. Use plain text if possible. If necessary, available HTML tags: <a>; <em>; <strong>. If <p> is needed use | as a separator. Do not use <p> or <br /> tags. 
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/abstract.html](https://www.loc.gov/standards/mods/userguide/abstract.html)
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** yes

## edition
* **Data Type:** string
* **Input Guidelines:** Information identifying the version of the resource.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/origininfo.html#edition](https://www.loc.gov/standards/mods/userguide/origininfo.html#edition )
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## extent
* **Data Type:** string
* **Input Guidelines:** A statement about the physical extent of the resource, in terms of units of measurement and material.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/physicaldescription.html#extent](https://www.loc.gov/standards/mods/userguide/physicaldescription.html#extent)
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** yes

## fisher_f_number
* **Data Type:** string
* **Input Guidelines:** Used **only** for Fisher collections. Contains only the F#. 
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/identifier.html](https://www.loc.gov/standards/mods/userguide/identifier.html) with type="fisher_f_number" attribute
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## form_gmd
* **Data Type:** string
* **Input Guidelines:** Mostly used when converting from MARC records. Do not use if data does not exist.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/physicaldescription.html#form](https://www.loc.gov/standards/mods/userguide/physicaldescription.html#form) - with authority="gmd" attribute
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## form_marcform
* **Data Type:** string
* **Input Guidelines:** Mostly used when converting from MARC records. Do not use if data does not exist.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/physicaldescription.html#form](https://www.loc.gov/standards/mods/userguide/physicaldescription.html#form) - with authority="marcform" attribute
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## genre
* **Data Type:** string
* **Input Guidelines:** "Contains terms that give more specificity for the form of an object than the broad terms used in <typeOfResource>

  * When converting from MARC, please delete any period that completes the term in this tag.

  * If cartographic, use ""map"" value to be consistent across collections."
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/genre.html](https://www.loc.gov/standards/mods/userguide/genre.html)
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** yes

## holding_institution
* **Data Type:** string
* **Input Guidelines:** "The Holding Institution, or UTL department, that cares for the object. Use consistent naming across collections:
  - Map & Data Library, University of Toronto Libraries
  - Richard Charles Lee Canada-Hong Kong Library
  - Thomas Fisher Rare Book Library
  - University of Toronto Archives
  - University of St. Michael's College Archives
  - University of St. Michael's College, John M. Kelly Library, Special Collections
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/location.html#physicallocation](https://www.loc.gov/standards/mods/userguide/location.html#physicallocation)
* **Controlled Vocabulary:** none
* **Obligation:** Required
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




