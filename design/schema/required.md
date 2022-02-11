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

| BIL | DANDI | NeMO | BKP | 
|--|------------------|--------------------|------------------------------| 
| Dataset.title | Dandiset.name | BDBag.dataSetTitle | dataCollection.title | 
| N/A | N/A | N/A | dataCollection.shortTitle | 
| Dataset.rights | Dandiset.license | BDBag.dataLicense | dataCollectionProject.license |
| Dataset.rightsURI | Dandiset.license | BDBag.dataLicense | dataCollectionProject.license | 
| Dataset.rightsIdentifier | Dandiset.license | BDBag.dataLicense | dataCollectionProject.license | 
| Dataset.rights | Dandiset.access | BDBag.dataAcess | dataCollection.accessControl |
| Dataset.abstract | Dandiset.description | BDBag.dataSetDescription | dataCollection.description | 
| N/A | Dandiset.url | BDBag.sourceDataUrl | dataCollection.webResources | 
| N/A | Dandiset.identifier | BDBag.NemoIdentifier | dataCollection.referenceId |
| N/A | Dandiset.citation | BDBag.fullDataSetCitation | dataCollectionProject.citation | 
| N/A | Dandiset.manifestLocation | BDBag.sourceDataUrl | N/A | 
| N/A | Dandiset.version | BDBag.version | dataCollection.lastUpdatedDate | 
| N/A | Dandiset.doi | N/A | N/A |

