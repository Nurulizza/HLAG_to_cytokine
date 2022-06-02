# HLAG_to_cytokine

## Table of contents
* [Project Title](#project-title)
* [Author](#author)
* [Project description](#project-description)
* [How to install and run the project](#how-to-install-and-run-the-project)
* [Build status](#build-status)
* [Contact information](#contact-information)

## Project title
Modularisation of published and novel models toward a complex KIR2DL4 pathway build in CellML

## Author
Nurul Izza Ismail 

## Organisation
1. University of Auckland
2. Universiti Sains Malaysia

## Project description
KIR2DL4 is an interesting receptor expressed on the peripheral blood natural killer (NK) cell as it can be either activating or inhibitory depending on the amino acid residues in the domain. This model uses mathematical modelling to investigate the downstream effects of natural killer cells’ activation (KIR2DL4) receptor after stimulation by key ligand (HLA-G) on NK cells. Development of this large pathway is based on a comprehensive qualitative description of NKs’ intracellular signalling pathways leading to chemokine and cytotoxin secretion, obtained from the KEGG database (https://www.genome.jp/pathway/hsa04650). From this qualitative description, we built a quantitative model for the pathway, reusing existing curated models where possible and implementing new models as needed. This large pathway consists of two published sub-models; the Ca2+ model and the NFAT model, and a newly built FCεRIɣ sub-model. The full pathway was fitted to HLA-G-KIR2DL4 pathway published dataset and the model that we developed fitted well to one of two secreted cytokines. The model can be used to predict the production of IFNγ and TNFα cytokines.

**Motivation**
The complexity of the immune system makes it difficult to study, both in vitro and in vivo. Moreover, difficulties in obtaining human samples create limitations for experimental work. For these reasons, mathematical modelling was employed in this study to investigate KIR2DL4 pathway NK cell signalling pathways in a biologically realistic manner. Mathematical models have been widely used to complement biological studies of cellular and subcellular signalling pathways and gene regulatory networks and are used widely in systems biology to predict responses of systems under different conditions.

## How to install and run the project
CellML (www.cellml.org) is a model encoding standard that is used to ensure model reproducibility. OpenCOR (www.opencor.ws) is a simulation package written by Alan Garny that is designed for authoring and running CellML models. OpenCOR is freely available for Windows, Mac, and some Linux platforms. In order to reproduce the results, user has to open the main model called dl4cytokines.cellml in OpenCOR. The SED-ML for the main model is called dl4cytokines.sedml. The main model integrates the sub-models as follows:

Model files:
Main model/top-level model
1.	dl4cytokines.cellml 
2.	dl4cytokines.sedml (SED-ML)

The models it called are:
* Level 1 models
1.	dupont_erneux_1997_noIP4.cellml
2.	NFATMyocyte_TomidaProtocol_Submodel.cellml

* Level 2 model
4.	FCepsilonRI.cellml

* Level 3 models
6.	hG_activation.cellml
7.	NFAT_NFATcytokine.cellml

## Build Status
This model was built using CellML which was used to produce the original results in the paper, and therefore it is known to be completely accurate. The downloaded model allows users to construct, edit and simulate models on CellML platform.

## Contact information
1. nism@aucklanduni.ac.nz
2. nurul.ismail@usm.my











