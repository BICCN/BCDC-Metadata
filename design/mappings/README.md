## Docs
* API client [documentation](https://dandi.readthedocs.io/en/latest/modref/index.html)
* Raw [schema definitions](https://github.com/dandi/schema/tree/master/releases)
* [DataCite CVs](https://schema.datacite.org/meta/kernel-4.0/doc/DataCite-MetadataKernel_v4.0.pdf)
    - see Appendices in link or context in dandi's raw schema
* Schema viewer links of latest (0.6.2 at the time of writing) are available here:
    - [dandiset](https://json-schema.app/view/%23?url=https%3A%2F%2Fraw.githubusercontent.com%2Fdandi%2Fschema%2Fmaster%2Freleases%2F0.6.2%2Fdandiset.json)
    - [asset](https://json-schema.app/view/%23?url=https%3A%2F%2Fraw.githubusercontent.com%2Fdandi%2Fschema%2Fmaster%2Freleases%2F0.6.2%2Fasset.json)

## How to read mappings:
* Root level keys correspond to ingest schema (CSV files for specimen, file manifest and project invnetory)
    - keys correspond to columns in csvs
    - values correspond to path of keys in dandi schema
    - The `relations` key denotes a relation between objects
* Path prefix of `asset` corresponds to the asset level metadata for a given dandiset
* Path prefix of `dandiset` corresponds to the dandiset level metadata for a given dandiset

