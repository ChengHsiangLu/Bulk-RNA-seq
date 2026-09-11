## Global Treatments in the Fibrotic group

After generating PCA plots to confirm distinct groupings among samples exposed to various treatments, we conducted pairwise comparisons within both the mesenchymal and epithelial datasets. Specifically, we contrasted the control group against the TGFb group, the control group against the TNFa group and the control group against the TGFb + TNFa group. Our main objective was to identify genes exhibiting notable differences under these treatment scenarios, thereby facilitating the elucidation of variations and similarities between the mesenchymal and epithelial datasets. However, we have since refined our analysis by employing the Wilcoxon test, which is better suited to our gene expression dataset, particularly in its ability to disregard lowly expressed signals.

<br>

## Workflow

In our analysis, we utilize batch-corrected count matrices as our inputs. Subsequently, each matrix undergoes filtration based on three criteria: a minimum requirement of 10 counts in some samples, a minimum total count threshold of 15, and the presence of minimum expression in 70% of samples within the smallest group. Finally, TMM normalization is performed, followed by the transformation of counts to CPM (Counts Per Million).

#### TGFb matrix

In the control and TGFb matrices, a total of 40 samples were initially present, evenly distributed with 20 samples in each group. This distribution was consistent across both the mesenchymal and epithelial datasets. Post-filtration, we preserved 12,235 genes within the mesenchymal dataset and 13,922 genes within the epithelial dataset.

![](README_Fig2_Fibrotic/workflow/workflow_TG_F.png)

#### TNFa matrix

In both the control and TNFa matrices of the mesenchymal dataset, there were initially 40 samples, evenly split with 20 samples in each group. Meanwhile, the epithelial dataset initially comprised 39 samples, with 20 in the control group and 19 in the TNFa group. Following filtration, we successfully retained 12,502 genes within the mesenchymal dataset and 13,925 genes within the epithelial dataset.

![](README_Fig2_Fibrotic/workflow/workflow_TN_F.png)

#### the TGFb + TNFa matrix

In the control and the TGFb + TNFa matrices of the mesenchymal dataset, there were initially 39 samples, with 20 in the control group and 19 in the combination group. Meanwhile, the epithelial dataset initially comprised 40 samples, evenly split with 20 samples in each group. Following filtration, we successfully retained 12,502 genes within the mesenchymal dataset and 13,925 genes within the epithelial dataset.

![](README_Fig2_Fibrotic/workflow/workflow_TT_F.png)

<br>

## Master spreadsheets

We've compiled comprehensive master spreadsheet excel files containing log2foldChnage, pValues, and FDR. These files serve as a centralized reference point, offering easy access to key data.

[Master_spreadsheet\_F\_CCvsTG](Masters/Master_spreadsheet_F_CCvsTG.xlsx)

[Master_spreadsheet\_F\_CCvsTN](Masters/Master_spreadsheet_F_CCvsTN.xlsx)

[Master_spreadsheet\_F\_CCvsTT](Masters/Master_spreadsheet_F_CCvsTT.xlsx)

<br>

## CC vs TG in the Fibrotic group

### Volcano plots of TG

After employing the Wilcoxon test, we proceeded to create a volcano plot comparing the control group to the TGFb group within the mesenchymal dataset and the epithelial dataset. the X-axis represents the Log2 fold change, while the Y-axis corresponds to the -Log10 adjusted p-value.

To enhance interpretability, we manually set the X-axis(Log2 fold change) threshold at an absolute value of 0.5 and adjusted the Y-axis(-Log10(FDR)) threshold to a value greater than 2 in the plots. For a comprehensive review of all pertinent details, please refer to the master spreadsheet above.

<br>

##### MES\_F\_CCvsTG

![](README_Fig2_Fibrotic/volcano_plots/043024_mes_F_CCvsTG_Volcano.png)

<br>

##### EPI\_F\_CCvsTG

![](README_Fig2_Fibrotic/volcano_plots/043024_epi_F_CCvsTG_Volcano.png)

<br>

### Heatmap of TG

We merged the result datasets from both the mesenchymal and epithelial analyses. Subsequently, we categorized the gene list into eight distinct groups, all of which are conveniently available in the master spreadsheet.


**up\_common\_genes,**
<br>
**down\_common\_genes,**
<br>
**up\_mes\_only\_genes,**
<br>
**down\_mes\_only\_genes,**
<br>
**up\_epi\_only\_genes,**
<br>
**down\_eip\_only\_genes,**
<br>
**up\_mes\_down\_epi\_genes,**
<br>
**down\_mes\_up\_epi\_genes.**


