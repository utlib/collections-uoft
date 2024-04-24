---
layout: default
title: What is IIIF? (for staff)
nav_order: 6
parent: Documentation
description: "What is IIIF? (for staff)"
permalink: /documentation/iiif-collections
---

# What is IIIF? (for staff)

> **DRAFT: further edits and instructions forthcoming.**

[IIIF (International Image Interoperability Framework)](http://iiif.io/) is a set of APIs and related tools created by an international community of leading cultural institutions. The IIIF community has created documentation to help you learn how to use the [IIIF APIs](https://iiif.io/get-started/how-iiif-works/), how to use the [IIIF Mirador viewer](https://iiif.io/guides/using_iiif_resources/#mirador), and how to [find other IIIF digitized collections](https://iiif.io/guides/finding_resources/) from cultural heritage institutions across the globe. 

**Public documentation about Collections U of T and IIIF is available at [https://collections-beta.library.utoronto.ca/explore/getting_started](https://collections-beta.library.utoronto.ca/explore/getting_started).**

Staff documentation about IIIF and Collections U of T is forthcoming.

## Using external IIIF services - Internet Archive

UTL makes use of the Internet Archive (IA) to publish digital collections. The IA is also [IIIF-enabled](https://github.com/internetarchive/iiif). Collection owners may consider the following when deciding if they should use Collections U of T versus the Internet Archive:
* If your UTL department is acquiring archives and special collections for digitization and unrestricted public access please [email us](mailto:digitalinitiatives@library.utoronto.ca) to discuss if your context fits the [Collections U of T policies](https://utlib.github.io/collections-uoft/#about-collections-u-of-t).
* If your UTL department's context fits within the Collections U of T policies and you anticipate reuse of digital objects via IIIF tools then Collections U of T IIIF is the recommended service
* Remember that Collections U of T IIIF manifests and image URLs are published with the goal of providing access and capacity for reuse in **perpetuity**
* Metadata fields in Collections U of T IIIF manifest are customizable according to the repository owner's specifications (within the constraints of the Collections U of T metadata profile and index)
* Collections U of T digital objects are published alongside all of UTL's other  digital collections within the [UTL top-level IIIF collection manifest](https://iiif.library.utoronto.ca/presentation/v2/collections)

## Embedding IIIF

IIIF embeds via Collections U of T can use the following parameters:

* manifestId: Allow multiple entries and render them up to four in sequence - e.g. manifestId=MANIFEST_ID1&manifestId=MANIFEST_ID2
* canvasId: Allow multiple entries and it pairs with a matching `manifestId` up to four in sequence. e.g. manifestId=MANIFEST_ID1&canvasId=CANVAS_ID1
* workspaceControlPanel=true - Allows the Mirador 3.x Workspace functionality within the embed
* thumbnailNavigationDisplay=true - Enables thumbnail display in embed (default is true)

These embed features are reflected on [the /explore/ pages' IIIF embeds](https://utlib.github.io/collections-uoft/documentation/add-simple-page) as well. 

If your department would like more information or training about IIIF for your staff please [email us](mailto:digitalinitiatives@library.utoronto.ca) to plan training sessions or support with IIIF / Collections U of T use for faculty and students after Summer 2025.
