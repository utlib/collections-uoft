---
layout: default
title: Metadata Elements
nav_order: 5
parent: Documentation
description: "Collections U of T Metadata Elements"
permalink: /documentation/metadata_elements
---
# Collections U of T Metadata Elements

This page provides information about Collections U of T metadata and element details.

The [Collections U of T Metadata Spreadsheet Template](https://docs.google.com/spreadsheets/d/1PMtZt5CzkidIXbTBUaoi8Qg7kBU-m9RzeM-lBMORPks/edit?usp=sharing) is currently stored in Google Drive for easiest access (U of T OneDrive all-staff links have an expiry date).

# Collections U of T Metadata Profile - Element Details

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
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/subject.html#coordinates](https://www.loc.gov/standards/mods/userguide/subject.html#coordinates)
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

  * Note: this is not the language of the resource - it is the language of the Creator_Contributor_lang value.  This field is included in our metadata for accessibility purposes - it helps screen readers understand the language of the value in the creator field. See [https://connect.library.utoronto.ca/display/DP/How+to+represent+languages+and+scripts+across+MODS+fields](https://connect.library.utoronto.ca/display/DP/How+to+represent+languages+and+scripts+across+MODS+fields) for background documentation. If multiple Creator_Contributor_lang values, enter language code within pipes in the same order that uniform titles appear in Creator_Contributor_lang. For transliterated names, include the language that will result in the screen reader reading the name correctly. If the value(s) is(are) multiple languages do not enter any value, leave blank. Default value is none.
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
* **Input Guidelines:** A summary of the content of the resource - i.e. the abstract, description, or scope and content. Use plain text if possible. If necessary, available HTML tags include: &lt; a &gt; ; &lt; em &gt; ; &lt; strong &gt;. If &lt;p&gt; is needed use a pipe symbol as a separator. Do not use &lt;p&gt; or &lt;br /&gt; tags. 
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

## image
* **Data Type:** filepath
* **Input Guidelines:** Enter the file path to the image(s) for the digital object. (.tiff; .tif; .jpg extension). Book objects should be a directory (i.e. a folder) of images.
* **MODS Input Guidelines:** does not map
* **Controlled Vocabulary:** N/A
* **Obligation:** required
* **Repeatable?:** no

## issuance
* **Data Type:** string
* **Input Guidelines:** Mostly used when converting from MARC records. Do not use if data does not exist - controlled term that designates how the resource is issued.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/origininfo.html#issuance](https://www.loc.gov/standards/mods/userguide/origininfo.html#issuance)
* **Controlled Vocabulary:**
  - monographic
  - single unit 
  - multipart monograph
  - continuing 
  - serial
_See MODS Guidelines for explanation of each term._
* **Obligation:** optional
* **Repeatable?:** no

## issue
* **Data Type:** string
* **Input Guidelines:** Use to indicate the issue number. Suggestion is to enter as numerical value, but just be consistent across collection.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/part.html#number](https://www.loc.gov/standards/mods/userguide/part.html#number - with detail type="issue") - with detail type="issue"
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## language_code
* **Data Type:** string
* **Input Guidelines:** Enter the 3 character ISO 639-2 code for the language of the resource. If the resource contains multiple languages, enter language code within pipes in the same order that language text appears. Default value is none."
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/language.html#languageterm](https://www.loc.gov/standards/mods/userguide/language.html#languageterm)
* **Controlled Vocabulary:** [https://www.loc.gov/standards/iso639-2/php/code_list.php](https://www.loc.gov/standards/iso639-2/php/code_list.php) - use 3 character code
* **Obligation:** optional
* **Repeatable?:** yes

## pages
* **Data Type:** string
* **Input Guidelines:** "Enter the page range - i.e. #-#
  * Examples:10-35
  * Use to indicate the page numbers. Suggestion is to enter as numerical value, but just be consistent across collection.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/part.html#extent with unit="pages](https://www.loc.gov/standards/mods/userguide/part.html#extent with unit="pages")
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## language_text
* **Data Type:** string
* **Input Guidelines:** [Enter the text for the language of the resource from the ISO 639-2 list](https://www.loc.gov/standards/iso639-2/php/code_list.php)
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/language.html#languageterm](https://www.loc.gov/standards/mods/userguide/language.html#languageterm)
* **Controlled Vocabulary:** [https://www.loc.gov/standards/iso639-2/php/code_list.php](https://www.loc.gov/standards/iso639-2/php/code_list.php) - use text that matches code
* **Obligation:** optional
* **Repeatable?:** yes

## lccn_identifier
* **Data Type:** string
* **Input Guidelines:** LCCN Identifier - usually present when converting metadata from MARC records
* **MODS Input Guidelines:** none
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## member_of
* **Data Type:** string
* **Input Guidelines:** "Enter the PID of the collection (or book - for page objects) that the object belongs to. 
  * An object can only belong to one parent collection. 
  * Ingest error will result if collection does not yet exist - you must create the collection/book object before adding items/pages to a collection/book. "
* **MODS Input Guidelines:** N/A
* **Controlled Vocabulary:** N/A
* **Obligation:** required
* **Repeatable?:** yes

## note
* **Data Type:** string
* **Input Guidelines:** Separate multiple notes by pipes. Do not use for Description, Table_Of_Contents, Physical_Description_Note, or where text fits in other fields.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/note.html](https://www.loc.gov/standards/mods/userguide/note.html)
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** yes

## object_model
* **Data Type:** string
* **Input Guidelines:**
  * Enter the Collections U of T object model for the object:
    - Collection
    - Image
    - Book
    - Page

  * These terms are leftover from Islandora Object Models and represent the different types of objects Collections U of T contains and may be included in a metadata spreadsheet.
    - Collections: can contain books or images
    - Images: single image, can belong to one or more Collections
    - Book: multiple images, can belong to one or more Collections - a ""Book"" is not always an actual digitized book. It is any object with multiple images.
    - Page: single image, can belong to a Book
* **MODS Input Guidelines:** N/A
* **Controlled Vocabulary:**
  - Collection
  - Image
  - Book
  - Page
* **Obligation:** required
* **Repeatable?:** no

## ocr
* **Data Type:** string
* **Input Guidelines:** Enter the file path to the OCR .txt file for the digital object. 
* **MODS Input Guidelines:** does not map
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## digitized?
* **Data Type:** string
* **Input Guidelines:** Controlled field to indicate if digital object is metadata-only. 
* **MODS Input Guidelines:** does not map
* **Controlled Vocabulary:**
  * Digitized
  * Not yet digitized"
* **Obligation:** optional, default should be Digitized
* **Repeatable?:** no

## part_of
* **Data Type:** string
* **Input Guidelines:** Used if item is part of bigger archival collection; commonly used for linking to archival collections or fonds in Discover Archives.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/relateditem.html](https://www.loc.gov/standards/mods/userguide/relateditem.html) - with type="host" + displayLabel="Part Of" attributes and title information for the archival fonds/collection. 
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** yes

## part_of_constituent
* **Data Type:** string
* **Input Guidelines:** Often used when converting from MARC. A title of a constituent unit of the resource.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/relateditem.html](https://www.loc.gov/standards/mods/userguide/relateditem.html) - with type="constituent" + attribute and title information for the constituent unit.
* **Controlled Vocabulary:** none
* **Obligation:** optional 
* **Repeatable?:** yes

## part_of_constituent_creator
* **Data Type:** string
* **Input Guidelines:** Often used when converting from MARC. A name related to the constituent unit of the resource.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/relateditem.html](https://www.loc.gov/standards/mods/userguide/relateditem.html) - with type="constituent" + attribute and name information for the constituent unit.
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** yes

## part_of_series
* **Data Type:** string
* **Input Guidelines:** Used for series information if specified by collection owner/archives.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/relateditem.html](https://www.loc.gov/standards/mods/userguide/relateditem.html) - with type="series" + attribute and title information for the archival fonds/collection's series. 
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** yes

## physical_description_note
* **Data Type:** string
* **Input Guidelines:** Use for information relating to the physical description of a resource that does not fit in one of the other available subelements. Documentation on material and technique used for works of art and similar materials may be recorded here.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/physicaldescription.html#note](https://www.loc.gov/standards/mods/userguide/physicaldescription.html#note)
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** yes

## pid
* **Data Type:** string
* **Input Guidelines:** Enter the Collections U of T identifier for the object. PID will also become the end portion of the URL to the object (it helps to have meaningful PIDs - names or titles in the URL can help with Search Engine Optimization)
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/identifier.html](https://www.loc.gov/standards/mods/userguide/identifier.html) with type="local"
* **Controlled Vocabulary:** No. Where possible, use the call number, accession number, catkey, or meaningful identifier. 
* **Obligation:** required
* **Repeatable?:** no

## placeterm_code
* **Data Type:** string
* **Input Guidelines:**
  * Enter the code that best fits the place associated with the resource. Select most appropriate code from https://www.loc.gov/marc/countries/countries_code.html - DO NOT USE VALUES THAT BEGIN WITH ""-"" - for example ""-cn"" for Canada. These values are deprecated.
  * If multiple place names, enter a corresponding code per place. Separate codes with pipes and order them in the same order that place names appear in PlaceTerm_Text, ideally, but any code will also generate an internal MarkLogic placeTermTextFacet field which will automatically store the https://www.loc.gov/marc/countries/countries_code.html value and display it as a facet
  * Codes are managed in https://git.library.utoronto.ca/utl-its/digital-collections/collections-lookup/-/blob/main/src/__generated__/countryCodes.js
  * Invalid placeterm_code will result in an ingest validation error.

* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/origininfo.html#placeterm](https://www.loc.gov/standards/mods/userguide/origininfo.html#placeterm)
* **Controlled Vocabulary:** [https://www.loc.gov/marc/countries/countries_code.html](https://www.loc.gov/marc/countries/countries_code.html)
* **Obligation:** optional
* **Repeatable?:** yes

## placeterm_text
* **Data Type:** string
* **Input Guidelines:** "Enter the text value for the place associated with the resource. Any entries are allowed in this text field. Remember that the publicly displayed facet text is automatically generated by Collections U of T based on the placeterm_code, not the placeterm_text.
  * If multiple place name use pipes between values. For cities and countries use the entire value - i.e. Turkey, Istanbul and not Turkey|Istanbul or Toronto, Ontario and not Toronto|Ontario
  * Note: the placeterm_code value is what will be used as a facet. This field is just for keyword search and display."
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/origininfo.html#placeterm](https://www.loc.gov/standards/mods/userguide/origininfo.html#placeterm)
* **Controlled Vocabulary:** Ideally use values from [https://www.loc.gov/marc/countries/countries_code.html](https://www.loc.gov/marc/countries/countries_code.html) but placeterm_code will help with placeterm standardization for faceting purposes.
* **Obligation:** optional
* **Repeatable?:** yes

## projection
* **Data Type:** string
* **Input Guidelines:** Enter projection information.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/subject.html#projection](https://www.loc.gov/standards/mods/userguide/subject.html#projection)
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## provenance
* **Data Type:** string
* **Input Guidelines:** Used when converting from MARC. Not suggested for use if you are not starting with MARC data.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/note.html](https://www.loc.gov/standards/mods/userguide/note.html) - with type="ownership" attribute
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## publication_note
* **Data Type:** string
* **Input Guidelines:** Used by UTARMS for "More Information" to indicate publications related to the resource.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/note.html](https://www.loc.gov/standards/mods/userguide/note.html) - with type="publication note" attribute
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** yes

## publisher
* **Data Type:** string
* **Input Guidelines:** Enter the Publisher information.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/origininfo.html#publisher](https://www.loc.gov/standards/mods/userguide/origininfo.html#publisher)
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## related_materials_note
* **Data Type:** string
* **Input Guidelines:** Used by UTARMS for "Related Materials" and KCHA:root. Other collections use this as well.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/note.html](https://www.loc.gov/standards/mods/userguide/note.html) - with type="Related Materials" attribute
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** yes

## rights_facet
* **Data Type:** string
* **Input Guidelines:** Enter the rights facet. We need to define these across collections - should also map to IIIF Rights info - [https://iiif.io/api/cookbook/recipe/0008-rights/](https://iiif.io/api/cookbook/recipe/0008-rights/)
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/accesscondition.html](https://www.loc.gov/standards/mods/userguide/accesscondition.html) with type="restriction on access" attribute
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## rights_note
* **Data Type:** string
* **Input Guidelines:** Enter the rights information to display alongside the resource.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/accesscondition.html](https://www.loc.gov/standards/mods/userguide/accesscondition.html) with type="use and reproduction" attribute
* **Controlled Vocabulary:** none
* **Obligation:** required
* **Repeatable?:** yes

## scale
* **Data Type:** string
* **Input Guidelines:** Enter scale information.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/subject.html#scale](https://www.loc.gov/standards/mods/userguide/subject.html#scale)
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## statement_of_responsibility
* **Data Type:** string
* **Input Guidelines:** Mostly used for metadata converted from MARC. Value comes from 245 $c
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/note.html](https://www.loc.gov/standards/mods/userguide/note.html) - with type="statement of responsibility" attribute
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** yes

## subject_topic
* **Data Type:** string
* **Input Guidelines:** [Enter the subject/topic for the resource. Use LCSH or FAST where possible.](https://fast.oclc.org/searchfast/)
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/subject.html#topic](https://www.loc.gov/standards/mods/userguide/subject.html#topic)
* **Controlled Vocabulary:** Suggestion to use [https://fast.oclc.org/searchfast/](https://fast.oclc.org/searchfast/)
* **Obligation:** optional
* **Repeatable?:** yes

## subject_topic_mesh
* **Data Type:** string
* **Input Guidelines:** Enter subject terms from MESH. Used for anatomia:root.
* **MODS Input Guidelines:** [MESH browser](https://www.loc.gov/standards/mods/userguide/tableofcontents.html)
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** yes

## table_of_contents
* **Data Type:** string
* **Input Guidelines:** A table of contents for the resource. Should also map to IIIF manifest for the object - [https://iiif.io/api/cookbook/recipe/0024-book-4-toc/](https://iiif.io/api/cookbook/recipe/0024-book-4-toc/)
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/tableofcontents.html](https://www.loc.gov/standards/mods/userguide/tableofcontents.html)
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## thumbnail
* **Data Type:** filepath
* **Input Guidelines:** Enter the file path to the image that should be used as the thumbnail of the digital object. If left blank, default is to make the first image the thumbnail. 
* **MODS Input Guidelines:** does not map
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## title
* **Data Type:** string
* **Input Guidelines:** "Enter the title of the object. Title will also become the IIIF label. For display purposes try to keep title values limited to under 256 characters."
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/titleinfo.html](https://www.loc.gov/standards/mods/userguide/titleinfo.html)
* **Controlled Vocabulary:** N/A
* **Obligation:** required
* **Repeatable?:** no

## title_alternative
* **Data Type:** string
* **Input Guidelines:** Enter the alternative title of the object, if one exists (varying form of the title if it contributes to the further identification of the item).
  * For titles with multiple languages in different character sets, use the Title_Alternative tag for the Romanized titles in the ASCII character set and use Title_Translated for other translations. For an example, see the rclc-hkl:xhrb collection
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/titleinfo.html](https://www.loc.gov/standards/mods/userguide/titleinfo.html) - with type="alternative"
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** yes

## title_alternative_lang
* **Data Type:** string
* **Input Guidelines:** Enter the 2 character ISO 639-2 code for the language of the Title_Alternative value.
  * Note: this is not the language of the resource - it is the language of the Title_Alternative value.  This field is included in our metadata for accessibility purposes - it helps screen readers understand the language of the value in the title field. See [https://connect.library.utoronto.ca/display/DP/How+to+represent+languages+and+scripts+across+MODS+fields](https://connect.library.utoronto.ca/display/DP/How+to+represent+languages+and+scripts+across+MODS+fields) for background documentation. 
  * If multiple Title_Alternative values, enter language code within pipes in the same order that alternative titles appear in Title_Alternative. 
  * If the value(s) is(are) multiple languages do not enter any value, leave blank. Default value is none.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/titleinfo.html](https://www.loc.gov/standards/mods/userguide/titleinfo.html) - with type="alternative" and value contained in lang="" attribute
* **Controlled Vocabulary:** [https://www.loc.gov/standards/iso639-2/php/code_list.php](https://www.loc.gov/standards/iso639-2/php/code_list.php)
  * Look into internationalization use cases: [https://www.w3.org/2013/dwbp/wiki/RDF_AND_JSON-LD_UseCases](https://www.w3.org/2013/dwbp/wiki/RDF_AND_JSON-LD_UseCases)
  * See also [https://www.w3.org/International/questions/qa-choosing-language-tags](https://www.w3.org/International/questions/qa-choosing-language-tags)
* **Obligation:** optional
* **Repeatable?:** yes

## title_lang
* **Data Type:** string
* **Input Guidelines:** "Enter the 2 character ISO 639-2 code for the language of the Title value.
  * Note: this is not the language of the resource - it is the language of the Title value. This field is included in our metadata for accessibility purposes - it helps screen readers understand the language of the value in the title field. See https://connect.library.utoronto.ca/display/DP/How+to+represent+languages+and+scripts+across+MODS+fields for background documentation. 
  * If the title value is multiple languages do not enter any value, leave blank. Default value is none. 
  * See further instructions to add to Collections U of T documentation at https://connect.library.utoronto.ca/display/DP/How+to+represent+languages+and+scripts+across+MODS+fields
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/titleinfo.html](https://www.loc.gov/standards/mods/userguide/titleinfo.html) - value contained in lang="" attribute
* **Controlled Vocabulary:** [https://www.loc.gov/standards/iso639-2/php/code_list.php](https://www.loc.gov/standards/iso639-2/php/code_list.php)
  * Look into internationalization use cases: https://www.w3.org/2013/dwbp/wiki/RDF_AND_JSON-LD_UseCases
  * See also https://www.w3.org/International/questions/qa-choosing-language-tags
* **Obligation:** optional
* **Repeatable?:** no

## title_translated
* **Data Type:** string
* **Input Guidelines:** Enter the translated title of the object, if one exists (translation or transcription of the main title).
  * For titles with multiple languages in different character sets, use the Title_Alternative tag for the romanized titles in the ASCII character set and use Title_Translated for other translations. For an example, see the rclc-hkl:xhrb collection
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/titleinfo.html](https://www.loc.gov/standards/mods/userguide/titleinfo.html) - with type="translated"
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** yes

## title_translated_lang
* **Data Type:** string
* **Input Guidelines:** Enter the 2 character ISO 639-2 code for the language of the Title_Translated value.
  * Note: this is not the language of the resource - it is the language of the Title_Translated value.  This field is included in our metadata for accessibility purposes - it helps screen readers understand the language of the value in the title field. See https://connect.library.utoronto.ca/display/DP/How+to+represent+languages+and+scripts+across+MODS+fields for background documentation. 
  * If multiple Title_Translated values, enter language code within pipes in the same order that uniform titles appear in Title_Translated. 
  * There should not be multiple languages in this field. 
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/titleinfo.html](https://www.loc.gov/standards/mods/userguide/titleinfo.html) - with type="translated" and value contained in lang="" attribute
* **Controlled Vocabulary:** [https://www.loc.gov/standards/iso639-2/php/code_list.php](https://www.loc.gov/standards/iso639-2/php/code_list.php)
  * Look into internationalization use cases: https://www.w3.org/2013/dwbp/wiki/RDF_AND_JSON-LD_UseCases
  * See also [https://www.w3.org/International/questions/qa-choosing-language-tags](https://www.w3.org/International/questions/qa-choosing-language-tags)
* **Obligation:** optional
* **Repeatable?:** yes

## title_uniform
* **Data Type:** string
* **Input Guidelines:** This field is used most often when using MARC as the source of the metadata. The uniform title is used as a main entry in a bibliographic record. Used when a work has appeared under varying titles, necessitating that a particular title be chosen to represent the work.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/titleinfo.html](https://www.loc.gov/standards/mods/userguide/titleinfo.html)  - with type="uniform"
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** yes

## title_uniform_lang
* **Data Type:** string
* **Input Guidelines:** Enter the 2 character [ISO 639-2 code](https://www.loc.gov/standards/iso639-2/php/code_list.php) for the language of the Title_Uniform value.
  * Note: this is not the language of the resource - it is the language of the Title_Uniform value.  This field is included in our metadata for accessibility purposes - it helps screen readers understand the language of the value in the title field. See [https://connect.library.utoronto.ca/display/DP/How+to+represent+languages+and+scripts+across+MODS+fields](https://connect.library.utoronto.ca/display/DP/How+to+represent+languages+and+scripts+across+MODS+fields) for background documentation.  
  * If multiple Title_Uniform values, enter language code within pipes in the same order that uniform titles appear in Title_Uniform. 
  * If the value(s) is(are) multiple languages do not enter any value, leave blank. Default value is none.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/titleinfo.html](https://www.loc.gov/standards/mods/userguide/titleinfo.html) - with type="uniform" and value contained in lang="" attribute
* **Controlled Vocabulary:** [https://www.loc.gov/standards/iso639-2/php/code_list.php](https://www.loc.gov/standards/iso639-2/php/code_list.php)
  * Look into internationalization use cases: [https://www.w3.org/2013/dwbp/wiki/RDF_AND_JSON-LD_UseCases](https://www.w3.org/2013/dwbp/wiki/RDF_AND_JSON-LD_UseCases)
  * See also [https://www.w3.org/International/questions/qa-choosing-language-tags](https://www.w3.org/International/questions/qa-choosing-language-tags)
* **Obligation:** optional
* **Repeatable?:** yes

## type_of_resource
* **Data Type:** string
* **Input Guidelines:** See [https://www.loc.gov/standards/mods/userguide/typeofresource.html](https://www.loc.gov/standards/mods/userguide/typeofresource.html)
  * Use only the selected following terms from [https://id.loc.gov/vocabulary/resourceTypes.html](https://id.loc.gov/vocabulary/resourceTypes.html) :
    * artifact
    * cartographic
    * collection
    * mixed material
    * still image
    * text
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/typeofresource.html](https://www.loc.gov/standards/mods/userguide/typeofresource.html)
* **Controlled Vocabulary:** Use only the selected following terms from https://id.loc.gov/vocabulary/resourceTypes.html : 
    * artifact
    * cartographic
    * collection
    * mixed material
    * still image
    * text
_Use lower case_
* **Obligation:** required
* **Repeatable?:** no

## url_catkey
* **Data Type:** URL
* **Input Guidelines:** Enter the full URL of the old Sirsi Catkey. As of May, 2021 we will keep Sirsi permalinks as is for legacy purposes but always add Alma Record Permalinks going forward.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/location.html#url](https://www.loc.gov/standards/mods/userguide/location.html#url) - with displayLabel="Catalog Record" attribute
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## url_permalink
* **Data Type:** URL
* **Input Guidelines:** Enter the Collections U of T permalink. Take from the PID of the object. 
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/attributes.html#usage](https://www.loc.gov/standards/mods/userguide/attributes.html#usage) - with usage="primary display" access="object in context" attributes
* **Controlled Vocabulary:** none
* **Obligation:** required
* **Repeatable?:** no

## utarms_digital_object_id
* **Data Type:** string
* **Input Guidelines:** Used only by UTARMS for the object's digital object ID.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/identifier.html](https://www.loc.gov/standards/mods/userguide/identifier.html) with type="/search/utarms-online_display" displayLabel="digital item no" attributes
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## utarms_original_item_no
* **Data Type:** string
* **Input Guidelines:** Used only by UTARMS for the object's original ID.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/identifier.html](https://www.loc.gov/standards/mods/userguide/identifier.html) with type="/search/utarms-online" displayLabel="original identifier" attributes
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## viaf_name_identifier
* **Data Type:** URL
* **Input Guidelines:** A unique standard URI that distinctively identifies a Creator_Contributor name via VIAF. If multiple names in Creator_Contributor then enter VIAF URIs in order of Creator_Contributor names appear. If no VIAF, leave blank but include pipe.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/name.html#nameidentifier](https://www.loc.gov/standards/mods/userguide/name.html#nameidentifier) - with type="viaf"
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** yes

## viewing_direction
* **Data Type:** string
* **Input Guidelines:** Enter either "l2r" or "r2l" for ingests where digital objects have different viewing directions (i.e. fisher:root)
* **MODS Input Guidelines:** does not map
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no

## volume
* **Data Type:** string
* **Input Guidelines:** Use to indicate the volume number. Suggestion is to enter as numerical value, but just be consistent across collection.
* **MODS Input Guidelines:** [https://www.loc.gov/standards/mods/userguide/part.html#number](https://www.loc.gov/standards/mods/userguide/part.html#number) - with detail type="volume"
* **Controlled Vocabulary:** none
* **Obligation:** optional
* **Repeatable?:** no




