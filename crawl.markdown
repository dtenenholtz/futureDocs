---
title: Crawl
layout: default
nav_order: 2
---
<details open markdown="block">
  <summary>
    Table of contents
  </summary>
  {: .text-delta }
1. TOC
{:toc}
</details>

# Crawling a Website

## 1. Select a seed to crawl. 
Considerations:
* Do we have a related collection?
* Is it related to an important collecting area?
* Is the seed well represented in the Wayback Machine?

## 2. Obtain permission
Only necessary if we do not have an established collecting relationship.

* Send a notification to the site owner of our intent to crawl.
* Allow four weeks for a response. No response will be taken as permission to crawl.
* Do not provide public access until a response is received or the four weeks passes.
* Contact the site owner even if crawling is not restricted by robots.txt as a courtesy and to potentially start a collecting relationship.

## 3. Add the seed to your department's seed list. 
The seed list and Archive-It reports make up the documentation of the crawl. Researchers sometimes need this information, particularly related to scoping decisions, to understand the completeness of the record.

Information to include:
* Information about the site (url, creator, related collection, type of site).
* Reason for collecting.
* Collecting priority. 
* Permissions information.
* Crawl information (intended crawl frequency, result of test crawls).

## 4. Add the seed to a collection
* Make a [new collection](https://support.archive-it.org/hc/en-us/articles/207999936-Create-and-manage-a-collection) in Archive-It if needed 
* Add collection metadata using [UGA Web Archives Metadata Profile](https://github.com/uga-libraries/web-archiving/blob/master/metadata_profile.md).
* Add the seeds to a collection. A seed may only belong to one collection.

## 5. Crawl the seed
If the Archive-It quota is getting low, do not crawl lower priority sites unless there is sufficient quota remaining at the end of the subscription year.

* Add the seed to the crawl (from the collection's seed list).
* Run as a test crawl.
* Select the seed type, generally Standard.
* Adjust the scoping rules. See scoping guidance for specific types of sites, using regular expressions to exclude other languages from Twitter, include or exclude parts of the seed site or linked sites. If necessary, address robots.txt exclusions
* If desired, only capture PDFs.
* Run a test crawl.
* You can monitor a crawl as it runs and cancel it with the "Stop Crawl" button if needed.

## 6. Quality assurance of the crawl
You have 60 days to review and save a test crawl before the content (but not its crawl reports) are deleted.
* Confirm the overall total size is about what you expected based on the site format and any previous crawls of the site.
* Review the crawl reports, especially looking for hosts with large amounts of content that you did not want to capture and for large amounts of blocked or queued or out of scope content you had intended to capture.
* Compare the crawled and live sites. Look for major differences such as missing images, embedded content, or formatting.
* If you have run previous crawls of this site, you can compare the results of each crawl.
* If you didn't get what you want, adjust the scope (see Step 5) and run another crawl.
  * You might also crawl missing pages as separate seeds.
  * For errors in capturing dynamic content try a Brozzler crawl instead.
  * You can add notes to the crawl in Archive-It as a record of what didn't work by clicking "notes" on the crawl overview tab.
* Save the test crawl once you are satisfied with what was captured.

## 7. Add seed metadata
* Use the UGA Web Archives Metadata Profile to determine what information to include.
* Add metadata to Archive-It for the seed.
* Add a description of the archived site in the finding aid if there is a related collection.

## 8. Make the seed public
* Change the private/public status of a single seed
* Change the private/public status of a batch of seeds.
