---
layout: default
title: History of Collections U of T
nav_order: 9
parent: Documentation
description: "History of Collections U of T"
permalink: /documentation/history
---

# History of Collections U of T



[Collections U of T](https://collections.library.utoronto.ca/) began as a project in the University of Toronto Libraries Information Technology Services department in 2013 in response to staff requests to make digitized special collections available online within a repository (presentation, search, preservation) ecosystem. The history of how the Collections U of T service evolved can be found in the _Introduction_ of ["Where Do We Go From Here: A Review of Technology Solutions for Providing Access to Digital Collections"](https://journal.code4lib.org/articles/15000) in _Code4Lib Journal_ issue 47 from 2020.

This article was published by the ITS team in anticipation of [Islandora 7](https://wiki.lyrasis.org/display/ISLANDORA/Start) / Drupal 7 end of support, which was originally scheduled for November 2021. In advance of this date, ITS initiated a technology review in 2019 to look at technology platform and infrastructure options to support the Collections U of T service, improve its efficiency and scalability, and also simplify its usability, maintenance, and workflows. 

Other internal migration goals for the service included:
* Enable end user ability to navigate and search _across_ U of T digitized special collections
* Improve end user's ability to quickly browse digitized images in any collection 
* Re-implement self-ingest for collection owners 
* Normalize metadata across collections
* Reduce Collections U of T maintenance hours for UTL ITS staff
* Simplify Collections U of T technology infrastructure (where possible: share infrastructure with other existing ITS, and Scholars Portal, services)
* Avoid replicating the web content creation/editing functionality available to staff through other web services
* Enhance search engine optimization (SEO) for digital collections
* Remain standards-based for relevant digital image and digitized special collections metadata standards
* Improve UTL public documentation of the standards used in Collections U of T and our local practices
* Incorporate web accessibility considerations into every design decision
* Remain flexible
* Consider [Linked Open Usable Data (LOUD) principles](https://www.slideshare.net/slideshow/publishing-linked-open-usable-data/89234543) when relevant to service policy and infrastructure decisions. Note: though linked data functionality was explicitly out of scope for the migration project, it remains of interest for future. The indexing tool used by the New Collections U of T Platform, MarkLogic, is [linked data ready](https://www.progress.com/resources/papers/marklogic-semantics-whitepaper).
* Consider integration with external tools such as hosted transcriptions via From The Page or external IIIF manifests from the Internet Archive

The research process and migration pathway decision to move the service away from the Islandora platform is documented in the [2020 Code4Lib article](https://journal.code4lib.org/articles/15000). However, Drupal 7 end of life was extended multiple times from 2020 to 2023. The final end of life date for Drupal 7 was finally communicated in June of 2023 - Drupal would reach its final end of support date on [January 5th of 2025](https://www.drupal.org/psa-2023-06-07). 

On May 21st, 2024, ITS soft launched its new homegrown New Collections U of T Platform comprised of "pluggable pieces" - a mix of new development alongside reusing existing UTL ITS technology infrastructure from other services as well as infrastructure provided by [Scholars Portal](https://ocul.on.ca/scholars-portal) - to deliver the Collections U of T service. The New Collections U of T Platform's infrastructure diagram is embedded below. It is also viewable in the UTL ITS [Miro](https://miro.com/app/board/uXjVM_vBtBc=/?share_link_id=757884216988). 

<iframe width="768" height="432" src="https://miro.com/app/live-embed/uXjVM_vBtBc=/?moveToViewport=-1663,2087,2432,1227&embedId=718971289571" frameborder="0" scrolling="no" allow="fullscreen; clipboard-read; clipboard-write" allowfullscreen></iframe>

The Islandora 7 multi-sites were redirected to the New Collections U of T Platform at the end of June 2024. All permalinks per digital object redirect to the New Platform. The old Islandora 7 multi-sites are each web archived on UTL's [Archive-It account](https://archive-it.org/collections/6473). The initial migration work completed in 2024 only marked the soft launch of New Collections U of T. Additional information about the 2024 soft launch can be found below. 

ITS continues to work on the Platform, gather staff and user feedback, and make iterative improvements, guided by our initial migration goals as well as the evolving requirements of service users and changes in technology.


If you have any questions, please email [Collections U of T support staff](mailto:digitalinitiatives@library.utoronto.ca). 

## Note: Collections U of T and LLM / generative AI features

As of 2026, the Collections U of T Platform **does not** include LLM or generative AI features in its public-facing systems. AI-assisted tools are sometimes used by ITS developer staff to support software development and data review. Some Collections U of T service documentation makes use of the [Scribe tool](https://scribe.com/) but does not make use of Scribe's Workflow AI features. As stated in the [Collections U of T service policies](https://utlib.github.io/collections-uoft/#collections-u-of-t-policies), Collection owners are responsible for review and approval of any content and metadata ingested into the Platform, including considerations around use of AI-assisted tools in individual work flows as well as AI-assistance disclosures.


## Additional information about the New Collections U of T 2024 soft launch
You can view the [2024 Migration Guide](https://utlib.github.io/collections-uoft/documentation/2024-migration-guide) for more information about changes from Islandora 7 to the new homegrown Collections U of T Platform. You can also visit the Collections U of T [help pages](https://collections.library.utoronto.ca/explore/help) to learn how to search and reuse digital objects in new platform. 

Thank you to the amazing staff who have contributed so much time and work into the Collections U of T service for well over a decade, some of whom are named below. Thank you all!

**Primary Collections U of T ITS Service Staff:**
* Service contact: [digitalinitiatives@library.utoronto.ca](digitalinitiatives@library.utoronto.ca)
* Kelli Babcock, service manager
* Sunny Lee, lead developer

**Thank you to the amazing 2023-2024 ITS development team:**
* Andy Foster
* Bilal Khalid
* Dickson Law
* Jana Rajakumar
* Jarvis Tse
* Andy Wagner

**Thank you OLRC and MarkLogic Scholars Portal staff for the development support:**
* Bikramjit Singh Channa
* Jayanthy Chengan
* Julie Shi
* Harpinder Singh

**Thank you to ITS and Scholars Portal staff, past and present, for planning and development input on the New Collections Platform:**
* Imran Asghar
* Leslie Barnes
* Steve Baroti
* Gordon Belray
* Chris Crebolder
* Kate Davis
* Rachel Di Cresce
* Marcel Fortin
* Julia Gilmore
* Lillian Hogendoorn
* Grant Hurley
* Shibo Liu
* Steve Marks
* Sian Meikle
* Hitesh Prabhakar
* Graham Stewart
* Amaz Taufique
* Monica Ung
* Jess Whyte

**Thank you to current and past ITS students for helping with metadata normalization, conducting research, assisting in migrating content, creating documentation, and providing other migration support over the years:**
* Isobel Carnegie
* Adam Cavanaugh
* Jasmine Lefresne
* Fahma Mohamed
* Alexandra Wong

**Thank you to all of the U of T Collection Owners plus other U of T staff, past and present, for your advice, support, championing, feedback, and eventual testing for the New Collections soft launch:**
* Larry Alford
* Daniela Ansovini
* Jessica Barr
* Susan Bond
* Liz Carroll
* Alexandra Carter
* May Chan
* David Fernandez
* Nick Field
* Tanis Franco
* Marnee Gamble
* Kyla Jemison
* Hana Kim
* Tys Klumpenhouwer
* Maria Lau
* Loryl MacDonald
* Mariya Maistrovskaya
* James Mason
* Kaitlin Newson
* Jordan Pedersen
* Tim Perry
* Kim Pham
* Natalya Rattan
* Liz Ridolfo
* Simon Rogers
* Nadav Sharon
* Becky Shaw
* John Shoesmith
* Emily Sommers - additional thank you for setting up these Github pages
* Karen Suurtamm
* Leanne Trimble
* Helen Tang
* Teresa Wong
* Nich Worby - additional thank you for your wealth of Archive-It knowledge and assistance
* Nicole Yang

Lastly, thanks to many folks from the Canadian, U.S., and international archives, digital collections, IIIF, Islandora, and open technology communities for sharing your work, publishing your documentation, and answering questions.

