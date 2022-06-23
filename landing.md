# Publication landing pages

From: Simon Worthington, Open Science Lab, TIB. NFDI4Culture. 23 June 2022. simon.worthington@tib.eu

## Auto-generated landing pages

The issue we are trying address solve is giving visibilty to other versions of a publication: formats, editions etc. Our observation is that publications quite often don't make avaiable information about other versions.

Feedback requested: 

We are looking for feedback on whether a version of Linked Open Data (LOD) metadata for a publication could be automatically used for rendering human and machine readable outputs. The idea is to have a small app that could gather metadata sources, cache (Kafka like) a limited LOD data-set, then output in different format based on a model of Content Addressable URL-Caching to create the required humand machine readable data needed. Publication display platforms could then use this data as best suits them - simply as a URL for an HTML landing page to show details of all other versions, or to create Web Element info boxes, publication navigation menus, etc. The simplest presentation data would be a menu link-list of other publication versions - short title, or format, or translation, plus a metadata version?

Does this already exist? Is their a working model or standard for doing this?

More details below in *Details: Auto-generated landing pages*

## About: The NFDI4Culture working group “enhanced publications” (TA4) 

URL: https://nfdi4culture.de/what-we-do/task-areas/task-area-4.html

The working group looking to establish criteria for enhancing a publication. Our aim is to make a definition and recommendations within a culture context of how to make a publication open, and what additional functionality and enrichment can be added. What types of requirements are made of scholarly publishing to be fully open, and how these are implemented in systems or infrastructure.

For this purpose we are comparing and looking at a very wide spectrum of publications ranging from conventional academic papers and monographs, to multi-modal project outcomes, or enriched historical databases.

## Question about publication landing pages

The working group is collating publication features that it sees as important to make a publication to be enhanced for open.

A key feature identified is 'Landing pages - to create visibility of all publication formats, editions, versions, or tranlations'.

### Description of the question

If a publication has multiple formats, output locations, editions, versions, or tranlation then a method is needed to make these visible on each instance. This information needs to be machine readable and human readable. The use of a landing page and access URL is one way to provide information about all outputs. If an access URL or the landing page is visible on each output then a manifest, or inventory (list) of publications can be made available. 

Our brief research has found that this is not done in most cases.

## Example

Open Book Publishers (OBP) do good job on human readable, but not sure about machine readable version - https://www.openbookpublishers.com/product/1535

The following paper points to the need for 'landing pages' and the use of an 'access URL' for a publication - see the following table - https://journals.plos.org/plosbiology/article/figure?id=10.1371/journal.pbio.2001414.t001 - Paper: 'Identifiers for the 21st century: How to design, provision, and reuse persistent identifiers to maximize utility and impact of life science data' https://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.2001414 

## Details: Auto-generated landing pages

The concept is to: 

a. To get as close to using primary source metadata as possible to ensure sustainability, and avoid duplication, extra work, or avoid the creation of errors.

b. Avoid being platform dependent as publications appear on all types of platforms. This is for metadata sources and publication display platforms.

c. Have as low technical bar for entry.

*Could the answer be about creating a simple LOD model for publication availabily, with these features?*

  - The ability to load metadata sources, like: DOIs, ISBN or ISSN records, Wikidata records.

  - With a LOD validator.

  - With a disambiguator.

  - And an human and machine rending output based on Content Addressable URL-caching models.

  - The result could be that the admin can select human and machine readable that they want from a form and it then generates them a landing access page URL or which users could attached a DOI, other PID, or crypto ID.

  - The service can be something self hosted, institutional hosted, or as a community service like Zenodo.

  - The output could be a static output, or it could be a live data output that updates when changes are made, self validates with CI, or at regular intervals.

*How would it work*

1. User inputs links to source metadata for publication.
2. Data is retreived, validated and created a LOD output.
3. User selects human and machine readable outputs needed, e.g., human = json feed for webpage - machine = Dublin Core XML URL.
4. User reviews outputs and goes back to metadata sources and makes inputs if needed.
5. User embeds output data URLs into their publication - the outputs can then be treated as preferred by publication platform - simple links to landing page, or as Wikpedia like infoboxes.

LOD fields to include:

   - ?
   - Model in Wikidata following Wikimedia book model?







