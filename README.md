# HLAG_to_cytokine

**Project Title**
Modularisation of published and novel models toward a complex KIR2DL4 pathway build in CellML

**Author**
Nurul Izza Ismail

**Organisation**
University of Auckland
Universiti Sains Malaysia

**Project Description**
KIR2DL4 is an interesting receptor expressed on the peripheral blood natural killer (pbNK) cell as it can be either activating or inhibitory depending on the amino acid residues in the domain. This model uses mathematical modelling to investigate the downstream effects of natural killer cells’ activation (KIR2DL4) receptor after stimulation by key ligand (HLA-G) on pbNK cells. Development of this large pathway is based on a comprehensive qualitative description of pbNKs’ intracellular signalling pathways leading to chemokine and cytotoxin secretion, obtained from the KEGG database (https://www.genome.jp/pathway/hsa04650). From this qualitative description, we built a quantitative model for the pathway, reusing existing curated models where possible and implementing new models as needed. This large pathway consists of two published sub-models; the Ca2+ model and the NFAT model, and a newly built FCRIγ sub-model. The full pathway was fitted to HLA-G-KIR2DL4 pathway published dataset and the model that we developed fitted well to one of two secreted cytokines. The model can be used to predict the production of IFNγ and TNFα cytokines.

 
Figure 1

**Motivation**
The complexity of the immune system makes it difficult to study, both in vitro and in vivo.
Moreover, difficulties in obtaining human samples create limitations for experimental work.
For these reasons, mathematical modelling was employed in this study to investigate KIR2DL4 pathway NK cell signalling pathways in a biologically realistic manner. Mathematical models have been widely used to complement biological studies of cellular and subcellular signalling pathways and gene regulatory networks and are used widely in systems biology to predict responses of systems under different conditions.

**How to Install and Run the Project**
CellML (www.cellml.org) is a model encoding standard that is used to ensure model reproducibility. OpenCOR (www.opencor.ws) is a simulation package written by Alan Garny that is designed for authoring and running CellML models. OpenCOR is freely available for Windows, Mac, and some Linux platforms. In order to reproduce the results, user has to open the main model called dl4cytokines.cellml in OpenCOR. The SED-ML for the main model is called dl4cytokines.sedml. The main model integrates the sub-models as follows:

Model files:
Main model/top-level model
1.	dl4cytokines.cellml 
2.	dl4cytokines.sedml (SED-ML)

The models it called are:
Level 1 models
1.	dupont_erneux_1997_noIP4.cellml
2.	NFATMyocyte_TomidaProtocol_Submodel.cellml
Level 2 model
1.	FCepsilonRI.cellml
Level 3 models
1.	hG_activation.cellml
2.	NFAT_NFATcytokine.cellml

**Build Status**
This model was built using CellML which was used to produce the original results in the paper, and therefore it is known to be completely accurate. The downloaded model allows users to construct, edit and simulate models on CellML platform.








![image](https://user-images.githubusercontent.com/29026025/171556964-fb13bc76-4835-42f1-a28f-7bec681d8564.png)
