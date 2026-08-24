# Pheno006 example dataset: Two sessions with one imaging-only session. Sessions file is an "inventory".

This dataset contains imaging and phenotypic data from the baseline session and phenotypic data from followup sessions. This an example of a case where adding a sessions file will be only an "inventory" of sessions. In other words, a sessions file only contains `participant_id` and `session_id` and does not feel strictly necessary here, but with the `"AdditionalValidation"` from BEP036 it is REQUIRED still. Bear in mind these sessions files do not contain `acq_time`, which will trigger a warning in the validator as well. The file tree is as follows:

```bash
pheno006
|-- README.md
|-- participants.json
|-- participants.tsv
|-- phenotype
|   |-- tool-ACE_phenotype.json
|   |-- tool-ACE_phenotype.tsv
|   |-- tool-Demographics_phenotype.json
|   `-- tool-Demographics_phenotype.tsv
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
