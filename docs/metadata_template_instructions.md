# Using the Collections U of T Metadata Spreadsheet Template

## About This Page

This page provides instructions and tips on using the Collections U of T Metadata Spreadsheet Template.

The [Collections U of T Metadata Spreadsheet Template](https://docs.google.com/spreadsheets/d/1PMtZt5CzkidIXbTBUaoi8Qg7kBU-m9RzeM-lBMORPks/edit?usp=sharing
) is currently stored in Google Drive for easiest access (U of T OneDrive all-staff links expire).

**Skip to:**
* [Getting Started](metadata_template_instructions.md#getting-started-with-collections-u-of-t-metadata)
* [Collections U of T Element Details](metadata_template_instructions.md#collections-u-of-t-element-details)
* [PID/Filename/Identifier Tips](metadata_template_instructions.md#pidfilenameidentifier-tips)
* [Pre-Ingest Checklist](metadata_template_instructions.md#pre-ingest-checklist)
* [Google Sheets Tips](metadata_template_instructions.md#google-sheets-tips)
* [MARCEdit Tips](metadata_template_instructions.md#marcedit-tips)
* [OpenRefine Tips](metadata_template_instructions.md#openrefine-tips)

## Getting Started with Collections U of T Metadata

To start, download or make your own Google Drive copy of the spreadsheet template. 
Name the spreadsheet with the PID of your collection.
If you wish, you can store this new spreadsheet copy on your staff OneDrive if you wish, or continue working in Google Sheets.

## Collections U of T Element Details

After copying the spreadsheet, begin filling in the spreadsheet for your collection(s) based on the [Collections U of T Element Details](https://docs.google.com/spreadsheets/d/1EidYREGS521xZKoxBN3Fl-PzkJnNJAR_zftuXXwQsZg/edit#gid=0 - these details are draft until New Collections is launched, but should not change much as we move into the new system.
). If you have any questions about any of the elements, contact Collections U of T staff for support.

### PID/Filename/Identifier Tips

See [slide deck](https://docs.google.com/presentation/d/1W2PWTBE22rj15h7FbVDgAv5DIfg33rnn-1vLQZ_qgDw/edit#slide=id.ge72446e2fa_0_90) on PID/Filename/Identifier tips. 

## Pre-Ingest Checklist

*This list to be filled in with additional instructions.*

* Check for entity codes
* Instead of entity codes, you are able to represent the actual special character in spreadsheet metadata. The ingest script accepts special characters - so long as spreadsheets are saved with UTF-8 encoding
* Check each column against the Element Details rules
* Check for spelling
* Check for duplicates
* More to add...

## Google Sheets Tips

### Fill down

Double click the blue box in the bottom right of the cell to fill a value down.

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

## MARCEdit Tips

*To be added.*

## OpenRefine Tips

*To be added.*
