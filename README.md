# Azure Data Factory Practice

Hands-on practice with Azure Data Factory (ADF) and Azure Data Lake Storage Gen2 (ADLS Gen2).

This repository contains my practice work as I continue learning and building Azure Data Engineering pipelines.

## Architecture

Source CSV Files
        ↓
Azure Data Lake Storage Gen2
        ↓
     Raw Layer
        ↓
Azure Data Factory
        ↓
   Get Metadata
        ↓
      ForEach
        ↓
    Copy Activity
        ↓
     Bronze Layer
        ↓
Azure Data Lake Storage Gen2

## Technologies

- Azure Data Factory
- Azure Data Lake Storage Gen2
- Azure Managed Identity
- Azure RBAC
- GitHub
- CSV

## Concepts Practiced

- Linked Services
- ADLS Gen2
- Managed Identity
- RBAC
- Datasets
- Parameterized Datasets
- Pipeline Parameters
- Dynamic Content
- Copy Activity
- Get Metadata
- ForEach Activity
- Raw and Bronze Data Layers
- GitHub Integration

## Pipelines

### Parameterized File Copy

Created a reusable pipeline to copy files from the ADLS Gen2 Raw layer to the Bronze layer using parameterized datasets.

### Dynamic File Processing

Created a pipeline using:

Get Metadata → ForEach → Copy Activity

The pipeline automatically discovers files in the Raw folder and processes them dynamically using `@item().name`.

## Project Status

🚧 Ongoing

I will continue adding more Azure Data Engineering concepts and projects as I progress.

## Future Learning

- Incremental Load
- Watermarking
- Triggers
- Error Handling
- Lookup Activity
- ADF → Databricks Integration
- PySpark Transformations
- Silver and Gold Layers
