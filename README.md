# Collections U Of T

## About this page
This documentation is intended for:
* U of T staff using Collections U of T
* Open technology community members interested in Collections U of T technology infrastructure
* Researchers or public users interested in browsing and searching U of T's digital collections 

As of March 2023 this documentation status is *draft* and has not been approved by UTL Senior Staff.

**Skip to:**
* [About Collections U of T](README.md#about-collections-u-of-t)
* Documentation for collection owners
    * Requesting a top-level collection
    * [Metadata instructions](docs/metadata_template_instructions.md)
    * [Ingest instructions](docs/ingest_instructions.md)
* Documentation for getting started with Collections U of T
    * Searching
    * [What is IIIF?](docs/iiif-collections-u-of-t.md)
        * Using IIIF - Tools
        * Using IIIF - Downloading
        * Using IIIF - Embedding

## About Collections U of T
[Collections U of T](https://collections.library.utoronto.ca) is the  University of Toronto Libraries' image repository for digitized special collections and archives. It provides open access to these digital image collections through the [International Image Interoperability Framework (IIIF)](https://iiif.io/) and standard metadata formats. 

Collections U of T provides U of T staff:

1. Collection management and digital object storage for university special collections and archives image collections
2. Indexing for digital object metadata
3. Search and discovery for collections and digital objects
4. User management and authentication (CRUD for collections and digital objects)
5. Statistics for collections and digital objects
6. "Exhibit" pages about collections and items stored in Collections U of T

Collections U of T is not:
* A digitization service
* A digital exhibit service
* A digital preservation service
* Able to store media types other than image files. Note: it does not currently support .pdf, audio, or video collections
* Open to anyone - digital collections must be *assessed* prior to inclusion. Because the service is intended for providing long term discovery and display of access copies of digital collections, the digital objects must belong to a UTL department or archives and be assessed by a UTL staff collection owner prior to inclusion. UTL collection owners are responsible for assessing digital objects for accessibility, privacy and copyright considerations, as well as staffing capacity to support the care and maintenance of the digital collection over time. 

UTL staff can request a consultation for Collections U of T support at [digitalinitiatives@library.utoronto.ca](mailto:digitalinitiatives@library.utoronto.ca).

Researchers, students, and faculty can read documentation provided here to learn how to use the system. Please send any questions or feedback to [digitalinitiatives@library.utoronto.ca](mailto:digitalinitiatives@library.utoronto.ca).

### List of Top-Level Collections in Collections U of T

As of March 2023, Collections U of T holds selected digital objects for the following libraries and archives:
* [University of Toronto Archives Online](https://collections.library.utoronto.ca/view/utarms:root)
* [University of Toronto Map and Data Library](https://collections.library.utoronto.ca/view/mdl:root)
* [University of Toronto Music Library](https://collections.library.utoronto.ca/view/musiclibrary:root)
* [University of Toronto Richard Charles Lee Canada-Hong Kong Library](https://collections.library.utoronto.ca/view/rclc-hkl:root)
* University of St. Michael's College, including:
    * [John M. Kelly Library Special Collections](https://collections.library.utoronto.ca/view/usmc:root)
    * [University of St. Michael's College Archives](https://collections.library.utoronto.ca/view/usmc-archives:root)
* [University of Toronto Thomas Fisher Rare Book Library](https://collections.library.utoronto.ca/view/fisher:root), including:
    * [The Discovery and Early Development of Insulin](https://collections.library.utoronto.ca/view/insulin:root)
    * [Anatomia Collection: anatomical plates, 1522-1867](https://collections.library.utoronto.ca/view/anatomia:root)
    * [The Wenceslaus Hollar Collection](https://collections.library.utoronto.ca/view/hollar:root)

Legacy digital projects making use of Collections U of T include:
* Ann Komaromi's *[Project for the Study of Dissidence and Samizdat](https://collections.library.utoronto.ca/view/samizdat:root)*
* *[French](https://collections.library.utoronto.ca/view/paleography:root)* and *[Italian Paleography](https://collections.library.utoronto.ca/view/italianpaleography:root)*, supported by a grant from The Andrew W. Mellon Foundation and completed in partnership with the Newberry Library and the Walter J. Ong Centre for Digital Humanities at Saint Louis University
* Pamela Klassen's *[Story Nations](https://storynations.utoronto.ca/index.php/the-diary/the-digital-edition/manuscript-and-transcription/)*
* The University of Toronto's East Asian Library and the University of British Columbia's *[Korean Canadian Heritage Archives](https://collections.library.utoronto.ca/view/eal3:root)*

## What is Collections U of T IIIF?

IIIF (International Image Interoperability Framework) is a set of APIs and related tools created by an international community of leading cultural institutions. The IIIF community has created [a guide](https://iiif.io/guides/using_iiif_resources/) to help you get started in learning about and using IIIF.

Our ["What is IIIF?"](docs/iiif-collections-u-of-t.md) page also includes IIIF documentation specific to Collections U of T. 

## Metadata and Data Model

The Collections U of T data model is available upon request.

## Descriptive Metadata Standards
Historically, Collections U of T used [MODS](https://www.loc.gov/standards/mods/userguide/generalapp.html)-based descriptive metadata formatted as spreadsheets and then converted to xml, or MARC to MODS xml via [MarcEdit](https://marcedit.reeset.net/). Descriptive metadata is also converted to JSON in Collections U of T IIIF manifests for display purposes. 

For help with Collections U of T metadata, read the Collections U of T Metadata Instructions page. 

## Metadata Templates

* [Collections U of T metadata spreadsheet template - all fields](https://docs.google.com/spreadsheets/d/1PMtZt5CzkidIXbTBUaoi8Qg7kBU-m9RzeM-lBMORPks/edit?usp=sharing)
* [Collections U of T Metadata Profile - Element Details](https://docs.google.com/spreadsheets/d/1EidYREGS521xZKoxBN3Fl-PzkJnNJAR_zftuXXwQsZg/edit?usp=sharing)
* Collections U of T metadata mapping:
    - [MODS xml mapping](docs/xml_mods_collections_uoft_mapping.xml)
    - Wikidata properties

Ready to start adding metadata to the Collections U of T spreadsheet? [See instructions](docs/metadata_template_instructions.md).

## Other UTL Services

Collections U of T is just one of the many services offered by the University of Toronto Libraries. Here are some other services that might be of interest or helpful in your work or research:
* [Discover Archives](https://discoverarchives.library.utoronto.ca/)
* [Exhibits U of T](https://exhibits.library.utoronto.ca/)
* [TSpace](https://tspace.library.utoronto.ca/?refresh=true)
* [Find out more about the University of Toronto Libraries](https://onesearch.library.utoronto.ca/)
