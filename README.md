# AATC

Full stack web app with several functionalities in the context of clinical trials.

## AACT Schema Explorer

An interactive, single-file web application for visually exploring the **AACT (Aggregate Analysis of ClinicalTrials.gov)** relational database schema.

### Features

- **Force-directed graph visualization** of all 48 AACT tables with physics-based layout
- **Color-coded nodes** by domain: Protocol (blue), Results (orange), Both (purple)
- **Node size** reflects column count; number displayed inside each node
- **Relationship highlighting**: click any table to see its foreign key connections light up
- **Searchable sidebar** with full-text search across table names, column names, and descriptions
- **Filter by domain** (Protocol / Results) or cardinality (1:1 / 1:Many)
- **Detail panel** showing all columns with data types, PK/FK badges, descriptions, relationships, and auto-generated SQL JOIN examples
- **Interactive controls**: pan, zoom (scroll wheel), drag nodes, Grid View, toggle `nct_id` edges
- **Zero dependencies** — single HTML file, no build step, no server required

### Usage

Open `index.html` in any modern web browser. No installation needed.

### Data Sources

Schema data was extracted from [AACT Database Documentation](https://aact.ctti-clinicaltrials.org/), the [AACT GitHub Repository](https://github.com/ctti-clinicaltrials/aact) (`schema.rb`, `foreign_keys.json`), and [ClinicalTrials.gov](https://clinicaltrials.gov/). The explorer includes **48 tables**, **63 foreign key relationships**, and full column metadata.
