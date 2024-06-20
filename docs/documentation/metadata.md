---
layout: default
title: Metadata Instructions
nav_order: 4
parent: Documentation
description: "Collections U of T Metadata Instructions"
permalink: /documentation/metadata
---

# Collections U of T Metadata Instructions

This page provides information about Collections U of T metadata and instructions to create metadata for ingest into Collections U of T.

Each Collections U of T repository is provided with a metadata spreadsheet template. The instructions below will assist collection owners in using the spreadsheet template to create metadata.

Metadata can be created for collection, book, page, and image items.

The [Collections U of T Metadata Spreadsheet Template](https://docs.google.com/spreadsheets/d/1PMtZt5CzkidIXbTBUaoi8Qg7kBU-m9RzeM-lBMORPks/edit?usp=sharing) is currently stored in Google Drive for easiest access (U of T OneDrive all-staff links have an expiry date).

**Skip to:**
* [Getting Started](https://utlib.github.io/collections-uoft/documentation/metadata#getting-started-with-collections-u-of-t-metadata)
* [Collections U of T Element Details](https://utlib.github.io/collections-uoft/documentation/metadata#collections-u-of-t-element-details)
* [PID/Filename/Identifier Tips](https://utlib.github.io/collections-uoft/documentation/metadata#pidfilenameidentifier-tips)
* [Pre-Ingest Checklist](https://utlib.github.io/collections-uoft/documentation/metadata#pre-ingest-checklist)
* [Google Sheets Tips](https://utlib.github.io/collections-uoft/documentation/metadata#google-sheets-tips)
* [MARCEdit Tips](https://utlib.github.io/collections-uoft/documentation/metadata#marcedit-tips)
* [OpenRefine Tips](https://utlib.github.io/collections-uoft/documentation/metadata#openrefine-tips)
* [How do I update Metadata Labels on Collections U of T for my collection?](https://utlib.github.io/collections-uoft/documentation/metadata#how-do-i-alter-the-metadata-labels-that-publicly-display-for-my-collection-on-collections-u-of-t)

## Getting Started with Collections U of T Metadata

First, if you have existing MARC records to work with you can scroll to [MARCEdit Tips](metadata_template_instructions.md#marcedit-tips) to read more about converting MARC records into a Collections U of T spreadsheet.

If you have an existing database of metadata and would like help exporting it, email [digitalinitiatives@library.utoronto.ca](mailto:digitalinitiatives@library.utoronto.ca).

If you are creating your metadata spreadsheet from scratch, start by downloading or making your own Google Drive copy of the [Collections U of T metadata spreadsheet template - all fields](https://docs.google.com/spreadsheets/d/1PMtZt5CzkidIXbTBUaoi8Qg7kBU-m9RzeM-lBMORPks/edit?usp=sharing).

After copying or downloading, rename the spreadsheet with the PID or title of your collection. It can be helpful to have **one spreadsheet per collection**. 

If you wish, you can store this new spreadsheet copy on your U of T staff OneDrive or continue working in Google Sheets.

## Collections U of T Element Details

After copying the spreadsheet, begin filling in the spreadsheet for your collection(s) based on the [Collections U of T Element Details](https://docs.google.com/spreadsheets/d/1EidYREGS521xZKoxBN3Fl-PzkJnNJAR_zftuXXwQsZg/edit#gid=0). If you have any questions about any of the elements, contact Collections U of T staff for support.

### PID/Filename/Identifier Tips

See [slide deck](https://docs.google.com/presentation/d/1W2PWTBE22rj15h7FbVDgAv5DIfg33rnn-1vLQZ_qgDw/edit?usp=sharing) on PID/Filename/Identifier tips. 

## Pre-Ingest Checklist

* Check that PIDs are correctly formatted (see above)
* Check for entity codes - i.e. *$amp;* in place of *&*. Note that you *are* able to represent the actual special character in the spreadsheet metadata - i.e. *&*. The ingest script accepts special characters - so long as spreadsheets are saved with UTF-8 encoding
* Check each column you have filled in against the [Element Details](https://docs.google.com/spreadsheets/d/1EidYREGS521xZKoxBN3Fl-PzkJnNJAR_zftuXXwQsZg/edit#gid=0) Input Guidelines to ensure you are following Collections U of T metadata rules
* Check for spelling errors
* Check for duplicate words or terms
* Check that the file paths to your digital images are correct

## Google Sheets Tips

The Google Sheet template is formatted to assist you with entering data for ingest into Collections. The instructions below can help you if you would like to add additional formatting to the spreadsheet.

### Fill down

Double click the blue box in the bottom right of the cell to fill a value down.

![Google sheets - fill down](../img/sheets_fill_down.png)


### Create Dropdown

1. Open a spreadsheet in [Google Sheets](https://docs.google.com/spreadsheets/).
2. Select the cell or cells where you want to create a drop-down list.
3. Click Data  Data validation.
4. Next to "Criteria," choose an option:
    * List from a range: Choose the cells that will be included in the list.
    * List of items: Enter items, separated by commas and no spaces.
5. The cells will have a Down arrow. To remove the arrow, uncheck "Show dropdown list in cell."
6. If you enter data in a cell that doesn’t match an item on the list, you’ll see a warning. If you want people to only enter items from the list, choose "Reject input" next to "On invalid data."
7. Click Save. The cells will show a drop-down list. To change the color of a cell based on the option selected, use conditional formatting. 

### Split Text to Columns

1. In Sheets, select the column that contains the data that you want to split.
2. Click DataSplit text to columns.
3. If you want Sheets to detect when a file is formatted using fixed-width, select Detect automatically.

![Google sheets - drown down](../img/sheets_drop_down.png)

## MARCEdit Tips

*To be added.*

## OpenRefine Tips

*To be added.*

Instructions on this page for OpenRefine will be specific to steps that could help you with Collections U of T metadata spreadsheets. You can also refer to the [OpenRefine documentation](https://openrefine.org/docs) or check out U of T's [Map and Data Library OpenRefine tutorials](https://mdl.library.utoronto.ca/tools/openrefine).

Note that if you are working in Google Sheets on your Collections U of T metadata spreadsheet, you can load the data into OpenRefine directly from Google Sheets by following [these instructions](https://openrefine.org/docs/manual/starting#google-data). Make sure the spreadsheet is a Google Sheet and not an .xlsx document stored in your Google Drive. 

## How do I alter the metadata labels that publicly display for my collection on Collections U of T?

All collections share the same metadata schema (see above documentation). It is possible to submit a request to change the labels of the metadata for your repository. To change the display labels of metadata for your repository's collection(s) please [email Collections U of T ITS staff](mailto:digitalinitiatives@library.utoronto.ca) to request a consultation about modifying metadata labels. If it is possible to accommodate your requested changes, ITS will modify [internal metadata mapping documents](https://git.library.utoronto.ca/utl-its/digital-collections/collections-lookup/-/tree/main/src/config/metadataMapping?ref_type=heads). Note that these internal metadata display documents also control the labels in your repository's IIIF manifests.

For values in the Creator / Contributor field the role term you select in the *creator_contributor_role* column will become the metadata label for the name entered in the *creator_contributor* column. If you enter "none", or do not enter anything into the role term column, then the default display label will be Creator / Contributor. Here is an example of names entered with "none" as well as "bookplate designer" for manuscript [fisher2:11952](https://collections.library.utoronto.ca/view/fisher2:11952).

![Creator or Contributor role terms become labels per name](../img/creator_contributor_role_terms.jpg)


