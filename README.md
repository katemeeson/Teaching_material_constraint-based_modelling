## **Teaching material constraint-based modelling** ##
- This repository contains some tutorials for constraint-based modelling, which would be useful for undergrads, masters students, PhD students, or anyone taking on constraint-based modelling for the first time. You can work through each tutorial, changing different modelling parameters to get an understanding of how these models work and what sort of visualisations you can perform to study their output. For any questions, or if you would like to collaborate in delivering this material to students, feel free to contact me at kate.meeson@manchester.ac.uk

## **Table of contents**
### **Tutorials**
####   1. 'Yeast_optimisation_tutorial.ipynb' 
- Tutorial for setting up your constraint-based modelling using the Yeast8.5 genome-scale model (PMID: 31395883; Lu et al, 2019) and the COBRA toolbox (Ebrahim et al, 2013). Required packages for this tutorial are in the first few cells of the notebook
####   2. 'CHO_modelling.ipynb'
- Tutorial for exploring the metabolic organisation and subsystems included in full-scale Chinese hamster ovary (CHO) cell models and a reduced CHO model
####   3. 'OV56_model_transcriptomics.ipynb'
- Tutorial for setting up a model for the OV56 ovarian cancer cell line. This includes adding media constraints according to the DMEM-F12 media and gene expression (RNAseq) constraints from the Cancer Cell Line Encyclopedia. I couldn't upload the Human-GEM-annotated.xml, but you can download this yourself at biomodels or from the Authors https://github.com/SysBioChalmers/Human-GEM/tree/main/model, but you may need to convert IDs using their txt file: https://github.com/SysBioChalmers/Human-GEM/blob/main/model/reactions.tsv, alternatively, email me (kate.meeson@manchester.ac.uk) and I will send you the version of the model that I was working with at the time

## **Models used in tutorials**
### 1. 'yeast-GEM.xml' 
- XML file for the yeast genome-scale model used in the 'Yeast_optimisation_tutorial.ipynb' tutorial (PMID: 31395883; Lu et al, 2019)
### 2. 'iCHO2441_221-107_producing.xml'
- XML file for the comprehensive CHO genome-scale model iCHO2441 (PMID: 36866411; Strain et al, 2023) updated with metabolic subsystems
### 3. 'iCHO2291.xml'
- XML file for the 2020 comprehensive CHO genome-scale model iCHO2291 (PMID: 32330653; Yeo et al, 2020)
### 4. 'CHOmpact_GEM_2023.xml'
- XML file for the 2023 reduced CHO metabolic model CHOmpact (PMID: 37272445, Jiménez Del Val et al, 2023)
### **Other resoruces**
### 1. 'Helpsheet Kate Meeson 181224.pdf' 
- Help sheet for constraint-based modelling, aimed at an audience with limited modelling background.

## **Repository layout** ##
Tutorials/
├── Chinese_Hamster_Ovary_cells/            # Folder containing tutorial for Chinese Hamster Ovary (CHO) cells  
  ├── CHO_modelling.ipynb                   # Tutorial for constraint-based modelling of CHO cells
  ├── CHOmpact_GEM_2023.xml                 # Reduced CHO metabolic model  (Jiménez Del Val et al, 2023)
  ├── iCHO2291.xml                          # 2020 CHO GEM (Yeo et al, 2020)
  ├── iCHO2441_221-107_producing.xml        # 2023 CHO GEM (Strain et al, 2023) updated with subsystems
├── Ovarian_cancer/                         # Folder containing tutorial for ovarian cancer modelling
  ├── OV56_model_transcriptomics.ipynb      # Tutorial for constraining the Human1 GEM with transcriptomics to create OV56 cell line-specific model
  ├── Gene_expression_constraints_OV56.csv  # Gene expression constraints from the Cancer Cell Line Encyclopedia for OV56
  ├── DMEM_F12_all_bounds.csv               # Specific media conditions for the OV56 cell line
├── Yeast/                                  # Folder containing tutorial for yeast cells
  ├── Yeast_optimisation_tutorial.ipynb     # Tutorial for constraint-based modelling of yeast cells
  ├── yeast-GEM.xml                         # Yeast GEM (Lu et al, 2019)

## **Acknowledgements** ##
I (Kate Meeson) acknowledge the University of Manchester, who employed me during the time in which I generated these tutorials. And I thank all students who have tested them as an introduction to their project 😀 
