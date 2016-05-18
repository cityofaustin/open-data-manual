---
layout: page
title: 'City Data Inventory (DRAFT)'
file: inventory.md
---

**Status:** Unapproved draft  

**Next step:** Design inventory schema and add content describe the project  

#### Questions and feedback are encouraged! Please submit [here](https://github.com/cityofaustin/open-data-manual/milestones/Open%20Data%20Inventory).

***

## About the Data Inventory Project

On April 8, 2015, the City Manager issued a memorandum directing all departments to participate in the City of Austin Open Data Initiative 2.0. Included in that memorandum was a requirement that each department create an inventory of known data that it managed and maintained that would indicate:

* a. If the information is publicly-accessible;  
* b. The date of when the information was made publicly-accessible or when it is scheduled to be made public;  
* c. The date the information was last updated or when it is scheduled to be updated;  
* d. If the data is in a consumable format;  
* e. If the information is from a primary source or has been aggregated or modified; and  
* f. If the information is restricted by any legal, license or privacy restrictions.

Additional guidelines set forth by CTM were that the inventory should:

* Include all data that that is considered “public.” Public data is any data that does not have legal or privacy restrictions and would be subject to Texas Public Information Act requirements. And to include data that is considered “private” in its entirety but that can be shared or considered “public” if sensitive/restricted fields are removed when published. 

* List data sets that are published, planned for publication, that are available online in other formats (pdf, doc, etc.) or those that currently have no plans for publication. Data sets identified as “not for publication” must be accompanied by a justification that will be reviewed by the Open Government Executive Board for exemption.

* The initial working version of the dataset inventory was published in Sharepoint for internal use only and included the following fields: Description; Dataset Title; Publication Status; Justification; Planned Date; Data Type; and Upload Frequency.

## Why is a Data Inventory Important?

The following is from the Sunlight Foundation's Open Data Policy Guidelines:

