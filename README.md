# Deep learning to diagnose VEXAS syndrome with peripheral blood smear   

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

Coming soon.

## Jupyter notebooks

### 1. [Self-supervised contrasting learning.ipynb](https://github.com/fchabrun/VEXAS-BloodSmear/blob/main/Self-supervised%20contrastive%20learning.ipynb)

<p>This script describes the steps followed for training the deep learnings encoders to translate leukocyte images into encodings, using self-supervised contrastive learning. Please note that input data (i.e. cell images) are not available in this github repository due to size considerations, but may be shared upon request from a qualified medical research investigator, as stated in our original manuscript.</p>

### 2. [Phenotypic prediction.ipynb](https://github.com/fchabrun/VEXAS-BloodSmear/blob/main/Phenotypic%20prediction.ipynb)

<p>This script describes the steps followed for testing the deep learning encoders and performing VEXAS phenotypic prediction. Data used (i.e. leukocyte images encodings and associated metadata) are available in the https://github.com/fchabrun/VEXAS-BloodSmear/tree/main/out directory.</p>
