# Pheno006 example dataset: Two sessions with one imaging-only session

This dataset contains imaging and phenotypic data from the baseline session and phenotypic data from followup sessions. Note how these sessions files do not contain `acq_time`, which will trigger a warning in the validator under the `"AdditionalValidation": ["Phenotype"]` in the `dataset_description.json`. The file tree is as follows:

```bash
pheno006
|-- README.md
|-- participants.json
|-- participants.tsv
|-- phenotype
|   |-- tool-ACE_phenotype.json
|   |-- tool-ACE_phenotype.tsv
|   |-- tool-demographics_phenotype.json
|   `-- tool-demographics_phenotype.tsv
|-- sub-01
|   `-- ses-baseline
|       `-- anat
|           |-- sub-01_ses-baseline_T1w.json
|           `-- sub-01_ses-baseline_T1w.nii.gz
`-- sub-02
    `-- ses-baseline
        `-- anat
            |-- sub-02_ses-baseline_T1w.json
            `-- sub-02_ses-baseline_T1w.nii.gz

8 directories, 11 files

```
