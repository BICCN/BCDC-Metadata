# Required fields for data collections

A summary of required fields to start a data collection across all organizations that BCDC collaborates with

## BIL

From https://www.brainimagelibrary.org/newmetadatamodel.html

### Dataset

* Title
* Rights
* rightURI
* rightsIdentifier
* Abstract

### Specimen

* Species
* NCBITaxonomy
* Age
* AgeUnit
* Sex

## DANDI

### Draft Dandiset

From https://github.com/dandi/schema/blob/master/releases/0.6.2/dandiset.json

* name
* description
* identifier
* citation
* manifestLocation
* version
* license

### Published Dandiset (including above)

From https://github.com/dandi/schema/blob/master/releases/0.6.2/published-dandiset.json

* datePublished
* url
* doi
* publishedBy.name
* assetsSummary.numberOfBytes
* assetsSummary.numberOfFiles

## NeMO

### BDBag

From https://github.com/nemoarchive/documentation/blob/master/data_citation.md
metadata spreadsheet found
here: https://docs.google.com/spreadsheets/d/1s7ZJaC9kYyyDnkYShRImmFXV11yxAO70mCV2ZhD1OvM/edit?usp=sharing

* External identifier
* Data Set Title
* Organization
* Contact information
* Contact
* Grant support
* Data set description
* Protocol ID
* Keywords
* Consortium or Project
* Data repository RRID
* Data license
* Data access
* Community standards used

## BKP GraphQL API

### DataCollectionProject

* title
* shortTitle
* description
* subProgram
* dataCollection
* creator
* license

#### DataCollection

* title
* shortTitle
* description

## BCDC Data Wrangling (Preferred)

### Project

* collection
* name
* title
* shortTitle
* description
* citation
* specimenType
* modality
* species
* technique
* creator
* grant
* license
* highlightedWebResource
* protocol

### Collection

* name
* title
* shortTitle
* description
* accessControl
* completionState
* modality
* species
* technique
* subprogram
* webResource

### Grant

* name
* title
* identifier
* reportSymbol
* funder
* awardee

### Subprogram

* name
* title
* shortTitle
* description
* informationResource

### Program

* name
* title
* shortTitle
* description
* informationResource

## Minimum for cross-institutional synchronization

| BIL (Dataset)    | DANDI (Dandiset   | NeMO (BDBag)             | BKP (DataCollectionProject     | Data Wrangling             |
|------------------|-------------------|--------------------------|--------------------------------|----------------------------|
| title            | name              | Data Set Title           | dataCollection.title           | Collection.title           |
|                  |                   |                          | dataCollection.shortTitle      | Collection.shortTitle      |
| rights           | license           | Data license             | license                        | Collection.license (new)   |
| rightsURI        | license           | Data license             | license.urlResource.url        | License.webResource        |
| rightsIdentifier | license           | Data license             | license                        | License.name               |
| rights           | access            | Data access              | dataCollection.accessControl   | Collection.accessControl   |
| abstract         | description       | Data set description     | dataCollection.description     | Collection.description     |
|                  | url               | Source data URL          | dataCollection.webResources    | Collection.webResource     |
|                  | identifier        | Nemo Identifier          | dataCollection.referenceId     | Collection.name            |
|                  | citation          | Full data set citation   | dataCollectionProject.citation | Collection.citation (new)  |
|                  | version           | version                  | dataCollection.lastUpdatedDate | Collection.lastUpdatedDate |
|                  | doi               |                          |                                | Collection.doi             |
|                  |                   |                          |                                | Project.doi                |
|                  | publishedBy.name  | Data publication         |                                | Project.publication        |
|                  |                   |                          | shortTitle                     | Project.shortTitle         |
|                  | publishedBy.title | Data publication         | title                          | Publication.title          |
|                  | status            |                          | dataCollection.accessControl   | Collection.accessControl   |
|                  |                   | External identifier      |                                | Collection.name            |
|                  | contributor       | Organization             | dataCreator                    | Project.creator            |
|                  | contributor       | Contact information      | contact                        | Project.contact            |
|                  | contributor       | Contact                  | contact                        | Project.contact            |
|                  | contributor       | Grant support            | grant                          | Project.grant              |
|                  | resource          | Protocol ID              | protocol                       | Project.protocol           |
|                  | wasGeneratedBy    | Consortium or Project    | subProgram.program             | Project.subProgram         |
|                  |                   | Data repository RRID     |                                | Collection.RRID            |
|                  |                   | Community standards used |                                | Program.webResource        |
