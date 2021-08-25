# Instructions for filling out Project Collection Template
The project and data collection template contains all the information necessary
to add a new project and/or data collection to our inventory. There are three
sheets in this Excel document: `Data collection project`, `Data collection`,
and `values`. The first two sheets are to be filled out with the appropriate
information about your project and data collection. The third sheet contains
controlled vocabulary and should not be modified.

Existing data collections and projects can be edited via requested made through
the metadata submission webpage, reached by your personalized link at
`https://bcdc-md-management.org/feedback?userid=<your_unique_issued_id_here>`.

If you have any questions or need us to set up a personalized link to the
metadata submission webpage, please feel free to email
[data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org)
so we can assist you with adding and updating project inventory metadata.

### Adding data collections to an existing project
If you are adding data collections to an existing project, please make sure you
have the human-readable identifier name for the project you are adding collections to.
On the `Data collection project` sheet, put this identifier as the value for the 
`Project` property. Put the identifier for your new data collection in the 
`has output` field of the `Data collection project` sheet. 
In the `Data collection` sheet, put the same identifier in the `Collection` 
field that you put in the `has output` field before. Add the necessary 
information for your new collection to the `Data collection` sheet. 
There is no need to modify any fields in the `Data collection project` sheet
except for `Project` and `has output` as mentioned before.

### Adding multiple data collections
If you have multiple data collections to add, please simply copy the 
`Data collection` sheet until you have enough sheets for all your new data 
collections. The sheet names do not matter, but the values in the `has output` 
field on the `Data collection project` sheet must match the identifiers in the 
`Collection` field on each `Data collection` sheet. The following section
describes the methods for adding multiple values to the `has output` field.

### Adding multiple values for a property
Multiple values can be added to some fields by using one of three methods:
1. Put the multiple values in the same cell, separated by commas.
2. Copy the row that you would like to duplicate, insert it below the
   original one, and change the value of the new row as appropriate.
3. The same as option 2, but the first cell can be left blank because the
   `Property name` is inferred from the row above.
   
#### Properties that *do not* support multiple values
On the `Data collection project` sheet, the following fields do not support multiple values:
* Project
* Title
* Short title
* Description

On the `Data collection` sheet, the following fields do not support multiple values:
* Collection
* Title
* Short title
* Description
* Access control
* Completion state

The addition of multiple values is supported for all other properties as 
described in the previous section.

### Explanation of properties and values
Please refer to the following descriptions of values when filling out `project_collection_template.xlsx`:

## Data collection project
This sheet contains information about your data collection project

A **project** describes the intent of the work and encapsulates a set of data 
collections that are tightly connected. Author attribution, license, and grant 
information is recorded at the project level. If your project has multiple
funding sources, licenses, or different sets of authors, you may want to
divide it into multiple projects.

#### **Project** - *project identifier* 
  * This is a unique human-readable identifier (i.e. handle) used to keep track 
    of your project
  * This identifier must match the project identifier given to the data 
    archives when submitting sample inventory
  * If your project does not have a name yet, you can email us at
    [data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org),
    and we will provide you with one.
  
#### **is part of** - *subprogram*
  * This is the subprogram that your project is part of (often a grant name)
  * This field is controlled by the vocabulary in the `subprogram` column on `values` sheet
  * If you don't see your subprogram on that list, please just add it in the cell
    to the right of the relevant field, then email
    [data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org), 
    so that we can update this template.
    
#### **is highlighted by** - *URL*
  * This is a hyperlink to something related to your project
  * Up to 3 URLs can be included here that will show up in the search results page
  * Two possible types of URLs to include would be:
    * A project-specific page that the data submitter has created to showcase the project and data
    * A data download URL (we generally add the data download URL for each data collection to this field)
  
#### **is funded by** - *grant*
  * This is the grant that is funds your project
  * This field is controlled by the vocabulary in the `grant` column on `values` sheet
  * If you don't see your grant on that list, please add it in the cell immediately 
    to the right of the relevant field, then email
    [data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org), 
    so that we can update this template.

