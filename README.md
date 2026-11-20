# CKG-Data

Main copies of the datasets behind the **Climate Knowledge Graph (CKG) for IPCC AR6**, together with the entity-relationship (ER) model that describes how they are linked as Linked Open Data (LOD).

This is research data. Methods are recorded in [`protocols/`](protocols/) so that every dataset can be traced back to its source and processing steps.

## Repository layout

```
CKG-Data/
|-- README.md              This file
|-- CHANGELOG.md           Release notes
|-- CITATION.cff           Citation metadata
|-- LICENSE                GPL-3.0 (code)
|-- LICENSE-DATA.md        CC0 1.0 (data)
|-- datasets/              Main copies of the published datasets
|   |-- acronyms-ar6/
|   |-- authors-ar6/
|   |-- bibliographic-ar6/
|   |-- corpus-ar6/
|   `-- glossary-ar6/
|-- data-model/            ER model and LOD mappings
|-- protocols/             Research protocols and methods
|-- source-data/           Original deposits (read-only)
|-- pipelines/             Scripts that build datasets from source
`-- docs/                  Longer documentation
```

| Folder | Contents |
|---|---|
| [`datasets/`](datasets/) | Main copies of the published datasets, one folder per dataset (CSV, XML, DTD, HTML). Start here if you want the data. |
| [`data-model/`](data-model/) | ER model and mappings to LOD. Start here to see how the data connects. |
| [`protocols/`](protocols/) | Research protocols and methods. |
| [`source-data/`](source-data/) | Original institutional deposits. Treated as read-only. |
| [`pipelines/`](pipelines/) | Scripts that convert source data into the datasets. |
| [`docs/`](docs/) | Longer documentation. |

## Datasets

| Dataset | Description | Folder |
|---|---|---|
| Acronyms (AR6) | [Brief description] | [`datasets/acronyms-ar6/`](datasets/acronyms-ar6/) |
| Authors (AR6) | [Brief description] | [`datasets/authors-ar6/`](datasets/authors-ar6/) |
| Bibliographic (AR6) | [Brief description] | [`datasets/bibliographic-ar6/`](datasets/bibliographic-ar6/) |
| Corpus (AR6) | [Brief description] | [`datasets/corpus-ar6/`](datasets/corpus-ar6/) |
| Glossary (AR6) | [Brief description] | [`datasets/glossary-ar6/`](datasets/glossary-ar6/) |

## Using the data

1. Choose a dataset folder and read its own `README.md` for the schema and fields.
2. Use the DTD to validate the XML.
3. Use the ER model in `data-model/` to see how datasets join.

## Provenance and protocols

- Each dataset states which source deposit and which protocol produced it.
- Processing scripts are in `pipelines/`. Re-running them on `source-data/` should reproduce `datasets/`.

## Versioning

Release notes are in [`CHANGELOG.md`](CHANGELOG.md).

## How to cite

Please cite this repository using the metadata in [`CITATION.cff`](CITATION.cff), or use GitHub's "Cite this repository" button.

## Licence

This repository uses two licences:

- **Code** (scripts in `pipelines/`, XSLT, and other software): GNU General Public License v3.0 (GPL-3.0). See [`LICENSE`](LICENSE).
- **Data** (datasets in `datasets/`, source deposits in `source-data/`, and the ER model in `data-model/`): Creative Commons CC0 1.0 Universal (public domain dedication). See [`LICENSE-DATA.md`](LICENSE-DATA.md).

## Acknowledgement

These data are derived from the Intergovernmental Panel on Climate Change (IPCC) Sixth Assessment Report (AR6). Please acknowledge the IPCC as the original data source when using or redistributing these data, for example:

> Data derived from IPCC (2021/2022) Sixth Assessment Report (AR6), Working Groups I, II and III. Intergovernmental Panel on Climate Change. https://www.ipcc.ch/assessment-report/ar6/

Please also acknowledge the Climate Knowledge Graph (CKG-Data) repository, and cite it as described in [`CITATION.cff`](CITATION.cff).

## Contact

[Name, institution, email or GitHub contact]
