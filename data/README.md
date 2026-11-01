# Data

Public register data from DeepWing, exported as CSV. This folder holds the public layer only: entries that are published on the website (deepwingai.com) under the register's public IDs. Withdrawn entries, unpublished candidates, and internal working registers are never included.

## incident-cases-public.csv

- Register: Desk 1 Incident Case Register （一号台 · AI 事故判例库）, maintained by DeepWing.
- Public source: the case register as published at https://deepwingai.com/cases
- Snapshot date: 2026-10-31
- Contents: the full public set on the snapshot date: 53 cases (INC-001 to INC-053) plus 1 special volume (SP-001). The collection is always counted this way, as cases plus the special volume, never as a single bare total.

### Fields

- `public_id`: the public ID of the entry in the website register. This is the only official numbering; cite entries by this ID.
- `title_zh`: the entry headline in Chinese, as published.
- `title_en`: the entry headline in English, as published.
- `date`: the disclosure date recorded in the case file （披露日期）. Some entries also carry a separate event date inside the case file on the website; this field is always the disclosure date.
- `primary_layer`: the primary failure layer assigned in the case file, using the framework layer names in English (Model, Orchestration, Tool, Memory, Knowledge, Access Control, Observability). SP-001 is filed as "Special File".
- `evidence_grade`: the evidence grade assigned in the case file, in the English form used on the website. The grade taxonomy is defined in Chinese on the website: Primary-source verified （一手已核）, Multi-source verified （多源已核）, Media-reported （媒体转述）, Pending verification （待核）. Two entries carry a qualifier in parentheses as part of their published grade (for example, "Primary-source verified (in part)"); the qualifier is reproduced as published.
- `source_url`: the canonical URL of the entry in the website register. The register cites each case's primary sources by publisher and date inside the case file; follow the entry URL to read the full case file, its timeline, and its source citations.

### Update cadence

The export is refreshed when the public set changes (a case is added, corrected, or withdrawn on the website). Each refresh is recorded in the repository CHANGELOG with its snapshot date. Between refreshes, the website register is the live source and governs in case of any difference.

## Boundary

Only the public layer is exported. Not exported, by design: the internal Desk 1 database (which uses internal working IDs that do not match the public numbering), unpublished candidate cases, and the product-side data listed in the repository README under "What is not here".
