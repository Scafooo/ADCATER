# ADCATER Dataset and Ontology

## Overview
ADCATER is an international initiative aimed at enhancing nutritional care for hospitalized patients by leveraging computer vision and semantic data management technologies. This repository contains the ADCATER food image dataset, used for analyzing patient diet intake, and the ontology developed to manage and integrate nutritional, medical, and food consumption data.

## Computer Vision Dataset
The ADCATER dataset includes high-resolution images of hospital meals, captured both before and after consumption, to monitor patient food intake. These images, acquired using a portable device, cover a variety of food categories and are annotated at the pixel level for each food type. This dataset was developed to train convolutional neural networks (CNNs), specifically the Mask R-CNN model, to segment images and classify various types of food.

### Dataset Highlights
- **Format**: 4K images, pixel-level annotations
- **Food Categories**: 39 different categories, including yogurt, semolina, salads, bread, etc.
- **Annotations**: Created using [LabelMe](https://github.com/labelmeai/labelme), with polygons identifying food regions and assigned categories.

For detailed information on the dataset and annotations, refer to the _ADCATER food image dataset_ section in the [Article](link to the article) paper.

## ADCATER Ontology
The ADCATER ontology integrates data from various healthcare and food management systems to support patient care and nutritional assessments. Developed with Graphol and compliant with OWL, this ontology provides a semantic structure to link patient health information, nutritional data, and food supply chain data.

### Ontology Features
- **Concepts**: 43 concepts representing items such as served meals, patient conditions, and nutritional metrics.
- **Relationships**: 28 semantic relationships linking concepts.
- **Attributes**: 65 descriptive attributes, useful for tracking details such as caloric intake, consumption of specific nutrients, and nutritional status assessment.

The ontology also supports integration with standard ontologies, including SNOMED CT, ICD, and FoodOn, to enable integrated data access and food traceability.

## System Architecture
The ADCATER system is designed with two main components:
1. **Data Sources Layer**: Collects data from Electronic Health Records (EHRs), nutritional planning tools, and food supply chain systems.
2. **Data Management Layer**: Enables data reconciliation and anonymization using the ontology and organizes the data in a data warehouse for business intelligence analysis.

The system also provides an interface for data visualization, allowing exploration of nutritional variables, Key Performance Indicators (KPIs), and assessment metrics for healthcare professionals.

## Installation and Usage
1. Clone the repository:
   ```bash
   git clone https://github.com/username/ADCATER.git
   cd ADCATER
