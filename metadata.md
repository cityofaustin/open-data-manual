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

#### `Title`
~~Human-readable name of the asset. Should be in plain English and include sufficient detail to facilitate search and discovery.~~  
Asset name in standard format to facilitate initial search and discovery.  

Some titles start with the year, some with the department, some with publishing frequency (e.g. Annual, Weekly), some with a description.  If we have department and publishing frequency as separate categories, those can be removed from title.  Year should be moved to the end of the title so datasets separated by year sort together.  What else should be in the standard?  

With Department and Frequency as categories:  
  
Asset Name  
Asset Name - Date  
  
Without one or both:  
Asset Name - Date, Frequency  
Asset Name - Date, Department  
Asset Name - Date, Frequency, Department  

Date formats:   
YYYY  
YYYY/QQ  
YYYY/MM  
YYYY/MM/DD  

**Purpose:**  To facilitate initial search and discovery.    
**Granularity:**  Standardized format, character limit 100?  
**Public**

#### `Description` 
~~Human-readable description (e.g., an abstract) with sufficient detail to enable a user to quickly understand whether the asset is of interest.~~  
Description or abstract in plain language with sufficient detail to determine whether the dataset meets the user's needs.
**Purpose:**  to enable a user to determine whether the asset is of interest  
**Granularity:** Character limit  500?  1000?  
**Public**  

#### `Last Update`
Most recent date on which the dataset was changed, updated or modified.   Automated.  
**Purpose:**  identifying stale datasets  
**Granularity:**  date (could be datetime, but really?)  
**Public**

#### ~~`Publisher`~~
~~The publishing entity and optionally their parent organization(s).~~   

#### `City Department`
**Purpose:**  Publisher is a little too generic.  City Department gives the user at least a basic idea where the data came from if they are pursuing further inquiry.   
**Granularity:**  City department?  Department and division?  Anything more granular than department would need to be optional since datasets may span departments or be the results of collaborative effort.  If we don't have any multi-departmental datasets, then Department is fine.  Drop-down list.  
**Public**

#### ~~`Tags`~~  `Keywords`
~~Tags (or keywords) help users discover your dataset; please include terms that would be used by technical and non-technical users.~~   
**Purpose:**  Technical and plain language search terms not otherwise included in the description or title to assist users in locating the data of interest.  
**Granularity:** Character limit  
**Public**  

####`Technical Contact`
Email address of the technical contact responsible for the data.  Chris has determined this data IS private.  
**Purpose:**  if a dataset is stale or has issues, another City user can ask if the set should be marked closed or let them know to fix it.   
**Granularity:**  what is our max email address length?      
**PRIVATE**  

####`Rowcount`
**Purpose:**  Users can choose to set page size or download dataset depending on the device used and need.  Automated.  
**Granularity:**  integer  
**Public**  


# List of optional elements: 


#### ~~`Department Budget Code`~~
~~The code for the COA Department represented by the dataset, as listed by the Budget Office. (needs link to dataset)~~  
**Purpose:** What information are you trying to impart to the public with this?  Origin of data?  Cost center?  What if the data has no associated cost center?  What if the data published spans several budget areas?  Moved to optional for these reasons.  I'm not really sold on this without a solid user purpose.  Second, would the public even know what a budget code is?  How to interpret it?  I've worked here eight years and I'm still confused.  
**Granularity:**  same issue  
**Public**  

#### `Category`  IN PROGRESS 
Even if categories are optional at the start, it's a good exercise to try to categorize our datasets.  If we can determine a logical categorization strategy, we can better understand how to help the public find what they are looking for.  

#### `Update Frequency`
**Purpose:**  Threefold:  publically, so the user knows how often to check for changes in volatile data; internally, to determine when a dataset has become stale or lost its technical contact; and to remove the need for these words in the standardized title.   
**Granularity:**  editable drop-down list  
**Public**  

#### `Related Datasets`
**Purpose:**  To guide the public toward data of similar interest.  Datasets in a series, or (if we monitor this) datasets frequently visited together or representing similar information.  May be superceded by Category and Subcategory.  
**Granularity:**  title and URL with those character limits  
**Public**  

#### `Data Dictionary`
**Purpose:**  Any clarification necessary for interpreting the data.  Including but not limited to units of measure; explanation of specific technical terms, abbreviations and acronyms; description of terms which exist only in the sphere of interest represented by the data; expansion of column names representing a related series.  
**Granularity:**  column max but try to keep it brief  
**Public**  

#### `Views`
**Purpose:** Determine whether dataset is being used and/or should be more or less frequently updated  
**Granularity:** integer   
**Public**  

#### `Downloads`
**Purpose:** Same as Views   
**Granularity:** integer   
**Public**  

#### `Types`
**Purpose:** Similar to viewType/displayType if we can get that clearly defined.  This field would clarify datasets with similar or identical data but offering different formats for different purposes.
**Granularity:** drop-down list  
**Public**

#### Metadata in Socrata 

**For discussion**   
department  (City Department)  
attribution  
category (Category)  
description (Description)  
title (Title)  
frequency (Update Frequency)  
issued  
modified (Last Update)  
displayType (Types)  
ViewCount(Views)  
downloadCount (Downloads)  
numberOfComments  
viewType (Types)  
accessLevel (public/private)    
landingPage    
dtype  
keyword (Keywords)  
contactPoint (Technical Contact)  
publisher  
identifier  


#### References
- [Project Open Data Schema 1.1](https://project-open-data.cio.gov/v1.1/schema/)
- [metadata element matrix](https://docs.google.com/spreadsheets/d/1aKp0ygULe6u6Dbrtj3ZOXn4rN3SV5hv-K5Ho4vlT3EE/edit?usp=sharing)
