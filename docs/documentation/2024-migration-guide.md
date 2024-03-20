---
layout: default
title: 2024 Migration Guide
nav_order: 1
parent: Documentation
description: "2024 Migration Guide"
permalink: /documentation/2024-migration-guide
---

# 2024 Collections U of T Migration Guide


* [2024 Collections U of T Migration Guide](#2024-collections-u-of-t-migration-guide)
* [Important Migration Dates](#important-migration-dates)
* ["New" Collections U of T Training Kit](#new-collections-u-of-t-training-kit)
* [Migration FAQ](#migration-faq)

**This guide is provides UTL staff with instructions and FAQs about the Collections U of T migration from Islandora 7 to the new UTL-homegrown "New Collections" application in Spring 2024.**


It is with much excitement that the University of Toronto Libraries Information Technology Services announces the March 2024 beta launch of its new website and application for the Collections U of T service. This migration is the result of a multi-year project by ITS staff to move the Collections U of T service off of Islandora 7 (Drupal 7) as Drupal 7 reaches [end of support on January 5, 2025](https://www.drupal.org/about/drupal-7/d7eol/partners?gad_source=1&gclid=CjwKCAiA_tuuBhAUEiwAvxkgTpcqWPPQRldzo2woWqXjQGdC9r5TTSbAuycGH45nlNF-2FpSv2Iv9xoCsB8QAvD_BwE).

**You can access the new Collections U of T beta website at [https://collections-beta.library.utoronto.ca/](https://collections-beta.library.utoronto.ca/).**

**The beta site is:**
* not public; it is only accessible on UTL VPN
  * _use VPN to access the beta site if you are off campus or not on a UTL ITS managed workstation_
* available for testing purposes _only_
  * _please remember the site is still in beta and under active development[1]_
* internal to U of T staff
  * _none of the beta site URLs are publicly accessible so please do not share the beta URLs with students, faculty, researchers, or the public_
* not impacting the Collections U of T Islandora 7 sites
  * _the Islandora sites remain publicly accessible and running concurrently alongside the new Collections U of T beta site_

  [1] Remaining beta development includes:
  * PID validation against Islandora RELS-EXT - you may notice that not all digital object counts match your Islandora site
  * adding thumbnails to all collection-level objects - you may notice some collection objects on /view/ pages have a grey folder icon; we are adding these
  * custom search facet labels on repository search pages - you may notice your custom search labels on your repository's search page are not yet implemented; these require additional development and are coming
  * finishing help pages and staff documentation
 

# Important Migration Dates

If you are a Collections U of T collection owner please complete the following checklist:

1. By March 29: refer to your "New Collections beta launch" email - go to the new beta website and find your collection from the list on the homepage
2. By March 29: review your collection against your old Islandora 7 website
3. By March 29: review this 2024 Migration Guide page
4. By April 2: check that you can access the [Collections U of T teams channel](https://teams.microsoft.com/l/team/19%3a6Gi_nOUv02tuKON6QI8HeJcsTDw5PEhxhbJ_qPafHa41%40thread.tacv2/conversations?groupId=2151c2c7-2063-412d-8ebf-de2c9f809003&tenantId=78aac226-2f03-4b4d-9037-b46d56c55210) for asynchronous support and migration updates
5. By April 2: [contact UTL ITS]((mailto:digitalinitiatives@library.utoronto.ca)) with any feedback, questions or bugs to report about the new Collections U of T beta website before the New Collections soft launch date on April 16, 2024

> ***The Collections U of T beta site's public soft launch is scheduled for Tuesday, April 16, 2024.***


## All Migration Dates

* March 21, 2024: collections-beta site shared with collection owners (internal U of T IP access only)
* April 2, 2024: collection owner deadline to submit feedback about collections-beta
* April 2-15, 2024: feedback reviewed by ITS and selected improvements implemented
* **April 16, 2024: collections-beta goes live** on collections.library.utoronto.ca
  * this is the New Collections public soft launch date!
  * facilitated ingests can resume into collections.library.utoronto.ca
  * the Islandora sites will remain live and publicly accessible but no new items will be ingested into Islandora sites
* By end of June 2024: ITS will work with collection owners to schedule shut down dates for each Islandora site. Islandora site URLs will be re-directed to the relevant collection URL on New Collections at the collections.library.utoronto.ca URLs. Collections U of T permalink /view/ URLs remain the same. For example, https://collections.library.utoronto.ca/view/utarmsIB:2006-23-38MS remains the permalink URL for this photograph of Harold Innis in the UTARMS collection. 
* July 2024 - Summer 2025: there will be reduced Collections U of T service management capacity due to staff leaves
* Fall 2025: ITS will roll out New Collections administrator user interface and collection owners will be able to self-ingest


# "New" Collections U of T Training Kit
--------
(To be added - this will be discussed during scheduled meetings with collection owners)      


# Migration FAQ
--------

**1) Can I resume ingesting new collections and images into the new Collections U of T beta site?**

_Yes - if you have an existing repository page in Collections U of T you can add new collections and items at any time. UTL ITS will support facilitated ingest throughout 2024 as we continue monitoring the performance of the new Collections U of T application. Please [email ITS](mailto:digitalinitiatives@library.utoronto.ca) if you need ingest and editing support. Facilitated ingest instructions can be found on the [Ingest Instructions](https://utlib.github.io/collections-uoft/documentation/ingest-instructions) page._

_Please consider that the Collections U of T service is operating at reduced capacity until Summer 2025 due to ITS staffing._

**2) Can I edit metadata again?**

_Yes but you need to [email ITS](mailto:digitalinitiatives@library.utoronto.ca) for support. Let us know what you need help editing and we will pass along instructions._

**3) Is there an administrator login for me to login to New Collections to edit and upload digital images into the new Collections U of T beta site?**

_No. See above. The administration login into new Collections U of T will be available in *2025*. UTL ITS is continuing to work on the Collections U of T administrator interface. 2024 will be devoted to monitoring new Collections U of T performance and indexing. ITS will support collection owners with facilitated ingests. The new Collections U of T administrator interface is expected to launch in late *2025*._ 

**4) I never had a Collections U of T repository on Islandora. Can I add a new repository to the new Collections U of T website for my UTL library/archive?**

_Due to service capacity from July 1, 2024 to Summer 2025 we will not be adding new repositories into Collections U of T. You can [email us](mailto:digitalinitiatives@library.utoronto.ca) to [request a new repository](https://utlib.github.io/collections-uoft/documentation/adding-new-collections) be added and we will review these requests and onboard new repositories in 2025 for you to begin using Collections U of T._

**5) When will the new Collections U of T website be available to the public (outside of U of T networks)?**    

_April 16, 2024._

_The [collections.library.utoronto.ca/*](https://collections.library.utoronto.ca/) URL will point to the new Collections U of T website on April 16, 2024. This scheduled date may change if any issues arise on the beta site._

**6) Should I still use the collections.library.utoronto.ca permalinks to collections and images?**

_Yes. The collections.library.utoronto.ca URL is still the correct permalink to collections and images. **Do not publicly promote or share the -beta URLs.** The collections-beta.library.utoronto.ca URL will be replaced with collections.library.utoronto.ca when the new Collections U of T website is publicly launched._

**7) When will my Islandora 7 website be taken offline?**

_Late Spring 2024 - we will communicate the exact date with collection owners as capacity allows (for both ITS and collection owners). Copies of the Islandora 7 sites will be captured in UTL's [Archive-It account](https://archive-it.org/collections/6473)._

**8) Will my Islandora site's page URLs be preserved in New Collections?**

_No - but the ITS team has set up re-directs that will re-direct old Islandora URLs to the appropriate new Collections U of T website's URLs, per collection, once the new site is publicly launched. Remember to continue to always use the **permalink URLs** when sharing collections and items with students, faculty, researchers, and the public._

**9) Why did UTL migrate the Collections U of T service off of Islandora?**

_We selected a UTL-homegrown IIIF digital image collection discovery solution based on existing technology and infrastructure supported by UTL ITS and Scholars Portal. This homegrown solution is best suited to provide flexible and scaleable technology for the Collections U of T service. It also leverages existing technology and staff expertise at UTL and Scholars Portal. You can read more about our research and planning around this migration in our [2020 Code4Lib article on the topic](https://journal.code4lib.org/articles/15000). Additional information about the New Collections platform will published in the year ahead._

Have more questions? [Email us!](mailto:digitalinitiatives@library.utoronto.ca)  
