---
layout: page
title: 'Metadata Standard'
file: metadata.md
---

**Status:** Unapproved draft  

**Next step:** Share with open data liaisons for early review and feedback  

#### Questions and feedback are encouraged! Please submit [here](https://github.com/cityofaustin/open-data-docs/milestones/Metadata%20Standard%20v1.0).

***

### About this document

This document explains how to use metadata to describe open data assets held by the City of Austin. By using a common and consistent metadata vocabulary across City departments, we can make it easier for people to discover and use City information. 

**When would someone use these metadata standards?**

* An open data liaison publishing a new resource to the City's open data portal
* A City web developer wanting to make a department's open data offerings more discoverable by search engines
* A member of the public looking for a dataset to use in a project

**What does the metadata standard contain?**

* A list of descriptors (metadata elements) that should be provided whenever a dataset is published on the open data portal
* Description of when to use the metadata elements
* Details about how to use each element correctly

#### Design principles

* Be interoperable with existing standards such as those developed by the Federal Government and popular web search engines
* Start small and increase the number of elements over time
* Develop openly and in close collaboration with end users

# When to use these metadata elements:

#### Required
Use of the standard metadata elements is required when publishing any dataset to the open data portal. The metadata values should also be included in the open data inventory. 
> An open dataset is a table, map, or any other resource that is published to the open data portal.

#### Optional
Any time a public dataset is shared internally or publically, it is beneficial to include these metadata elements in a note or accessory file that accompanies the share. All City of Austin staff and partners are welcome to use this standard. 

# List of required elements:

***Holly*** - to make sure we are thinking these through, I am adding three comment areas to each element:  Purpose (why include this component of metadata?), granularity (scale of element or field), audience (public or private).  We don't know if there will be private metadata available so all marked private must be optional.


#### `Title`
Human-readable name of the asset. Should be in plain English and include sufficient detail to facilitate search and discovery.
**Purpose:**  To facilitate initial search and discovery.  Truncate description after "plain English".  Sufficient detail is implicit.  
**Granularity:**  Character limit? 100?  
**Public**

#### `Description` 
Human-readable description (e.g., an abstract) with sufficient detail to enable a user to quickly understand whether the asset is of interest.   
***Holly*** - Perhaps 'Sufficiently detailed summary or abstract to clarify contents beyond title'.  
**Purpose:**  to enable a user to determine whether the asset is of interest  
**Granularity:** Character limit?  500?  1000?  
**Public**  

#### `Last Update`
Most recent date on which the dataset was changed, updated or modified.   
***Holly*** - I am assuming this will be automated.  One goal of metadata is to make it as user-friendly as possible from both sides, the client and the publisher.  No one wants to update their metadata every time they update their dataset.  
**Purpose:**  identifying stale datasets  
**Granularity:**  date (could be datetime, but really?)  
**Public**

#### `Publisher`
The publishing entity and optionally their parent organization(s).  
**Purpose:**  What is the purpose?  To allow the user to determine source of data?  But then you have to define source.  
**Granularity:**  City department?  Department and division?  Anything more granular than department would need to be optional since datasets may span departments or be the results of collaborative effort.  
**Public**

#### `Tags`
Tags (or keywords) help users discover your dataset; please include terms that would be used by technical and non-technical users.   
***Holly*** - use keywords.  Tags, labels, etc. are used by proprietary software.  
**Purpose:** for use in search fields - how would this differ from the information in the description metadata?  If your description is sufficient, it should hit most or all of the keywords.  Perhaps synonyms.  
**Granularity:** Character limit XXX  
**Public**

####`Technical Contact`
Email address of the technical contact responsible for the data.  ONLY if private metadata is allowed.   
**Purpose:**  if a dataset is stale or has issues, another City user can ask if the set should be marked closed or let them know to fix it.   
**Granularity:**  what is our longest email address?  Add a few chars and that's it.    
**PRIVATE**  

#### `Category`  GO CHRIS GO

####`Rowcount`
**Purpose:**  Users can choose to set page size or download dataset depending on the device used and need.  ONLY if this is automated.  
**Granularity:**  integer  
**Public**  


# List of optional elements: 


#### `Department Budget Code`
The code for the COA Department represented by the dataset, as listed by the Budget Office. (needs link to dataset)  
**Purpose:** What information are you trying to impart to the public with this?  Origin of data?  Cost center?  What if the data has no associated cost center?  What if the data published spans several budget areas?  Moved to optional for these reasons.  I'm not really sold on this without a solid user purpose.  Second, would the public even know what a budget code is?  How to interpret it?  I've worked here eight years and I'm still confused.  
**Granularity:**  same issue  
**Public**  

#### `Update Frequency`
**Purpose:** Right now we're wasting title space with the words Annual, Weekly, Monthly, Quarterly, Every Five Years, whatever.  
And some data sets may be one-time things.  Take, for example, oh, a post-SXSW customer survey.  They might not ask all the same questions two years in a row.   
But if I'm looking at data for road closures, I  want to know if I need to check back for changes tomorrow or next month. Makes a difference.  
**Granularity:**  editable drop-down list  
**Public**  

#### `Related Datasets`
**Purpose:**  Separate datasets that may be useful together.  Some of these exist already and have been incorporated into GIS maps -- awesome.  Let's say, bike paths, public parks events, and bus schedules.  All different kinds of data, but if a person is looking at one they might say "oh hey, that one is useful too..."  Could also link datasets with their charted subsets.  
**Granularity:**  title/url  
**Public**  

####`Data Dictionary`
**Purpose:**  I stole this from San Fran but wow, it would be wonderful.  I have column names right now with things like International Revenue Enplanements, International Revenue Deplanements, Domestic Revenue Enplanements, Domestic Revenue Deplanements, International Non-Revenue Enplanements....AIEEEEEEEEEE!!!  My columns are ten feet wide.  
How much nicer visually if I could use IntRevEnp, IntRevDep, DomRevEnp, etc. and let the data dictionary explain what the abbreviations mean and what the heck an Enplanement is and why belly freight is different from cargo freight.  
I won't even go into the data sets where one column value is pounds per square inch and the next in liters...  
**Granularity:**  nvarchar(max) but try to keep it brief  
**Public**  



#### References
- [Project Open Data Schema 1.1](https://project-open-data.cio.gov/v1.1/schema/)
- [metadata element matrix](https://docs.google.com/spreadsheets/d/1aKp0ygULe6u6Dbrtj3ZOXn4rN3SV5hv-K5Ho4vlT3EE/edit?usp=sharing)