(Source: http://sunlightfoundation.com/opendataguidelines/)

"For an open data policy to have a strong foundation, you first need to know what data you have—and so does the public. Governments should conduct an inventory of existing data early in the process of open data policy development in order for the government and other stakeholders to be aware of the full potential dimensions of data release. While defining total information holdings may be a complex undertaking, governments should conduct as comprehensive a review of existing data information as possible, with the inclusion of information holdings that may benefit from becoming structured data themselves." 

"The inventory should itself be made public. Publicly accounting for agency information helps ensure that information is managed to benefit the public interest, allows for common understanding of what data the government holds, and can create efficiencies among government departments. It empowers policymakers and administrators to determine whether information is being appropriately managed, and empowers the public oversight of those determinations. An individual or group should be charged with oversight of the inventory to ensure its ongoing maintenance and accuracy. To make the listing of data as useful as possible, such a list should also encompass data that may be viewed as sensitive or unlikely to be released (along with any other helpful context.) In addition to setting the stage for meaningful public discussions around dataset release, an inventory process can provide a roadmap for creating ambitious timelines and identify whether new data may need to be collected."

## City of Austin Data Inventory Policy <Requirements 2.1>

### Create and Maintain an Enterprise Data Inventory

#### Purpose

To develop a clear and comprehensive understanding of what data assets they possess, each City of Austin department is required to create an Enterprise Data Inventory (Inventory) that accounts for all data assets created or collected by the department. This includes, but is not limited to, data assets used in the department’s information systems. The Inventory must be enterprise-wide, accounting for data assets across divisions and program, and must use the required Open Data Initiative metadata schema. After creating the Inventory, departments should continually improve the usefulness of the Inventory by expanding, enriching, and opening the Inventory.

#### Objectives

* Build an internal inventory that accounts for data assets used in the department’s information systems
* Include data assets produced through department contracts and cooperative agreements, and in some cases deparment-funded grants; include data assets associated with, but not limited to, research, program administration, statistical, and financial activities
* Indicate if the data may be made publicly available and if currently available
* Describe the data with Open Data Initiative metadata schema.

#### Framework

Since City departments have varying levels of visibility into their data assets, the size and maturity of agencies’ Enterprise Data Inventories will differ across agencies. CTM will assess department progress toward overall maturity of the Enterprise Data Inventory through the maturity areas of “Expand,” “Enrich,” and “Open.”

##### Expand 
Expanding the inventory refers to adding additional data assets to the Inventory. Departments should develop their own strategy to expand the inventory and break down the work according to department-defined classes of data. Departments should communicate their plans for expanding the Inventory in the Inventory Schedule (described in the minimum requirements). As departments develop an Inventory Schedule, they may find it helpful to group their data assets into classes of data. 

##### Enrich
To improve the discoverability, management, and re-usability of data assets, departments should enrich the Inventory over time by improving the quality of metadata describing each data asset. 

##### Open 
Departments should implement tools and processes that will accelerate the opening of additional valuable data assets by making them public and machine-readable, while ensuring adequate policy, process, and technical safeguards are in place to prevent against the release of sensitive data. Departments are required to increase the number of public data assets included in the Public Data Listing (described in the next section) over time. Departments should work toward increasing the ratio of data that are public and machine-readable to data that can be made public as measured in the Inventory.

### Minimum Requirements to Create and Maintain an Enterprise Data Inventory

#### Develop and submit an Inventory schedule by INSERT DATE

* Describe how the department will ensure that all datasets from each division and program in the department have been identified and accounted for in the Inventory, to the extent practicable, no later than INSERT DATE.
* Describe how the department plans to expand, enrich, and open their Inventory each quarter through INSERT DATE at a minimum; include a summary and milestones in the schedule
* Publish Inventory Schedule on the INSERT URL by DATE

#### Create an Enterprise Data Inventory by INSERT DATE

* Include, at a minimum, all dataset which were posted on data.austintexas.gov before INSERT DATE and additional representative datasets from divisions and programs.
* Ensure the Inventory contains one metadata record for each dataset. A data asset can describe a collection of datasets (such as a CSV file for each state).
* Use “required” fields and “required-if-applicable” fields on data.austintexas.gov (includes indicating whether data can be made publicly available).
•	Submit to ODI via INSERT METHOD the inventory as a single JSON file using the defined schema from data.austintexas.gov. ODI invites department input on the option of replacing future submission with an API via a discussion on data.austintexas.gov.

#### Maintain the Enterprise Data Inventory (ongoing after INSERT DATE) ## Let's discuss Insert dates
* Continue to expand, enrich, and open the Inventory on an on-going basis
* Update the Inventory Schedule submitted on INSERT DATE on a quarterly basis on the INSERT ULR OR METHOD

### Create and Maintain a Public Data Inventory

#### Purpose

To improve the discoverability and usability of data assets, all departments must contribute to a Public Data Inventory, which contains a list of all data assets that are or could be made available to the public. This Public Data Inventory, posted at data.austintexas.gov, would typically be a subset of the department’s Inventory. This will allow the public to view agencies’ open data assets and subsequent progress as additional data assets are published.

Departments should include entries for non-public data assets in their Public Data Inventory, taking into account guidance regarding information that cannot be made public. For example, an agency may list data assets with an ‘accessLevel’ of ‘restricted public’ to make the public aware of their existence and the process by which these data may be obtained.

#### Objectives

* List any data assets in the department’s Enterprise Data Inventory that can be made publicly available, i.e. not restricted or non-public
* Publish Public Data Inventory at data.austintexas.gov
* Include data assets produced through department-funded grants, contracts, and cooperative agreements

#### Publish a Public Data Inventory (by INSERT DATE)

* Include, at a minimum, all data assets that are categorized as "Public" in the Enterprise Data Inventory. By design, a department should be able to filter the Inventory to generate the Public Data Inventory.
* Publish the Public Data Inventory at data.austintexas.gov.
* Follow the schema available on INSERT URL.
* Include link in the data asset’s metadata for all data assets in the Public Data Inventory that are already publicly available on data.austintexas.gov, as opposed to those that could be publicly available.

### Create a Process to Help Facilitate and Prioritize Data Release

#### Purpose

Identifying and engaging with key data customers to help determine the value of City data assets can help departments prioritize those of highest value for quickest release. Data customers include public as well as government stakeholders. 

Departments may develop criteria at their discretion for prioritizing the opening of data assets, accounting for a range of factors, such as the quantity and quality of user demand, internal management priorities, and agency mission relevance. As customer feedback mechanisms and internal prioritization criteria will likely evolve over time and vary across agencies, departments should share successful innovations in incorporating customer feedback through the Open Data Initiative to disseminate best practices. Departments should regularly review the evolving customer feedback and public engagement strategy.

#### Objectives

* .....
* .....
* .....


## How to Create Your Data Catalog (Inventory)
The first major task for the Data Liaisons is to create a data catalog (or inventory) of your
department’s data. Below we provided guidance on how to do this. But we recognize that this
will be in part a learning process. As a result, we will make changes to this guidance based on
your feedback. After the initial catalog creation, this process may continue as new datasets are
created, discovered or requested by other parties.
Follow the 3 major steps below to conduct your data inventory:
  1. Identify data sources
  2. Brainstorm and identify datasets in each data source
  3. Complete dataset inventory template (for each dataset)
We also included an example from the Rent Board that you can use for guidance. Appendix A.
includes templates to support this process.
Also, visit this resource for additional guidance:

  ● [Bloomfire Austin Open Data] (https://opendata.bloomfire.com)

## Step 1: Identify data sources
Your data may be housed in a variety of places from
inside information systems or databases
to shared drives and folders. This can also include 3rd party vendors and data hosted on vendor
systems. Step 1 is about identifying the major data sources in your department.

Questions to help identify and discover data sources:
  1. What information systems does your department use? On premise or hosted? 
  2. What databases does your department use? These include databases that are maintained by other departments.
  3. What applications capture information or are used in your business processes?
  4. Are some data resources kept in spreadsheets (on shared or individual drives)?
  5. What reports do you create on a regular basis?
  5. What information are we already publishing and where did that information come from?  For each of the data sources:
  6. Provide a name and brief description of the data sources
  7. Capture any technical details and point of contacts
Appendix A. includes a templates for this process.

## Step 2: Identification of Data Assets and Datasets
Some of your information sources may be fairly straightforward (e.g. a single sheet in a
spreadsheet). In these cases, you have already identified the dataset.
In addition, you may already have a list of datasets you are publishing or plan to publish.
But others, like relational databases, may be very complex. Identifying subsets of the database
that could serve as datasets, probably requires some brainstorming. You may want to include
your PIO, data stewards and lead analysts in this process.
To help brainstorm, use the questions below:
  1. What data populates your monthly or quarterly reports?
  2. What departmental data is currently publicly available on DataSF or elsewhere online?
  3. What data does your department use for internal performance and trend analysis?
  4. What information is published as a performance metric?
  5. What data is reported to federal, state or local agencies?
  6. Talk with your Public Information Officer (PIO) what data has been requested under Sunshine?
  7. What data do other departments ask for?
  8. What kinds of open data are similar agencies across the country publishing?
      Caution: Don’t exclude any datasets based on privacy or confidentiality concerns! Our goal is to
      have a holistic picture of our data. Based on this big picture, we can then decide what we should
      publish. Step 3 provides a means to capture privacy and confidentiality concerns.

## Step 3: Complete dataset inventory template
For each dataset you identify in Step 2, complete the inventory template. Include:
1. New datasets (identified via brainstorming)
2. Existing datasets, including already published datasets
Appendix A. includes the templates and description of template fields.

#### Purpose

The first step in releasing open data is identifying which data sets or data resources to release. There are a number of easy ways to identify data that is suitable for release.

#### Objectives / Methods

##### Identify sources

* Program/Data Owners
* Legal Counsel
* Data Stewards/IT
* Department Executives
* Public Information Officer

##### Establish research questions

* What data (including historical data) does the department collect, maintain, or hold? 
* What “high value” data are currently publicly available? 
* What underlying data populates aggregate information in published reports? 
* What data does the department policy and planning unit use for trending and statistical analysis? 
* What data are reported to the federal government; or frequently requested by other government entities (federal, state, local)? 
* What data is the subject of frequent PIR requests? What data is the public requesting? 
* What data have not been previously published but meet the definition of “high value”? 

### Assessment and Prioritiazation of Data Assets and Datasets

#### Purpose
Test purpose
...

#### Objectives

* Low Inventory Complexity
* Medium Inventory Complexity
* High Inventory Complexity

### Publish Data to Airtable 
Brad will include instructions to AirTable.

#### Purpose

To publish to Airtable . . . 

#### Objectives

##### Understand the expectation

* . . .
* . . .
* . . .

##### Obtain access to Airtable

* . . .
* . . .
* . . .

##### Add rows to the inventory

* . . .
* . . .
* . . .

# View the current inventory (experimental)

[Metadata AirTable] (https://airtable.com/tblHs9vJwdOxhrbQB/viwh4RJGgLjQSxqTB)

[Erin AirTable] (https://airtable.com/tbll3avqmLebbGmS9/viwxHAlM6pk5JrpX8)

<iframe class="airtable-embed" src="https://airtable.com/embed/shrz1xwqcxvm117x1?backgroundColor=purple&viewControls=on" frameborder="0" onmousewheel="" width="100%" height="533" style="background: transparent; border: 1px solid #ccc;"></iframe>