In each group, we selected and analyzed a subset of 200 to 400 genes using pathway analysis.

Here is the link to the html file.[html](Masters/Pathway_analysis_F_CCvsTG/AnalysisReport.html)

Here is the Excel file containing the results of the pathway analysis.[metascape\_result\_F\_CCvsTG](Masters/metascape_result_F_CCvsTG.xlsx)

![](README_Fig2_Fibrotic/HeatmapSelectedGO_F_CCvsTG.png)

<br>

### Top 10 up\_common\_genes of TG 

![](README_Fig2_Fibrotic/up_common_genes_F_CCvsTG.png)

<br>

### Top 10 down\_common\_genes of TG

![](README_Fig2_Fibrotic/down_common_genes_F_CCvsTG.png)

<br>

### Top 10 up\_mes\_only\_genes of TG

![](README_Fig2_Fibrotic/up_mes_only_genes_F_CCvsTG.png)

<br>

### Top 10 down\_mes\_only\_genes of TG

![](README_Fig2_Fibrotic/down_mes_only_genes_F_CCvsTG.png)

<br>

### Top 10 up\_epi\_only\_genes of TG

![](README_Fig2_Fibrotic/up_epi_only_genes_F_CCvsTG.png)

<br>

### Top 10 down\_epi\_only\_genes of TG

![](README_Fig2_Fibrotic/down_epi_only_genes_F_CCvsTG.png)

<br>

### Top 10 up\_mes\_down\_epi\_genes of TG

![](README_Fig2_Fibrotic/up_mes_down_epi_genes_F_CCcsTG.png)

<br>

### Top 10 down\_mes\_up\_epi\_genes of TG

![](README_Fig2_Fibrotic/down_mes_up_epi_genes_F_CCcsTG.png)

<br>

### Scatter plots of TG

![](README_Fig2_Fibrotic/scatter_plots/Scatterplot_F_CCvsTG_mes_epi_signed_logP_labels.png)

The x-axis illustrates the -log10(FDR) values for the mesenchymal dataset, while the y-axis represents the -log10(FDR) values for the epithelial dataset. Each point on the plot corresponds to an individual gene. The gradient within the central region indicates the density of genes located within those areas.

<br>

<br>

## CC vs TN in the Fibrotic group

### Volcano plots of TN

We proceeded to create a volcano plot comparing the control group to the TNFa group within the mesenchymal dataset and the epithelial dataset. the X-axis represents the Log2 fold change, while the Y-axis corresponds to the -Log10 adjusted p-value.

To enhance interpretability, we manually set the X-axis(Log2 fold change) threshold at an absolute value of 0.5 and adjusted the Y-axis(-Log10(FDR)) threshold to a value greater than 2 in the plots. For a comprehensive review of all pertinent details, please refer to the master spreadsheet above.

##### MES_CCvsTN

![](README_Fig2_Fibrotic/volcano_plots/043024_mes_F_CCvsTN_Volcano.png)

<br>

##### EPI_CCvsTN

![](README_Fig2_Fibrotic/volcano_plots/043024_epi_F_CCvsTN_Volcano.png)

<br>

### heatmap of TN

We merged the result datasets from both the mesenchymal and epithelial analyses. Subsequently, we categorized the gene list into eight distinct groups, all of which are conveniently available in the master spreadsheet.

Here is the link to the html file.[html](Masters/Pathway_analysis_F_CCvsTN/AnalysisReport.html)

Here is the Excel file containing the results of the pathway analysis.[metascape\_result\_F\_CCvsTN](Masters/metascape_result_F_CCvsTN.xlsx)

![](README_Fig2_Fibrotic/HeatmapSelectedGO_F_CCvsTN.png)

<br>

### Top 10 up\_common\_gene of TN

![](README_Fig2_Fibrotic/up_common_genes_F_CCvsTN.png)

<br>

### Top 10 down\_common\_gene of TN

![](README_Fig2_Fibrotic/down_common_genes_F_CCvsTN.png)

<br>

### Top 10 up\_mes\_only\_genes of TN

![](README_Fig2_Fibrotic/up_mes_only_genes_F_CCvsTN.png)

<br>

### Top 10 down\_mes\_only\_genes of TN

![](README_Fig2_Fibrotic/down_mes_only_genes_F_CCvsTN.png)

<br>

### Top 10 up\_epi\_only\_genes of TN

![](README_Fig2_Fibrotic/up_epi_only_genes_F_CCvsTN.png)

<br>

### Top 10 down\_epi\_only\_genes of TN

