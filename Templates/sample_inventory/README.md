# Instructions for the Sample Metadata Template
The sample metadata template contains all the information necessary to add
a new samples to our inventory. There are three
sheets in this Excel document: `Sample_Metadata`, `Controlled Values`, and
`Data_Collections_CV`. The `Sample_Metadata` sheet is filled out with the
appropriate information about your samples. The other two sheets contain
controlled vocabularies for the fields in the first sheet and should not be
modified. ***Please do not rename, add, or remove sheets from this template.***

For any requests or other questions about the form, please don't
hesitate to contact the Data Curation team at 
[data.curation@alleninstitute.org](mailto:data.curation@alleninstitute.org)
so we can assist you.


## Usage of sample/specimen identifiers and types
In order to better enable synchronization of specimen metadata with the
files deposited at the data archives, we encourage you to provide your list
of samples/specimens at the most granular level that corresponds to files
(or a bundle of files) at an archive. It important that your sample identifier
matches between your archive manifest and the BCDC. In addition, we have fields
in the template for Sample/Parent Specimen/Subspecimen Types, and it would
be very helpful for us if you could provide as much of this information as is 
relevant to your dataset.


## Explanation of metadata fields
Please refer to the following descriptions of the fields when filling out
the `Sample_Metadata` sheet on the
`Sample_Inventory_Metadata_2021Q3_template.xlsx`:


#### **Sample ID** (string)
* The unique identifier of the biological sample. 

#### **Sample Type** (string)
* The specimen type of this sample. The list of permitted values are found in 
the `Specimen Type` box in the `Controlled Values` tab.

#### **Species** (string)
* Common name for the species of the sample. The list of permitted values can
be found in the `Controlled Values` sheet.

#### **Species NCBI Taxonomy ID** (string)
* The unique identifier for the species of the sample (e.g., **NCBI:txid10090**
for mouse). Other species IDs can
be found at the NCBI Taxonomy browser [here](https://www.ncbi.nlm.nih.gov/taxonomy).

#### **Parent Specimen ID** (string, optional)
* The unique identifier of the parent specimen associated with this
sample, if applicable.

#### **Parent Specimen Type** (string, optional)
* The specimen type of the parent specimen associated with this
sample, if applicable. The list of permitted values are found in the 
`Specimen Type` box in the `Controlled Values` tab.

#### **Subject ID** (string, optional)
* The unique identifier of the subject that provided the biological
sample.

#### **Age** (string, optional)
* The age of the subject when the sample was taken. Please also add 
the relevant units to the value (e.g., '24d', 'P56'). 

#### **Sex** (string, optional)
* The sex of the subject. Values are 'male' or 'female'.

#### **Genotype** (string, optional)
* The genotype of the animal. Entries should be formatted as
"allele1/allele2;allele3/allele4".

#### **Modality** (string)
* The type of data modality. These are broad terms used to categorize the data
at a high level. The list of permitted values can be found on the `Controlled
Values` sheet.

#### **Technique** (string)
* The experimental technique that generated this sample. This differentiates 
between data types within a modality. The list of permitted values are found in the 
`Controlled Values` tab.

#### **Anatomical Structure** (string, optional)
* The name of anatomical structure from which sample was obtained. The
`Controlled Values` sheet has links to brain atlas references for mouse
and human structures - fill in this entry with the (acronym/name) field
for the relevant brain area. For marmoset, use the closest analogous
human structure.

#### **Subspecimen Type** (string, optional)
* The type of subspecimen counted, if any. See the `Controlled Values` tab
for allowed values.

#### **Total Processed Subspecimens** (integer, optional)
* Total number of quality-controlled subspecimens from this sample (e.g.,
the number of cells from this sample; if there are no subspecimens,
leave this field blank).

#### **Organization** (string)
* Full name of originating organization. See the `Controlled Values`
tab for the list of accepted values for this field (organizations and
formatting).

#### **Investigator** (string)
* The name of Investigator who conducted the experiment.

#### **Grant Number** (string)
* Identification number of the grant supporting this effort. The list
of current grant numbers can be found in the `Controlled Values` tab.

#### **Data Collection** (string)
* The BCDC code names that describes a given dataset. This reflects the
grouping of data for reporting purposes. The `Data Collection` names
currently in use can be found in the `Data_Collections_CV` tab in the
highlighted column. 

#### **R24 Name** (string)
* The name of R24 archive that has received the files associated with
this sample. This will be **BIL**, **DANDI**, or **NeMO**.

#### **R24 Link** (string, optional)
* A direct link to the publicly accessible dataset with data from this
sample at the R24 archive. If unknown/not yet determined, leave blank.

#### **Comments** (string, optional)
* This is a space for any information that the investigator wants to
provide that may be useful for describing the sample or experiment.

#### **Metadata Submission** (string)
* The Year and Quarter of the initial metadata submission for a sample.
For this quarter, this would be '2021Q3'
