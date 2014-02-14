API v1: Dossiers
==============

Access the dossiers for individual patients

## Retrieve the dossier of a given patient:
    GET /api/v1/dossiers/{:id}

Provide de following parameters:

 * `id` - Unique identifier for the patient to gather the dossiers for (the epd_id of a patient).

Result:

 * `id`                   - (integer) unique dossier id,
 * `epd_id`               - (string) the provided patient id, unique for a patient,
 * `formal_name`          - (string) name of the patient,
 * `gender`               - (string) gender of the patient,
 * `birthdate`            - (date) birthdate of the patient,
 * `sync_status_message`  - (string) message showing if the data is up to date,
 * `editable`             - (boolean), whether the patient data is editable
