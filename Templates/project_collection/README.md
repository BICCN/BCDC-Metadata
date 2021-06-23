# Instructions for filling out Project Collection Template
The project and data collection template contains all the information necessary
to add a new project and/or data collection to our inventory. There are three
sheets in this Excel document: `Data collection project`, `Data collection`,
and `values`. The first two sheets are to be filled out with the appropriate
information about your project and data collection. The third sheet contains
controlled vocabulary and should not be modified.

If you have any questions, please feel free to email
[data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org)
so we can assist you with adding your metadata to the project inventory.


Please refer to the following descriptions of values when filling `project_collection_template.xlsx`:

## Data collection project
This sheet contains information about your data collection project

#### **Project** - *project name* 
  * This is a unique human-readable identifier (i.e. handle) used to keep track 
    of your project
  * By convention, we prefer to use names in `snake_case_with_proj` as a suffix
  * If you are not sure what project name to use, please email 
    [data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org), 
    and we will help you choose one
  
#### **is part of** - *subprogram*
  * This is the subprogram that your project is part of (often a grant name)
  * This field is controlled by the vocabulary in the `subprogram` column on `values` sheet
  * If you don't see your subprogram on that list, please email 
    [data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org), 
    and we will add it
    
#### **is highlighted by** - *URL*
  * This is a hyperlink to something related to your project
  * A landing page with a general overview of your project is best
  * If you don't have a landing page, you could include a DOI for a flagship paper,
    or a link to the repository to where the data for this project are stored
  
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
  * If the project collected Allen Institute data it might use `AIBSTOU` instead
  * Please contact data.curation@alleninstitute.org if you are not sure what license to use.

#### **has methodology specification** - *protocol URL*
  * This is a hyperlink to a protocol, usually from https://www.protocols.io/.
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
  * If your project has a new data collection as it's output, please email 
    [data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org)
    and let us know.
  * Collection names must be unique, so make sure any new data collections do 
    not have a name that is already in the controlled vocabulary
  * By convention, we prefer to use names in `snake_case` without `_proj` as a suffix
  
#### **has contact person** - *person name*
  * This is the person that we will send correspondence to if we have questions 
    or need to talk to you about your project or data collection
  * You can submit multiple values for this field, separated by commas or 
    new rows immediately after this one
  * Usually the contact person is either a data wrangler, or a PI
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

### **Collection** - *collection name*
  * This is a unique human-readable identifier (i.e. handle) used to keep track 
    of your data collection
  * This field is controlled by the vocabulary in the `collection` column on `values` sheet
  * If this is a new data collection, please email 
    [data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org)
    and let us know.
  * Collection names must be unique, so make sure any new data collections do 
    not have a name that is already in the controlled vocabulary
  * By convention, we prefer to use names in `snake_case` without `_proj` as a suffix
  * This field corresponds to the `has output` field on the `Data collection project` tab
    
#### **has samples of type** - *specimen type*
  * This is the type of specimen that this data collection is about
  * This field is controlled by the vocabulary in the `specimen type` column on `values` sheet
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
  * Data collections about human subjects should be separate from other species
  
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
  * Human data collections should be `controlled`

#### **Completion state** - *completion state*
  * This indicates whether or not new data is still being added to this collection
  * This field is controlled by the vocabulary in the `completion state` column on `values` sheet
  * If more data are expected to be added to this collection, then the state is `in progress`
  * If data not more data will be added to this collection, then the state is `complete`
  
#### **Last updated date** - *yyyy/mm/dd*
  * This is the day of the most recent data submission deadline where the `Reported count` was updated
  * Please input the date in `yyyy/mm/dd` format if possible (some software likes to auto-change this)
  
#### **Reported count** - *int*
  * This is the most recent *total* number of specimens reported for this project
  * Please submit specimen counts that correspond to the specimen type specified for this collection
