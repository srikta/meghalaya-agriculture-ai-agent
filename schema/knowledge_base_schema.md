# Knowledge Base Schema

## Project
Rainfall–Crop Intelligence System for Meghalaya

## Purpose
The knowledge base will connect rainfall information with crop area,
production, and yield across districts and agricultural seasons in Meghalaya.

## 1. Location

Fields:
- state
- district
- station

## 2. Rainfall

Fields:
- year
- month
- district
- station
- rainfall_mm
- rainy_days

Source example:
`RainfallData2020.xlsx`

## 3. Crop Statistics

Fields:
- crop_year
- season
- district
- crop_name
- area
- production
- yield

Source example:
`ApprovedSLCSR2020_21.pdf`

## 4. Source / Provenance

Fields:
- source_name
- source_url
- document_name
- page_number
- modality

## Main Relationship

Rainfall and crop statistics will primarily be connected using:

District + Year / Agricultural Season

Example:

Rainfall 2020
        |
        | District
        v
Kharif Crop Statistics 2020-21

## Initial Query Types

The knowledge base should eventually support questions such as:

- What was the rainfall in a particular district in 2020?
- Which crops had the highest yield in a district?
- How did rainfall vary across districts?
- How does rainfall relate to crop production or yield?
- Which source and page contain a particular crop statistic?
