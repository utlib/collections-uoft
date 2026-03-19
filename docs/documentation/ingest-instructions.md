---
layout: default
title: Ingest Instructions
nav_order: 3
parent: Documentation
description: "Ingest Instructions"
permalink: /documentation/ingest-instructions
---

# Ingest instructions

{: .note }
> ***From July 2024 - Spring 2026 ingests must be facilitated by ITS. Follow the instructions below and email [digitalinitiatives@library.utoronto.ca](mailto:digitalinitiatives@library.utoronto.ca) to ingest your content.***


## Before ingesting collections and items into Collections U of T...

* You must already be a [participating repository](https://utlib.github.io/collections-uoft/documentation/adding-new-collections)
* Clear all copyright, privacy, and rights considerations for the collection before submitting the images to Collections U of T for online public access and review all [service policies](https://utlib.github.io/collections-uoft/#collections-u-of-t-policies)
* Confirm that all collections/items are intended for public access in perpetuity
* Consult Collections U of T [Metadata Instructions](https://utlib.github.io/collections-uoft/documentation/metadata) in full
* Review this page in full
* Ensure PIDs in your metadata spreadsheet are correct - in most cases, PIDs cannot be changed after ingest
* Ensure image files are correctly named to match PIDs in your metadata spreadsheet
* Ensure image files are the final, edited copies that you would like to make public

## To add a new collection to your repository:

[Contact ITS](mailto:digitalinitiatives@library.utoronto.ca) with the following details:

1. Title of the collection
2. Brief description for the collection (this will display publicly on the collection's /view/ page and be included in the collection's metadata)
3. PID of collection
4. Related catalog record catkey, permalink, or any “Part of” links - i.e. corresponding Discover Archives finding aid or link to external collection website
5. Call number, if any
6. Path to the completed and validated [metadata spreadsheet](https://utlib.github.io/collections-uoft/documentation/metadata) for the collection's metadata and any child items (if you are including child items, indicate whether the viewing direction of the images should be right to left)
7. Path to the directory where the images are stored (you must ensure image filenames match metadata spreadsheet filenames)
8. Deadline for ingest to help ITS prioritize and schedule the work

## To add new items to an existing collection in your repository:

[Contact ITS](mailto:digitalinitiatives@library.utoronto.ca) with the following details:

1. PID of the collection you are adding  the item(s) to (this PID should also be present in the `member_of` field in your metadata spreadsheet for any book or image items)
2. Path to the completed and validated [metadata spreadsheet](https://utlib.github.io/collections-uoft/documentation/metadata) for the items' metadata
3. Whether the viewing direction of the images should be right to left
4. Path to the directory where the images are stored (you must ensure image filenames match metadata spreadsheet filenames)
5. Deadline for ingest to help ITS prioritize and schedule the work

Consult with the Collections U of T team if you need to ingest OCR text for your image files. Instructions for using transcription tools with Collections U of T IIIF manifests can also be found [here](https://utlib.github.io/collections-uoft/documentation/transcriptions-with-iiif).

## Collections U of T Deletion Policy
_Last updated: March 19, 2026_

**Collection deletion is disabled** - deleting collections is currently restricted to system administrators only. To request deletion of a collection, please contact [digitalinitiatives@library.utoronto.ca](mailto:digitalinitiatives@library.utoronto.ca).


### Once items are published please avoid deleting published Image, Book, or Page items and avoid replacing or deleting image files

**Image, Book, Page item deletion _is_ enabled** - while deletion of Image, Book, and Page items _is_ enabled, it should only be used with caution and for exceptional circumstances. _Published items_ in Collections U of T should only be the final, reviewed images and metadata ready for publication. Remember that Collections U of T publishes images as _data_ - this data is represented as a [IIIF Manifest](https://iiif.io/guides/using_iiif_resources/). If you delete an Image, Book, or Page, or update an image in an item published to Collections U of T, the item's IIIF Manifest will _also_ be deleted or permanently altered. Therefore, updating image files in a published item in Collections U of T may cause unintentional broken links or corrupted data for end users who make use of the item's IIIF Manifest. This may unintentionally impact an end user's research output. Please only publish final, edited copies of digital images to Collections U of T. If you need to conduct test ingests, use the test instance of the Collections U of T Admin UI. 

Note that Collections U of T does not yet have the [IIIF Change Discovery API enabled](https://iiif.io/api/discovery/1.0). 


### Can I ingest A/V file formats into Collections U of T?

No, you cannot ingest A/V file formats into Collections U of T. At this time, A/V file formats can be stored in UTL's [MyMedia service](https://mymedia.library.utoronto.ca/). Once stored in MyMedia, you can use the MyMedia embed link to add the videos to basic pages for your collection. You can also ingest metadata for these files to surface in Collections U of T search. For more information about how to handle A/V digital collections, [contact us](mailto:digitalinitiatives@library.utoronto.ca). See other format support information [here](https://utlib.github.io/collections-uoft/#format-support). 

**This page will be updated with self-ingest instructions when the new Collections U of T administrator user interface is launched after Spring 2026.**
