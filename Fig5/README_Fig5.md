## Patient-Specific responses

We devised a novel strategy to capture genes with patient-specific profiles, spanning both baseline and treatment stages. This approach was designed to circumvent the numerous "technical" confounds encountered when employing standard statistical methods.

Subsequently, we aggregated these patient-specific genes into biological pathways, operating under the hypothesis that individualized features may converge upon common core signaling pathways.

<br>

## Workflow

Our approach comprises the following steps:

1. Select a treatment group.
2. Remove sex-related genes.
3. Split the replicates into 2 matrices.
4. Calculate VSD - the median of other samples.
5. Select genes by sorting the values of each gene in each sample.
6. Pick the common up- or down-regulated genes for each sample.
7. Combine common up- or down-regulated genes from all samples for pathway analysis.


![](README_Fig5/workflow.png)

<br>

## Pathways

All Pathways are saved in the **Pathways** folder. 

#### CC_mes

Here is the link to the CC_mes html file. [html](Pathways/CC/mes/CC_mes/AnalysisReport.html)

Here is the link to the CC_mes result file. [result](Pathways/CC/mes/CC_mes/metascape_result.xlsx)

![](Pathways/CC/mes/pathways/Signaling_by_GPCR.png)

<br>

![](Pathways/CC/mes/pathways/Non_integrin_membrane_ECM_interactions.png)

<br>

![](Pathways/CC/mes/pathways/Signaling_by_WNT.png)

<br>

![](Pathways/CC/mes/pathways/RHO_GTPase_cycle.png)

<br>

![](Pathways/CC/mes/pathways/WNT_ligand_biogenesis_and_trafficking.png)

<br>

![](Pathways/CC/mes/pathways/Cell_junction_organization.png)

<br>

#### CC_epi

Here is the link to the CC_epi html file. [html](Pathways/CC/epi/CC_epi/AnalysisReport.html)

Here is the link to the CC_epi result file. [result](Pathways/CC/epi/CC_epi/metascape_result.xlsx)

![](Pathways/CC/epi/pathways/IGFBPs.png)

<br>

![](Pathways/CC/epi/pathways/Signaling_by_Receptor_Tyrosine_Kinases.png)

<br>

![](Pathways/CC/epi/pathways/Cell_junction_organization.png)

<br>

![](Pathways/CC/epi/pathways/MHC_class_II_antigen_presentation.png)

<br>

![](Pathways/CC/epi/pathways/Signaling_by_GPCR.png)

<br>

![](Pathways/CC/epi/pathways/O_linked_glycosylation.png)

<br>

![](Pathways/CC/epi/pathways/RHO_GTPases_Activate_Formins.png)

<br>


#### TG_mes

Here is the link to the TG_mes html file. [html](Pathways/TG/mes/TG_mes/AnalysisReport.html)

Here is the link to the TG_mes result file. [result](Pathways/TG/mes/TG_mes/metascape_result.xlsx)

![](Pathways/TG/mes/pathways/Signaling_by_Receptor_Tyrosine_Kinases.png)

<br>

![](Pathways/TG/mes/pathways/IGFBPs.png)

<br>

![](Pathways/TG/mes/pathways/Diseases_of_glycosylation.png)

<br>

![](Pathways/TG/mes/pathways/Diseases_associated_with_glycosaminoglycan_metabolism.png)

<br>

![](Pathways/TG/mes/pathways/Signaling_by_GPCR.png)

<br>

![](Pathways/TG/mes/pathways/Dissolution_of_Fibrin_Clot.png)

<br>

![](Pathways/TG/mes/pathways/CHL1_interactions.png)

<br>

#### TG_epi

Here is the link to the TG_epi html file. [html](Pathways/TG/epi/TG_epi/AnalysisReport.html)

Here is the link to the TG_epi result file. [result](Pathways/TG/epi/TG_epi/metascape_result.xlsx)

![](Pathways/TG/epi/pathways/IGFBPs.png)

<br>

![](Pathways/TG/epi/pathways/Non_integrin_membrane_ECM_interactions.png)

<br>

![](Pathways/TG/epi/pathways/Cell_junction_organization.png)

<br>

![](Pathways/TG/epi/pathways/O_linked_glycosylation.png)

<br>

![](Pathways/TG/epi/pathways/Signaling_by_Receptor_Tyrosine_Kinases.png)

<br>

#### TN_mes

Here is the link to the TN_mes html file. [html](Pathways/TN/mes/TN_mes/AnalysisReport.html)

Here is the link to the TN_mes result file. [result](Pathways/TN/mes/TN_mes/metascape_result.xlsx)

![](Pathways/TN/mes/pathways/Non_integrin_membrane_ECM_interactions.png)

<br>

![](Pathways/TN/mes/pathways/IGFBPs.png)

<br>

![](Pathways/TN/mes/pathways/Signaling_by_Receptor_Tyrosine_Kinases.png)

<br>

![](Pathways/TN/mes/pathways/Diseases_of_glycosylation.png)

<br>

![](Pathways/TN/mes/pathways/Glycosaminoglycan_metabolism.png)

<br>

![](Pathways/TN/mes/pathways/Cell_junction_organization.png)

<br>

#### TN_epi

Here is the link to the TN_epi html file. [html](Pathways/TN/epi/TN_epi/AnalysisReport.html)

Here is the link to the TN_epi result file. [result](Pathways/TN/epi/TN_epi/metascape_result.xlsx)

![](Pathways/TN/epi/pathways/IGFBPs.png)

<br>

![](Pathways/TN/epi/pathways/Signaling_by_Receptor_Tyrosine_Kinases.png)

<br>

![](Pathways/TN/epi/pathways/GPCR_ligand_binding.png)

<br>

![](Pathways/TN/epi/pathways/O_linked_glycosylation_of_mucins.png)

<br>

![](Pathways/TN/epi/pathways/Cell_junction_organization.png)

<br>


#### TT_mes

Here is the link to the TT_mes html file. [html](Pathways/TT/mes/TT_mes/AnalysisReport.html)

Here is the link to the TT_mes result file. [result](Pathways/TT/mes/TT_mes/metascape_result.xlsx)

![](Pathways/TT/mes/pathways/Diseases_of_glycosylation.png)

<br>

![](Pathways/TT/mes/pathways/IGFBPs.png)

<br>

![](Pathways/TT/mes/pathways/Signaling_by_Receptor_Tyrosine_Kinases.png)

<br>

![](Pathways/TT/mes/pathways/Glycosaminoglycan_metabolism.png)

<br>

![](Pathways/TT/mes/pathways/Dissolution_of_Fibrin_Clot.png)

<br>

#### TT_epi

Here is the link to the TT_epi html file. [html](Pathways/TT/epi/TT_epi/AnalysisReport.html)

Here is the link to the TT_epi result file. [result](Pathways/TT/epi/TT_epi/metascape_result.xlsx)

![](Pathways/TT/epi/pathways/Cell_junction_organization.png)

<br>

![](Pathways/TT/epi/pathways/Diseases_of_glycosylation.png)

<br>

![](Pathways/TT/epi/pathways/Signaling_by_Receptor_Tyrosine_Kinases.png)

<br>

![](Pathways/TT/epi/pathways/Signaling_by_GPCR.png)

<br>

![](Pathways/TT/epi/pathways/MHC_class_II_antigen_presentation.png)

<br>