#### **has use of results limited by** - *license*
  * This is the usage license for the data collected by this project
  * This field is controlled by the vocabulary in the `license` column on `values` sheet
  * Most BICCN projects should have a `CCBY4` license (https://creativecommons.org/licenses/by/4.0/) 
  * Most Allen Institute projects should have an `AIBSTOU` license 
    (https://alleninstitute.org/legal/terms-use/), unless they are receiving BICCN funding 
  * If there are related data included in this project that received funding from 
    a separate source, then it could potentially be submitted with a separate license
  * Please contact [data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org)
    and / or program officer if you are not sure what license to use.

#### **has methodology specification** - *protocol URL*
  * This is a hyperlink to a protocol, usually from https://www.protocols.io/.
  * The BICCN requires that protocols be provided in support of all data submitted. 
    These should take the form of a URL to a protocol drafted specifically for this dataset
  * You can submit multiple values for this field, separated by commas or 
    new rows immediately after this one
  * Please make sure the protocol has been published before providing us a link
  * Provide the URL in the form of a DOI, so we can be consistent with other projects.
  * Example: `http://doi.org/<doi_number>/protocols.io.<protocol_id>`
  
#### **has output** - *collection name*
  * This is a unique human-readable identifier (i.e. handle) used to keep track 
    of your data collection
  * You can submit multiple values for this field, separated by commas or 
    new rows immediately after this one
  * This field is controlled by the vocabulary in the `collection` column on `values` sheet
  * This identifier must match the collection identifier given to the data 
    archives when submitting sample inventory
  * If your data collection does not have a name yet, you can email us at
    [data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org), 
    and we will provide you with one.
  
#### **has contact person** - *person name*
  * This is the person that we will send correspondence to if we have questions 
    or need to talk to you about your project or data collection
  * You can submit multiple values for this field, separated by commas or 
    new rows immediately after this one
  * Usually the contact person is either a data wrangler, a PI, or a lead scientist
  * Please provide names in the following format: `GivenName FamilyName`
  * `GivenName` can include a middle name(s) or initial(s)
  * If `FamilyName` has a space in it please let us know
  
#### **has contributor** - *person name*
  * This is anybody who worked on this project that you would like to include 
    in your data citation
  * You can submit multiple values for this field, separated by commas or 
    new rows immediately after this one
  * Provide the list of names in the order that you would like them to appear 
    in your citation.
  * Please include the PI / PM in this list of names
  * Please provide names in the following format: `GivenName FamilyName`
  * `GivenName` can include a middle name or initial
  * If `FamilyName` has a space in it please let us know

#### **has creator** - *person name*
  * This is usually the PI and / or the person who is primarily responsible 
    for this project
  * You can submit multiple values for this field, separated by commas or 
    new rows immediately after this one
  * Please provide names in the following format: `GivenName FamilyName`
  * `GivenName` can include a middle name(s) or initial(s)
  * If `FamilyName` has a space in it please let us know
  
#### **is subject of publication** - *DOI*
  * This is a hyperlink to a publication about this project
  * You can submit multiple values for this field, separated by commas or 
    new rows immediately after this one
  * Provide the URL in the form of a DOI, so we can be consistent with other projects.
  * Example: `http://doi.org/<doi_number>/<publication_id>`

#### **Title** - *string*
  * This is the long form of the title for this project
    
#### **Short title** - *string*
  * This is a display-friendly title for this project
  * Please limit short titles to 30 characters or fewer
  
#### **Description** - *string*
  * Please limit your project description to one paragraph

## Data collection
This sheet contains information about your data collection

A **data collection** can be created to encapsulate any set of data. Generally,
we prefer the deposition of raw files to be separated into different 
data collections, such that a data collection contains a set of data generated 
by the same methodology and of the same modality. Raw data files and derived data 
files should ideally be separated into different collections (e.g., fastq files vs. 
bam files vs. cell-x-gene matrix) so that we can ingest and report out metadata 
appropriately.

### **Collection** - *collection name*
  * This is a unique human-readable identifier (i.e. handle) used to keep track 
    of your data collection
  * This field is controlled by the vocabulary in the `collection` column on `values` sheet
  * This field corresponds to the `has output` field on the `Data collection project` tab
  * If your data collection does not have a name yet, you can email us at
    [data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org), 
    and we will provide you with one.
    
#### **has samples of type** - *specimen type*
  * This is the type of specimen that this data collection is about
  * This field is controlled by the vocabulary in the `specimen type` column on `values` sheet
  * The specimen type listed here should match the specimen/sample whose 
    identifier is listed in the Sample Inventory template.
  * Please choose the lowest-level specimen type that is appropriate for your collection
  * If you cannot find an appropriate specimen type, please add it in the cell 
    immediately to the right of the relevant field, then email
    [data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org), 
    so that we can update this template.
    
#### **is data about** - *species*
  * This is the common name of the species that this data collection is about
  * This field is controlled by the vocabulary in the `species` column on `values` sheet
  * You can submit multiple values for this field, separated by commas or 
    new rows immediately after this one
  
#### **is data of type** - *modality*
  * This is the name of the data modality for this collection
  * This field is controlled by the vocabulary in the `modality` column on `values` sheet
  * You can submit multiple values for this field, separated by commas or 
    new rows immediately after this one
  
#### **is subject of resource** - *URL*
  * This is usually a link to the repository where the raw data is stored.
  * You can submit multiple values for this field, separated by commas or 
    new rows immediately after this one

#### **was collected using** - *technique*
  * This is the name technique used to acquire data for this collection
  * This field is controlled by the vocabulary in the `technique` column on `values` sheet
  * You can submit multiple values for this field, separated by commas or 
    new rows immediately after this one
  * If you cannot find an appropriate technique, please add it in the cell 
    immediately to the right of the relevant field, then email
    [data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org), 
    so that we can update this template.
  
#### **Title** - *string*
  * This is the long form of the title for this collection
    
#### **Short title** - *string*
  * This is a display-friendly title for this collection
  * Please limit short titles to 30 characters or fewer
  
#### **Description** - *string*
  * Please limit your description to one paragraph
  
#### **Access control** - *access control*
  * This indicates the level of control of access to these data
  * This field is controlled by the vocabulary in the `access control` column on `values` sheet
  * Most non-human data collections should be `open`
  * Human data collections may be either `open` or `controlled` access, 
    depending on the type of data and your IRB approval

#### **Completion state** - *completion state*
  * This indicates whether new data is still being added to this collection
  * This field is controlled by the vocabulary in the `completion state` column on `values` sheet
  * If more data are expected to be added to this collection, then the state is `in progress`
  * If data not more data will be added to this collection, then the state is `complete`
