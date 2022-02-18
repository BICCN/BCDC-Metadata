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

## BossDB

### Project

* Name
* Title
* Short Title
* Keywords
* Description
* Year
* Public
* Image Banner
* Image Tile
* Species
* Imaging Modalities
* Imaging Locations
* Publications
* Contributor
* Date Created
* License
* Unique Identifier

### Collections

* Name
* Description
* Public
* Creator
* Contributors
* Date Created
* License

### Experiments

* Name
* Description
* Public
* Creator
* Contributors
* Date Created
* License
* Species
* Image Location
* Protocol
* Coordinate Frame

### Channels

* Name
* Description
* Public
* Creator
* Contributors
* Date Created
* License
* Imaging Modality
* Image Resolution
* Channel Type
* Data Type

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

| BIL (Dataset)    | DANDI (Dandiset   | NeMO (BDBag)             | BKP (DataCollectionProject     | BossDB                     | Data Wrangling             |
|------------------|-------------------|--------------------------|--------------------------------|----------------------------|----------------------------|
| title            | name              | Data Set Title           | dataCollection.title           | Collection.name            | Collection.title           |
|                  |                   |                          | dataCollection.shortTitle      |                            | Collection.shortTitle      | 
| rights           | license           | Data license             | license                        | Collection.license         | Collection.license (new)   | 
| rightsURI        | license           | Data license             | license.urlResource.url        |                            | License.webResource        | 
| rightsIdentifier | license           | Data license             | license                        |                            | License.name               | 
| rights           | access            | Data access              | dataCollection.accessControl   | Collection.public          | Collection.accessControl   | 
| abstract         | description       | Data set description     | dataCollection.description     | Collection.description     | Collection.description     | 
|                  | url               | Source data URL          | dataCollection.webResources    |                            | Collection.webResource     | 
|                  | identifier        | Nemo Identifier          | dataCollection.referenceId     | Collection.name            | Collection.name            | 
|                  | citation          | Full data set citation   | dataCollectionProject.citation |                            | Collection.citation (new)  | 
|                  | version           | version                  | dataCollection.lastUpdatedDate |                            | Collection.lastUpdatedDate | 
|                  | doi               |                          |                                |                            | Collection.doi             | 
|                  |                   |                          |                                | Project.uniqueIdentifier   | Project.doi                | 
|                  | publishedBy.name  | Data publication         |                                | Project.publication        | Project.publication        | 
|                  |                   |                          | shortTitle                     | Project.shortTitle         | Project.shortTitle         | 
|                  | publishedBy.title | Data publication         | title                          | Project.title              | Publication.title          | 
|                  | status            |                          | dataCollection.accessControl   | Project.public             | Collection.accessControl   | 
|                  |                   | External identifier      |                                | Project.name               | Collection.name            | 
|                  | contributor       | Organization             | dataCreator                    | Project.creator            | Project.creator            | 
|                  | contributor       | Contact information      | contact                        | Project.contributors       | Project.contact            | 
|                  | contributor       | Contact                  | contact                        | Project.contributors       | Project.contact            | 
|                  | contributor       | Grant support            | grant                          | Project.funding            | Project.grant              | 
|                  | resource          | Protocol ID              | protocol                       | Experiment.protocol        | Project.protocol           | 
|                  | wasGeneratedBy    | Consortium or Project    | subProgram.program             |                            | Project.subProgram         | 
|                  |                   | Data repository RRID     |                                | Project.name               | Collection.RRID            | 
|                  |                   | Community standards used |                                |                            | Program.webResource        | 
