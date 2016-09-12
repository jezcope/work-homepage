<!-- 
.. title: DataCite Client Meeting July 2016
.. slug: datacite-client-meeting-july-2016
.. date: 2016-07-25 11:24:30 UTC+01:00
.. tags: DataCite,Metadata,Citation
.. category: Meetings
.. link: 
.. description: 
.. type: text
-->

On Monday 25 July, I went down to London for a DataCite Client meeting hosted by the British Library. The main purpose of the event was to communicate updates from DataCite, but it was also an opportunity to discuss some key issues and feed back possible areas for further development, as well as the ever-present networking.

The main update centred around the development of [version 4.0 of the DataCite metadata schema](http://schema.labs.datacite.org/), which is due to go into production in September.  The main changes here are:

- `resourceTypeGeneral` is now *mandatory*
- `creatorName` has been expanded to optionally allow family name and given name to be identified
- `fundingReference` is a new optional property with subfields: `funderName`, `funderIdentifier`, `awardNumber`, `awardURI`, `awardTitle`
  - `contributorType` "funder" now deprecated
- Polygon option available for geolocation

Version 4.1 is already in planning, and is expected to include updates to align with [the FORCE11 Software Citation Principles](https://www.force11.org/software-citation-principles) and recent working groups on dynamic citation.

We were given a number of recommendations to maximise the usefulness of our metadata in line with recently-created tools:

- The ORCID auto-update tool requires the use of ORCIDs to identify contributors
- DataCite event data (which enables tracking of "events" such as citations) depends on proper use of `relatedIdentifier`
- Use of a URI to link to rights statements (instead of just including these as free text) enables machine analysis and discovery based on the rights

Both the ORCID tool and the DataCite event data tracker are recent developments from the THOR (Technical & Human infrastructure for Open Research) project, which has the goal of helping systems and services to link and actively exchange information, building on existing systems of identifiers for people, publications and datasets, along with less-well established identifiers for organisations, funders and grants. They have introduced a [Knowledge Hub](https://project-thor.readme.io/) with lots of helpful documentation and a [dashboard of persistent identifier adoption](http://dashboard.project-thor.eu).

Vimal Shah of King's College London and Rachel Proudfoot of the University of Leeds both gave brief presentations on developments in their own services. Both have relatively manual workflows for ingesting metadata and minting DOIs: King's have used out-of-the-box functionality in Microsoft SharePoint to provide a mediated deposit workflow for their data catalogue; Leeds use a simple standalone [DataCite metadata generator](https://github.com/mpaluch/datacite-metadata-generator) to create XML and set up temporary landing pages to enable minting of DOIs for data which isn't itself available yet.

Finally, there was a good workshop-style session focusing on licensing, in which we were invited to submit queries for discussion. My query, about how to represent non-open licenses/right statements in a machine-readable way produced some interesting discussion. Two resources flagged up were:

1. The RIOXX "All Rights Reserved" license URI: http://rioxx.net/licenses/all-rights-reserved/
2. The W3C [Open Digital Rights Language (ODRL) spec](https://www.w3.org/TR/odrl/)

Overall it was a useful catchup.
