# Deep learning to diagnose VEXAS syndrome with peripheral blood smear

<p align="center">
<img src="https://github.com/fchabrun/VEXAS-BloodSmear/blob/main/Figure%201.png?raw=true" width="80%">
</p>

## Authors
**Floris Chabrun**<sup>[§](#authors),[1](#affiliations),[2](#affiliations)</sup>, **Valentin Lacombe**<sup>[§](#authors),[1](#affiliations),[3](#affiliations)</sup>, **Xavier Dieu**<sup>[1](#affiliations),[2](#affiliations)</sup>, **Franck Geneviève**<sup>[4](#affiliations),[5](#affiliations)</sup>, **Geoffrey Urbanski**<sup>[*](#corresponding-author),[1](#affiliations),[3](#affiliations),[6](#affiliations)</sup><br>
<sup>§</sup>contributed equally to this manuscript

### Affiliations
<sup>1</sup> Univ Angers, Inserm 1083, CNRS 6015, MITOVASC, SFR ICAT, F-49000, Angers, France<br>
<sup>2</sup> Laboratoire de Biochimie et Biologie Moléculaire, Centre Hospitalier Universitaire Angers, France<br>
<sup>3</sup> Service de Médecine Interne et Immunologie clinique, Centre Hospitalier Universitaire Angers, France<br>
<sup>4</sup> Laboratoire d’Hématologie, Centre Hospitalier Universitaire Angers, France<br>
<sup>5</sup> Fédération Hospitalo-Universitaire ‘Grand Ouest Against Leukemia’ (FHU GOAL), France<br>
<sup>6</sup> Department of Orofacial Sciences, School of Dentistry, University of California, San Francisco, CA, USA<br>

### Corresponding author
**Geoffrey Urbanski**. Service de Médecine Interne et Immunologie clinique, Centre Hospitalier Universitaire Angers. Univ Angers, Inserm 1083, CNRS 6015, MITOVASC, SFR ICAT, F-49000 Angers, France. Department of Orofacial Sciences, School of Dentistry, University of California San Francisco, San Francisco, CA, USA. Phone: +33 2 41 35 40 03. Fax: +33 2 41 35 49 69. E-mail: <geoffrey.urbanski@ucsf.edu>

## Abstract

**Importance.** VEXAS syndrome is a newly described autoinflammatory disease associated with *UBA1* somatic mutations and vacuolization of myeloid precursors. This disease has a more and more broad spectrum leading to an increase in the number of suspected cases, but it remains a rare disease. Its diagnosis via bone-marrow aspiration and *UBA1*-gene sequencing is time-consuming and expensive.

**Objective.** To identify new markers of VEXAS syndrome within peripheral leukocytes.

**Design.** Deep learning was applied to the analysis of leukocyte images from blood smears collected between January 2020 and May 2022.

**Setting.** Case-control study in a tertiary care center.

**Participants.** We compared three groups: patients with VEXAS syndrome (identified *UBA1* mutation) (VEXAS group); patients with clinical and biological features strongly suggestive of VEXAS syndrome but without *UBA1* mutation (UBA1-WT group); patients with a myelodysplastic syndrome and without clinical suspicion of VEXAS syndrome, that were matched on gender and age to patients from the VEXAS and UBA1-WT groups, with at a 1:1 ratio (SMD group).

**Intervention.** To compare images of circulating leukocytes, we applied a two-step procedure. First, we used self-supervised contrastive learning to train convolutional neural networks to translate leukocyte images into lower-dimensional encodings. Then, we employed support vector machine to predict patients’ condition based on those leukocyte encodings.

**Main Outcome and Measure.** We used mean ROC-AUC to represent the predictive performance of the deep learning model in distinguishing among the leukocytes from the three groups.

**Results.** The VEXAS, UBA1-WT, and MDS groups included 3, 3, and 6 patients respectively. Analysis of 33,757 images of neutrophils and monocytes enabled us to distinguish VEXAS patients from both UBA1-WT and MDS patients, with mean ROC-AUC ranging from 0.87 to 0.95. 

**Conclusions and Relevance.** Image analysis of blood smears via deep learning accurately distinguished neutrophils and monocytes drawn from patients with VEXAS syndrome from those of patients with similar clinical and/or biological features but without UBA1 mutation. Our findings offer a promising pathway to better screening for this disease.

## Jupyter notebooks

### 1. [Self-supervised contrasting learning.ipynb](https://github.com/fchabrun/VEXAS-BloodSmear/blob/main/Self-supervised%20contrastive%20learning.ipynb)

<p>This script describes the steps followed for training the deep learnings encoders to translate leukocyte images into encodings, using self-supervised contrastive learning. Please note that input data (i.e. cell images) are not available in this github repository due to size considerations, but may be shared upon request from a qualified medical research investigator, as stated in our original manuscript.</p>

### 2. [Phenotypic prediction.ipynb](https://github.com/fchabrun/VEXAS-BloodSmear/blob/main/Phenotypic%20prediction.ipynb)

<p>This script describes the steps followed for testing the deep learning encoders and performing VEXAS phenotypic prediction. Data used (i.e. leukocyte images encodings and associated metadata) are available in the https://github.com/fchabrun/VEXAS-BloodSmear/tree/main/out directory.</p>
