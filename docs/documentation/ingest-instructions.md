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
> ***The Collections U of T administrator interface is currently under development.<br />From July 2024 - Summer 2025 ingests have to be facilitated by ITS.Follow the instructions below and email [digitalinitiatives@library.utoronto.ca](mailto:digitalinitiatives@library.utoronto.ca) to ingest your content.<br />
<br />
> You must already be a [participating repository](https://utlib.github.io/collections-uoft/documentation/adding-new-collections) to ingest collections and images into Collections U of T.<br />
<br />
> Please also be aware that the Collections U of T service is operating in maintenance mode with reduced staff capacity in 2024-2025.***


## Before ingesting collections and items into Collections U of T...

* Clear all copyright, privacy, and rights considerations for the collection before submitting the images to Collections U of T for online public access and review all [service policies](https://utlib.github.io/collections-uoft/#collections-u-of-t-policies)
* Consult Collections U of T [Metadata Instructions](https://utlib.github.io/collections-uoft/documentation/metadata) in full
* Review this page in full
* Ensure PIDs in your metadata spreadsheet are correct - in most cases, PIDs cannot be changed after ingest
* Ensure image files are correctly named to match PIDs in your metadata spreadsheet
* Ensure image files are the final, edited copies that you would like to make public

## To add a new collection to your repository:

[Contact ITS](mailto:digitalinitiatives@library.utoronto.ca) with the following details:

1. Title of the collection
2. Brief description to the collection (to be included in the collection's metadata description)
3. PID of collection
4. Related catalog record catkey, permalink, or any “Part of” links - i.e. corresponding Discover Archives finding aid or link to external collection website
5. Call number, if any
6. Path to the completed and validated [metadata spreadsheet](https://utlib.github.io/collections-uoft/documentation/metadata) for the collection's metadata and any child items
7. Path to the directory where the images are stored (you must ensure image filenames match metadata spreadsheet filenames)
8. Deadline for ingest to help ITS prioritize and schedule the work

## To add new items to an existing collection in your repository:

[Contact ITS](mailto:digitalinitiatives@library.utoronto.ca) with the following details:

1. PID of the collection you are adding  the item(s) to (this PID should also be present in the `member_of` field in your metadata spreadsheet for any book or image items)
2. Path to the completed and validated [metadata spreadsheet](https://utlib.github.io/collections-uoft/documentation/metadata) for the items' metadata
3. Whether the viewing direction of the images should be right to left
4. Path to the directory where the images are stored (you must ensure image filenames match metadata spreadsheet filenames)
5. Deadline for ingest to help us prioritize and schedule the work

Consult with the Collections U of T team if you need to ingest OCR text for your image files. Instructions for using transcription tools with Collections U of T IIIF manifests can also be found [here](https://utlib.github.io/collections-uoft/documentation/transcriptions-with-iiif).

### Beware updating image files within an item published in Collections U of T

Remember that Collections U of T publishes images as _data_ - this data is represented as a [IIIF Manifest](https://iiif.io/guides/using_iiif_resources/). If you update an image in your digital object, the IIIF Manifest is *also* altered. Therefore, updating image files in an item published in Collections U of T may cause unintentional issues for end users making use of the item's IIIF Manifest. 

Be aware that changing the images in your digital objects after they have been published for an extended period of time may impact a user's research output. Please only update images after you have published them with extreme caution. Ideally, please only publish final, edited copies of digital images to Collections U of T. 


### Can I ingest A/V file formats into Collections U of T?

No, you cannot ingest A/V file formats into Collections U of T. At this time, A/V file formats can be stored in UTL's [MyMedia service](https://mymedia.library.utoronto.ca/). Once stored in MyMedia, you can use the MyMedia embed link to add the videos to basic pages for your collection. You can also ingest metadata for these files to surface in Collections U of T search. For more information about how to handle A/V digital collections, [contact us](mailto:digitalinitiatives@library.utoronto.ca).

**This page will be updated with self-ingest instructions when the new Collections U of T administrator user interface is launched in Fall 2025.**