![](README_Fig2_Fibrotic/down_epi_only_genes_F_CCvsTN.png)

<br>

### Top 10 up\_mes\_down\_epi\_genes of TN

![](README_Fig2_Fibrotic/up_mes_down_epi_genes_F_CCcsTN.png)

<br>

### Top 10 down\_mes\_up\_epi\_genes of TN

![](README_Fig2_Fibrotic/down_mes_up_epi_genes_F_CCcsTN.png)

<br>

### Scatter plots of TN

The x-axis depicts the -log10(FDR) values for mesenchymal, and the y-axis represents the -log10(FDR) values for epithelial. Each point on the plot corresponds to an individual gene. 

![](README_Fig2_Fibrotic/scatter_plots/Scatterplot_F_CCvsTN_mes_epi_signed_logP_labels.png)

<br>

<br>

## CC vs TT in the Fibrotic group

### Volcano plots of TT

After employing the Wilcoxon test, we proceeded to create a volcano plot comparing the control group to the TGFb group within the mesenchymal dataset and the epithelial dataset. the X-axis represents the Log2 fold change, while the Y-axis corresponds to the -Log10 adjusted p-value.

To enhance interpretability, we manually set the X-axis(Log2 fold change) threshold at an absolute value of 0.5 and adjusted the Y-axis(-Log10(FDR)) threshold to a value greater than 2 in the plots. For a comprehensive review of all pertinent details, please refer to the master spreadsheet above.

<br>

##### MES_CCvsTT

![](README_Fig2_Fibrotic/volcano_plots/043024_mes_F_CCvsTT_Volcano.png)

<br>

##### EPI_CCvsTT

![](README_Fig2_Fibrotic/volcano_plots/043024_epi_F_CCvsTT_Volcano.png)

<br>

### Heatmap of TT

We merged the result datasets from both the mesenchymal and epithelial analyses. Subsequently, we categorized the gene list into eight distinct groups, all of which are conveniently available in the master spreadsheet.


**up\_common\_genes,**
<br>
**down\_common\_genes,**
<br>
**up\_mes\_only\_genes,**
<br>
**down\_mes\_only\_genes,**
<br>
**up\_epi\_only\_genes,**
<br>
**down\_eip\_only\_genes,**
<br>
**up\_mes\_down\_epi\_genes,**
<br>
**down\_mes\_up\_epi\_genes.**


In each group, we selected and analyzed a subset of 200 to 400 genes using pathway analysis.

Here is the link to the html file.[html](Masters/Pathway_analysis_F_CCvsTT/AnalysisReport.html)

Here is the Excel file containing the results of the pathway analysis.[metascape\_result\_CCvsTT](Masters/metascape_result_F_CCvsTT.xlsx)

![](README_Fig2_Fibrotic/HeatmapSelectedGO_F_CCvsTT.png)

<br>

### Top 10 up\_common\_genes of TT 

![](README_Fig2_Fibrotic/up_common_genes_F_CCvsTT.png)

<br>

### Top 10 down\_common\_genes of TT

![](README_Fig2_Fibrotic/down_common_genes_F_CCvsTT.png)

<br>

### Top 10 up\_mes\_only\_genes of TT

![](README_Fig2_Fibrotic/up_mes_only_genes_F_CCvsTT.png)

<br>

### Top 10 down\_mes\_only\_genes of TT

![](README_Fig2_Fibrotic/down_mes_only_genes_F_CCvsTT.png)

<br>

### Top 10 up\_epi\_only\_genes of TT

![](README_Fig2_Fibrotic/up_epi_only_genes_F_CCvsTT.png)

<br>

### Top 10 down\_epi\_only\_genes of TT

![](README_Fig2_Fibrotic/down_epi_only_genes_F_CCvsTT.png)

<br>

### Top 10 up\_mes\_down\_epi\_genes of TT

![](README_Fig2_Fibrotic/up_mes_down_epi_genes_F_CCcsTT.png)

<br>

### Top 10 down\_mes\_up\_epi\_genes of TT

![](README_Fig2_Fibrotic/down_mes_up_epi_genes_F_CCcsTT.png)

<br>

### Scatter plots of TT

![](README_Fig2_Fibrotic/scatter_plots/Scatterplot_F_CCvsTT_mes_epi_signed_logP_labels.png)

The x-axis illustrates the -log10(FDR) values for the mesenchymal dataset, while the y-axis represents the -log10(FDR) values for the epithelial dataset. Each point on the plot corresponds to an individual gene. The gradient within the central region indicates the density of genes located within those areas.

<br>

<br>
