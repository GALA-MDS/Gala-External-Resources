# CHIST ERA 2025 Proposal - GALA

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

This repository compiles and organizes three distinct but synergistic data sources created for the CHIST ERA 2025 proposal. Our goal is to lay the groundwork for an advanced multi-lingual framework that goes beyong the general trends of state-of-the-art models seem today. These sources could potentially serve as a stepping stone to get our goal.

The sources include:

- **Disaster Dataset:** Scraped from [ReliefWeb](https://reliefweb.int) and parsed using an LLM (GPT-4o) into a structured case-base format.
- **Multilingual Embedding Rankings:** A CSV summary benchmarking current state-of-the-art multilingual embedding models.
- **Radiography Medical Usecase:** A comprehensive medical imaging dataset built from data sourced from [MedPix](https://medpix.nlm.nih.gov/) and the [VQA-RAD Dataset](https://paperswithcode.com/dataset/vqa-rad), used to support advanced diagnostic and analysis tools in radiography.

This repository not only details the data collection and processing methods but also explains how each dataset supports a multi-lingual, multi-modal system with potential for future expansion.

---

## Technologies

<div style="display: flex; flex-wrap: wrap; align-items: center;">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=selenium&logoColor=white" alt="Selenium">
  <img src="https://img.shields.io/badge/GPT_4o-FF5722?style=for-the-badge&logo=openai&logoColor=white" alt="GPT-4o">
  
</div>

---


## Folder Structure & Dataset Overview

```plaintext

├───Disaster_Dataset
│   │   llm_parser.ipynb           # Notebook for parsing scraped disaster data using GPT-4
│   │   main.ipynb                 # Main analysis notebook for disaster dataset
│   │
│   └───assets
│       │   cbr_casebase_dict.json
│       │   disaster_details.json           # Detailed disaster descriptions and metadata
│       │
│       └───.ipynb_checkpoints
│               cbr_casebase_dict-checkpoint.json
│               disaster_details-checkpoint.json
│
├───Multilingual_Embedding_Rankings
│       Multi_Lingual_Embedding_Model_Ranking_2025_March.csv  # Summary CSV for multilingual embedding models
│
└───Radiography_Medical_Usecase
    │   medical_case_base.ipynb      # Notebook for processing and analyzing the medical imaging case base
    │
    ├───chromedriver-win64         # Selenium ChromeDriver files for web scraping tasks
    │       chromedriver.exe
    │       LICENSE.chromedriver
    │       THIRD_PARTY_NOTICES.chromedriver
    │
    ├───VQ-RAD-Case-Base           # Processed medical case base data for the radiography usecase
    │   │   results.json
    │   │   structured_cbr_link_dict.json
    │   │   structured_results.json
    │   │   VQA_RAD Dataset Public.json
    │   │
    │   ├───.ipynb_checkpoints
    │   │       results-checkpoint.json
    │   │       structured_cbr_link_dict-checkpoint.json
    │   │       structured_results-checkpoint.json
    │   │       VQA_RAD Dataset Public-checkpoint.json
    │   │
    │   └───images                # Associated images for the medical case base
    │
    └───VQ-RAD-Dataset           # Original dataset files for the VQA-RAD project
        │   Readme.docx
        │   VQA_RAD Dataset Public.json
        │   VQA_RAD Dataset Public.xlsx
        │   VQA_RAD Dataset Public.xml
        │
        └───VQA_RAD Image Folder
            │   synpic100132.jpg
            │   synpic100176.jpg
            │   synpic100228.jpg
            │   synpic12210.jpg
            │   synpic13385.jpg
            │   ...
            │   synpic60831.jpg
            │   synpic676.jpg
            │   synpic9872.jpg


