# Proposed Agent and Tool Plan

## Goal
The system will extract and organize rainfall and crop information from
different source modalities and store the structured information in a database.

## Source 1: Rainfall Excel

File:
RainfallData2020.xlsx

Proposed tool:
- Excel reader

Purpose:
- Read rainfall tables
- Extract district, station, month, rainfall and rainy-day information
- Restructure the data into the knowledge-base schema

## Source 2: Scanned Crop Report

File:
ApprovedSLCSR2020_21.pdf

Proposed tools:
- OCR
- Table extraction

Purpose:
- Read the scanned crop-statistics tables
- Extract district, crop, area, production and yield
- Preserve page-level source information

## Validation

Extracted values should be checked before being stored in the database.

Possible validation:
- Required-field checks
- Numeric-format checks
- District-name consistency
- Manual verification for selected OCR outputs

## Database

The validated structured data will later be stored in a queryable database.

## Proposed Flow

Source
→ Appropriate extraction tool
→ Structured output
→ Validation
→ Database
→ Agent-based querying
