# Collections U Of T

## About this page
This documentation is intended for collection owners, end users, and U of T staff or open technology community members interested in Collections U of T.

As of March 2023 this documentation status is *draft* and has not been approved by UTL Senior Staff.

**Skip to:**
* [About Collections U of T](README.md#about-collections-u-of-t)
* Documentation for collection owners
    * Requesting a top-level collection
    * [Metadata instructions](docs/metadata_template_instructions.md)
    * Ingest instructions
* Documentation for getting started with Collections U of T
    * Searching
    * Using IIIF
        * Downloading
        * Embedding

## About Collections U of T
[Collections U of T](https://collections.library.utoronto.ca) is the  University of Toronto Libraries' repository for digitized special collections and archives. It provides open access to these digital collections through the [International Image Interoperability Framework (IIIF)](https://iiif.io/) and standard metadata formats.

Collections U of T provides U of T staff:

1. Collection management and digital object storage for university special collections and archives image collections
2. Indexing for digital object metadata
3. Search and discovery for collections and digital objects
4. User management and authentication (CRUD for collections and digital objects)
5. Statistics for collections and digital objects

Collections U of T is not:
* A digitization service
* A digital exhibit service
* A digital preservation service
* Open to anyone - digital collections must be *assessed* prior to inclusion. Because the service is intended for providing long term discovery and display of access copies of digital collections, the digital objects must belong to a UTL department or archives and be assessed by a UTL staff collection owner prior to inclusion. UTL collection owners are responsible for assessing digital objects for accessibility, privacy and copyright considerations, as well as staffing capacity to support the care and maintenance of the digital collection over time. 

UTL staff can request a consultation for Collections U of T support at [digitalinitiatives@library.utoronto.ca](mailto:digitalinitiatives@library.utoronto.ca).

Researchers, students, and faculty can read documentation provided to learn how to use the system. Please send any questions or feedback to [digitalinitiatives@library.utoronto.ca](mailto:digitalinitiatives@library.utoronto.ca).

### List of Top-Level Collections in Collections U of T

As of March 2023, Collections U of T holds selected digital objects for the following libraries and archives:
* University of Toronto Archives Online
* University of Toronto Map and Data Library
* University of Toronto Music Library
* University of Toronto Richard Charles Lee Canada-Hong Kong Library
* * University of St. Michael's College, including:
    * John M. Kelly Library Special Collections
    * University of St. Michael's College Archives
* University of Toronto Thomas Fisher Rare Book Library, including:
    * The Discovery and Early Development of Insulin
    * Anatomia Collection: anatomical plates, 1522-1867
    * The Wenceslaus Hollar Collection

Legacy digital projects making use of Collections U of T include:
* Ann Komaromi's *Project for the Study of Dissidence and Samizdat*
* *French* and *Italian Paleography*, supported by a grant from The Andrew W. Mellon Foundation and completed in partnership with the Newberry Library and the Walter J. Ong Centre for Digital Humanities at Saint Louis University
* Pamela Klassen's *[Story Nations](https://storynations.utoronto.ca/index.php/the-diary/the-digital-edition/manuscript-and-transcription/)*
* The University of Toronto's East Asian Library and the University of British Columbia's *Korean Canadian Heritage Archives*

## What is Collections U of T IIIF?

IIIF (International Image Interoperability Framework) is a set of APIs and related tools created by an international community of leading cultural institutions. The IIIF community has created documentation to help you learn how to use the IIIF APIs, how to use the IIIF Mirador viewer, and how to find other IIIF digitized collections from cultural heritage institutions across the globe. Below you will find additional IIIF documentation specific to Collections U of T and the University of Toronto's IIIF digital collections.

Read more about IIIF in Collections U of T.

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
