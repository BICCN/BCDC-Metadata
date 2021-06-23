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

Please refer to the following descriptions of values when filling `project_collection_template.xlsx`:

## Data collection project
This sheet contains information about your data collection project

A **project** describes the intent of the work and encapsulates a set of data 
collections that are tightly connected. Often we have one project for each 
data collection, and a grant may have many projects. A project is currently 
the level at which we provide author attribution, license, and grant information. 
Thus, if you have sets of work that require different sets of authors, 
you would divide the work into multiple data collections.

#### **Project** - *project name* 
  * This is a unique human-readable identifier (i.e. handle) used to keep track 
    of your project
  * If your project does not have a name yet, you can email us at
    [data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org), 
    with a suggested name.
  * We will try to use your suggested name, but we reserve the right to change it if necessary
  * By convention, we prefer to use names in `snake_case_with_proj` as a suffix
  
#### **is part of** - *subprogram*
  * This is the subprogram that your project is part of (often a grant name)
  * This field is controlled by the vocabulary in the `subprogram` column on `values` sheet
  * If you don't see your subprogram on that list, please email 
    [data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org), 
    and we will add it
    
#### **is highlighted by** - *URL*
  * This is a hyperlink to something related to your project
  * Up to 3 URLs can be included here that will show up in the search results page
  * Two possible types of URLs to include would be:
    * A project-specific page that the data submitter has created to showcase the project and data
    * A data download URL (we generally add the data download URL for each data collection to this field)
  
#### **is funded by** - *grant*
  * This is the grant that is funds your project
  * This field is controlled by the vocabulary in the `grant` column on `values` sheet
  * If you don't see your grant on that list, please email 
    [data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org), 
    and we will add it

#### **has use of results limited by** - *license*
  * This is the usage license for the data collected by this project
  * This field is controlled by the vocabulary in the `license` column on `values` sheet
  * For most BICCN projects this should be `CCBY4` (https://creativecommons.org/licenses/by/4.0/)
  * If there are related data included in this project that received funding from 
    a separate source, then it could potentially be submitted with a separate license
  * Please contact [data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org)
    and your program officer to clarify which license to use

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
  * If your data collection does not have a name yet, you can email us at
    [data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org), 
    with a suggested name.
  * We will try to use your suggested name, but we reserve the right to change it if necessary
  * By convention, we prefer to use names in `snake_case` without `_proj` as a suffix
  * Collection names must be unique, so make sure any new data collections do 
    not have a name that is already in the controlled vocabulary
  
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
  * This is a simple string that will be displayed on 
    https://knowledge.brain-map.org/ as your project title
    (note: Title _is not_ displayed for _data collections_)
  
#### **Short title** - *string*
  * This is a simple string is currently not displayed. 
    (note: Short title _is_ displayed for _data collections_)
  * Please limit short titles to 30 characters or less
  
#### **Description** - *string*
  * This is a simple string that will be displayed on 
    https://knowledge.brain-map.org/ as your project description
  

## Data collection
This sheet contains information about your data collection

A **data collection** can be created to encapsulate any set of data. Generally, for 
the BICCN we prefer the deposition of raw files to be separated into different 
data collections, such that a data collection contains a set of data generated 
by the same methodology and for the same purpose. Raw files and derived files 
would ideally be separated into different collections (e.g., fastq files vs. 
bam files vs. cell-x-gene matrix) so that we can ingest and report out metadata 
appropriately. Exceptions may exist to these rules.

### **Collection** - *collection name*
  * This is a unique human-readable identifier (i.e. handle) used to keep track 
    of your data collection
  * This field is controlled by the vocabulary in the `collection` column on `values` sheet
  * This field corresponds to the `has output` field on the `Data collection project` tab
  * If your data collection does not have a name yet, you can email us at
    [data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org), 
    with a suggested name.
  * We will try to use your suggested name, but we reserve the right to change it if necessary
  * By convention, we prefer to use names in `snake_case` without `_proj` as a suffix
  * Collection names must be unique, so make sure any new data collections do 
    not have a name that is already in the controlled vocabulary
    
#### **has samples of type** - *specimen type*
  * This is the type of specimen that this data collection is about
  * This field is controlled by the vocabulary in the `specimen type` column on `values` sheet
  * The specimen type listed here should match the specimen/sample whose 
    identifier is listed in the Sample Inventory template.
  * Each data collection should only have one specimen type
  * Please choose the lowest-level specimen type that is appropriate for your collection
  * If you believe that there is more than one specimen type, you might need a new data collection
  * If you cannot find an appropriate specimen type, or you are not sure which one to use,
    please email [data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org)
    and we will add a new specimen type or help you choose the appropriate one
    
#### **is data about** - *species*
  * This is the common name of the species that this data collection is about
  * This field is controlled by the vocabulary in the `species` column on `values` sheet
  * You can submit multiple values for this field, separated by commas or 
    new rows immediately after this one
  * Usually there is only one species associated with a data collection
  
#### **is data of type** - *modality*
  * This is the name of the data modality for this collection
  * This field is controlled by the vocabulary in the `modality` column on `values` sheet
  * You can submit multiple values for this field, separated by commas or 
    new rows immediately after this one
  * Usually there is only one modality associated with a data collection
  
#### **is subject of resource** - *URL*
  * This is usually a link to the repository where the raw data is stored.
  * You can submit multiple values for this field, separated by commas or 
    new rows immediately after this one

#### **was collected using** - *technique*
  * This is the name technique used to acquire data for this collection
  * This field is controlled by the vocabulary in the `technique` column on `values` sheet
  * You can submit multiple values for this field, separated by commas or 
    new rows immediately after this one
  * Usually there is only one technique associated with a data collection
  * If you cannot find an appropriate technique, or you are not sure which one to use,
    please email [data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org)
    and we will add a new technique or help you choose the appropriate one
  
#### **Title** - *string*
  * This is a simple string is currently not displayed. 
    (note: Title _is_ displayed for _data collection projects_)
    
#### **Short title** - *string*
  * This is a simple string that will be displayed on 
    https://knowledge.brain-map.org/ as your data collection title
    (note: Short title _is not_ displayed for _data collection projects_)
  * Please limit short titles to 30 characters or less
  
#### **Description** - *string*
  * This is a simple string that will be displayed on 
    https://knowledge.brain-map.org/ as your data collection description
  
#### **Access control** - *access control*
  * This indicates the level of control of access to these data
  * This field is controlled by the vocabulary in the `access control` column on `values` sheet
  * Most non-human data collections should be `open`
  * Human data collections may be either `open` or `controlled` access, 
    depending on the type of data and your IRB approval

#### **Completion state** - *completion state*
  * This indicates whether or not new data is still being added to this collection
  * This field is controlled by the vocabulary in the `completion state` column on `values` sheet
  * If more data are expected to be added to this collection, then the state is `in progress`
  * If data not more data will be added to this collection, then the state is `complete`
