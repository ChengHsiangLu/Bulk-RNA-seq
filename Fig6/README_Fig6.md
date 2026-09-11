## Ligand-Receptor Interaction Analysis

We aim to capitalize on the availability of epithelial and mesenchymal organoids derived from the same cohort of patients and treatments. 

The objective is to explore combinations of ligands and receptor signals exhibiting noteworthy trends, such as positive or negative correlations across patients, and potentially specific patterns within fibrotic or non-fibrotic groups. We have explored potential autocrine correlations within each cell type, as well as the scenario of paracrine correlations between ligands in mesenchymal organoids and receptors in epithelial cells. As anticipated, we have identified a few examples of ligand-receptor pairs that may warrant consideration, some of which overlap with results from Part 4(Fig4).

<br>

## Workflow

Our approach comprises the following steps:

1. Select treatment groups for mesenchymal and epithelial VSD matrices.
2. Select top 300 genes from Part 4(Fig4) for NF vs F comparison.
3. Find intersection of top genes with ligand and receptor lists.
4. Generate ligand-receptor pairs from significant Part 4(Fig4) genes.
5. Manually select clear NF vs F ligand-receptor pairs.

<br>

![](README_Fig6/workflow.png)

<br>

## Ligand-Receptor pairs

I've established a folder named LR_pairs including Ligand-Receptor pairs alongside their respective Ligands and receptors.

[LR_pairs](LR_pairs/LR_pairs.csv)

[Ligands](LR_pairs/ligands.csv)

[Receptors](LR_pairs/receptors.csv)

## Scatterplots

Here is a breakdown of how to interpret each panel title. For instance, "Vmes\_epi\_correlations\_scatterplots\_panel" denotes that the X-axis (ligand) pertains to the mesenchymal group, while the Y-axis (receptor) pertains to the epithelial group. In each panel, the one marked with "**V**" represents data extracted from Part 4(Fig4). You can also locate comprehensive scatter plot panels within the directory named "**Scaterplots/Full_Scatterplots**".

### CC group

#### Vmes\_mes\_corrlations\_scatterplots\_panel

![](Scatterplots/CC/scatterplots/032724_Vmes_mes_corrlations_scatterplots_panel.png)

<br>

#### Vepi\_epi\_corrlations\_scatterplots\_panel

![](Scatterplots/CC/scatterplots/032724_Vepi_epi_corrlations_scatterplots_panel.png)

<br>

#### Vmes\_epi\_corrlations\_scatterplots\_panel

![](Scatterplots/CC/scatterplots/032724_Vmes_epi_corrlations_scatterplots_panel.png)

<br>

#### Vepi\_mes\_corrlations\_scatterplots\_panel

![](Scatterplots/CC/scatterplots/032724_Vepi_mes_corrlations_scatterplots_panel.png)

<br>

#### epi\_Vepi\_corrlations\_scatterplots\_panel

![](Scatterplots/CC/scatterplots/032724_epi_epiV_corrlations_scatterplots_panel.png)

<br>

#### mes\_Vepi\_corrlations\_scatterplots\_panel

![](Scatterplots/CC/scatterplots/032724_mes_epiV_corrlations_scatterplots_panel.png)

<br>

#### epi\_Vmes\_corrlations\_scatterplots\_panel

![](Scatterplots/CC/scatterplots/032724_epi_mesV_corrlations_scatterplots_panel.png)

<br>


### TG group

#### Vmes\_mes\_corrlations\_scatterplots\_panel

![](Scatterplots/TG/scatterplots/032724_Vmes_mes_corrlations_scatterplots_panel.png)

<br>

#### Vepi\_epi\_corrlations\_scatterplots\_panel

![](Scatterplots/TG/scatterplots/032724_Vepi_epi_corrlations_scatterplots_panel.png)

<br>

#### Vmes\_epi\_corrlations\_scatterplots\_panel

![](Scatterplots/TG/scatterplots/032724_Vmes_epi_corrlations_scatterplots_panel.png)

<br>

#### Vepi\_mes\_corrlations\_scatterplots\_panel

![](Scatterplots/TG/scatterplots/032724_Vepi_mes_corrlations_scatterplots_panel.png)

<br>

#### mes\_Vmes\_corrlations\_scatterplots\_panel

![](Scatterplots/TG/scatterplots/032724_mes_mesV_corrlations_scatterplots_panel.png)

<br>

#### epi\_Vepi\_corrlations\_scatterplots\_panel

![](Scatterplots/TG/scatterplots/032724_epi_epiV_corrlations_scatterplots_panel.png)

<br>

#### mes\_Vepi\_corrlations\_scatterplots\_panel

![](Scatterplots/TG/scatterplots/032724_mes_epiV_corrlations_scatterplots_panel.png)

<br>

#### epi\_Vmes\_corrlations\_scatterplots\_panel

![](Scatterplots/TG/scatterplots/032724_epi_mesV_corrlations_scatterplots_panel.png)

<br>


### TN group

#### Vmes\_mes\_corrlations\_scatterplots\_panel

![](Scatterplots/TN/scatterplots/032724_Vmes_mes_corrlations_scatterplots_panel.png)

<br>

#### Vepi\_epi\_corrlations\_scatterplots\_panel

![](Scatterplots/TN/scatterplots/032724_Vepi_epi_corrlations_scatterplots_panel.png)

<br>

#### Vmes\_epi\_corrlations\_scatterplots\_panel

![](Scatterplots/TN/scatterplots/032724_Vmes_epi_corrlations_scatterplots_panel.png)

<br>

#### Vepi\_mes\_corrlations\_scatterplots\_panel

![](Scatterplots/TN/scatterplots/032724_Vepi_mes_corrlations_scatterplots_panel.png)

<br>

#### mes\_Vmes\_corrlations\_scatterplots\_panel

![](Scatterplots/TN/scatterplots/032724_mes_mesV_corrlations_scatterplots_panel.png)

<br>

#### epi\_Vepi\_corrlations\_scatterplots\_panel

![](Scatterplots/TN/scatterplots/032724_epi_epiV_corrlations_scatterplots_panel.png)

<br>

#### mes\_Vepi\_corrlations\_scatterplots\_panel

![](Scatterplots/TN/scatterplots/032724_mes_epiV_corrlations_scatterplots_panel.png)

<br>

#### epi\_Vmes\_corrlations\_scatterplots\_panel

![](Scatterplots/TN/scatterplots/032724_epi_mesV_corrlations_scatterplots_panel.png)

<br>