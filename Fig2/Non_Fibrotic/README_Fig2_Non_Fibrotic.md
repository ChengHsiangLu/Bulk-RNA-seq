## Global Treatments in the Non-Fibrotic group

After generating PCA plots to confirm distinct groupings among samples exposed to various treatments, we conducted pairwise comparisons within both the mesenchymal and epithelial datasets. Specifically, we contrasted the control group against the TGFb group, the control group against the TNFa group and the control group against the TGFb + TNFa group. Our main objective was to identify genes exhibiting notable differences under these treatment scenarios, thereby facilitating the elucidation of variations and similarities between the mesenchymal and epithelial datasets. However, we have since refined our analysis by employing the Wilcoxon test, which is better suited to our gene expression dataset, particularly in its ability to disregard lowly expressed signals.

<br>

## Workflow

In our analysis, we utilize batch-corrected count matrices as our inputs. Subsequently, each matrix undergoes filtration based on three criteria: a minimum requirement of 10 counts in some samples, a minimum total count threshold of 15, and the presence of minimum expression in 70% of samples within the smallest group. Finally, TMM normalization is performed, followed by the transformation of counts to CPM (Counts Per Million).

#### TGFb matrix

In the control and TGFb matrices, a total of 36 samples were initially present, evenly distributed with 18 samples in each group. This distribution was consistent across both the mesenchymal and epithelial datasets. Post-filtration, we preserved 12,024 genes within the mesenchymal dataset and 13,966 genes within the epithelial dataset.

![](README_Fig2_Non_Fibrotic/workflow/workflow_TG_NF.png)

#### TNFa matrix

In the control and TNFa matrices, a total of 36 samples were initially present, evenly distributed with 18 samples in each group. This distribution was consistent across both the mesenchymal and epithelial datasets. Post-filtration, we retained 12,125 genes within the mesenchymal dataset and 13,969 genes within the epithelial dataset.

![](README_Fig2_Non_Fibrotic/workflow/workflow_TN_NF.png)

#### the TGFb + TNFa matrix

In the control and the TGFb + TNFa matrices, a total of 36 samples were initially present, evenly distributed with 18 samples in each group. Post-filtration, we retained 12,201 genes within the mesenchymal dataset and 14,004 genes within the epithelial dataset.

![](README_Fig2_Non_Fibrotic/workflow/workflow_TT_NF.png)

<br>

## Master spreadsheets

We've compiled comprehensive master spreadsheet excel files containing log2foldChnage, pValues, and FDR. These files serve as a centralized reference point, offering easy access to key data.

[Master_spreadsheet\_NF\_CCvsTG](Masters/Master_spreadsheet_NF_CCvsTG.xlsx)

[Master_spreadsheet\_NF\_CCvsTN](Masters/Master_spreadsheet_NF_CCvsTN.xlsx)

[Master_spreadsheet\_NF\_CCvsTT](Masters/Master_spreadsheet_NF_CCvsTT.xlsx)

<br>

## CC vs TG in the Non-Fibrotic group

### Volcano plots of TG

After employing the Wilcoxon test, we proceeded to create a volcano plot comparing the control group to the TGFb group within the mesenchymal dataset and the epithelial dataset. the X-axis represents the Log2 fold change, while the Y-axis corresponds to the -Log10 adjusted p-value.

To enhance interpretability, we manually set the X-axis(Log2 fold change) threshold at an absolute value of 0.5 and adjusted the Y-axis(-Log10(FDR)) threshold to a value greater than 2 in the plots. For a comprehensive review of all pertinent details, please refer to the master spreadsheet above.

<br>

##### MES\_NF\_CCvsTG

![](README_Fig2_Non_Fibrotic/volcano_plots/043024_mes_NF_CCvsTG_Volcano.png)

<br>

##### EPI\_NF\_CCvsTG

![](README_Fig2_Non_Fibrotic/volcano_plots/043024_epi_NF_CCvsTG_Volcano.png)

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

Here is the link to the html file.[html](Masters/Pathway_analysis_NF_CCvsTG/AnalysisReport.html)

Here is the Excel file containing the results of the pathway analysis.[metascape\_result\_NF\_CCvsTG](Masters/metascape_result_NF_CCvsTG.xlsx)

![](README_Fig2_Non_Fibrotic/HeatmapSelectedGO_NF_CCvsTG.png)

<br>

### Top 10 up\_common\_genes of TG 

![](README_Fig2_Non_Fibrotic/up_common_genes_NF_CCvsTG.png)

<br>

### Top 10 down\_common\_genes of TG

![](README_Fig2_Non_Fibrotic/down_common_genes_NF_CCvsTG.png)

<br>

### Top 10 up\_mes\_only\_genes of TG

![](README_Fig2_Non_Fibrotic/up_mes_only_genes_NF_CCvsTG.png)

<br>

### Top 10 down\_mes\_only\_genes of TG

![](README_Fig2_Non_Fibrotic/down_mes_only_genes_NF_CCvsTG.png)

<br>

### Top 10 up\_epi\_only\_genes of TG

![](README_Fig2_Non_Fibrotic/up_epi_only_genes_NF_CCvsTG.png)

<br>

### Top 10 down\_epi\_only\_genes of TG

![](README_Fig2_Non_Fibrotic/down_epi_only_genes_NF_CCvsTG.png)

<br>

### Top 10 up\_mes\_down\_epi\_genes of TG

![](README_Fig2_Non_Fibrotic/up_mes_down_epi_genes_NF_CCcsTG.png)

<br>

### Top 10 down\_mes\_up\_epi\_genes of TG

![](README_Fig2_Non_Fibrotic/down_mes_up_epi_genes_NF_CCcsTG.png)

<br>

### Scatter plots of TG

![](README_Fig2_Non_Fibrotic/scatter_plots/Scatterplot_NF_CCvsTG_mes_epi_signed_logP_labels.png)

The x-axis illustrates the -log10(FDR) values for the mesenchymal dataset, while the y-axis represents the -log10(FDR) values for the epithelial dataset. Each point on the plot corresponds to an individual gene. The gradient within the central region indicates the density of genes located within those areas.

<br>

<br>

## CC vs TN in the Non-Fibrotic group

### Volcano plots of TN

We proceeded to create a volcano plot comparing the control group to the TNFa group within the mesenchymal dataset and the epithelial dataset. the X-axis represents the Log2 fold change, while the Y-axis corresponds to the -Log10 adjusted p-value.

To enhance interpretability, we manually set the X-axis(Log2 fold change) threshold at an absolute value of 0.5 and adjusted the Y-axis(-Log10(FDR)) threshold to a value greater than 2 in the plots. For a comprehensive review of all pertinent details, please refer to the master spreadsheet above.

##### MES_CCvsTN

![](README_Fig2_Non_Fibrotic/volcano_plots/043024_mes_NF_CCvsTN_Volcano.png)

<br>

##### EPI_CCvsTN

![](README_Fig2_Non_Fibrotic/volcano_plots/043024_epi_NF_CCvsTN_Volcano.png)

<br>

### heatmap of TN

We merged the result datasets from both the mesenchymal and epithelial analyses. Subsequently, we categorized the gene list into eight distinct groups, all of which are conveniently available in the master spreadsheet.

Here is the link to the html file.[html](Masters/Pathway_analysis_NF_CCvsTN/AnalysisReport.html)

Here is the Excel file containing the results of the pathway analysis.[metascape\_result\_NF\_CCvsTN](Masters/metascape_result_NF_CCvsTN.xlsx)

![](README_Fig2_Non_Fibrotic/HeatmapSelectedGO_NF_CCvsTN.png)

<br>

### Top 10 up\_common\_gene of TN

![](README_Fig2_Non_Fibrotic/up_common_genes_NF_CCvsTN.png)

<br>

### Top 10 down\_common\_gene of TN

![](README_Fig2_Non_Fibrotic/down_common_genes_NF_CCvsTN.png)

<br>

### Top 10 up\_mes\_only\_genes of TN

![](README_Fig2_Non_Fibrotic/up_mes_only_genes_NF_CCvsTN.png)

<br>

### Top 10 down\_mes\_only\_genes of TN

![](README_Fig2_Non_Fibrotic/down_mes_only_genes_NF_CCvsTN.png)

<br>

### Top 10 up\_epi\_only\_genes of TN

![](README_Fig2_Non_Fibrotic/up_epi_only_genes_NF_CCvsTN.png)

<br>

### Top 10 down\_epi\_only\_genes of TN

![](README_Fig2_Non_Fibrotic/down_epi_only_genes_NF_CCvsTN.png)

<br>

### Top 10 up\_mes\_down\_epi\_genes of TN

![](README_Fig2_Non_Fibrotic/up_mes_down_epi_genes_NF_CCcsTN.png)

<br>

### Top 10 down\_mes\_up\_epi\_genes of TN

![](README_Fig2_Non_Fibrotic/down_mes_up_epi_genes_NF_CCcsTN.png)

<br>

### Scatter plots of TN

The x-axis depicts the -log10(FDR) values for mesenchymal, and the y-axis represents the -log10(FDR) values for epithelial. Each point on the plot corresponds to an individual gene. 

![](README_Fig2_Non_Fibrotic/scatter_plots/Scatterplot_NF_CCvsTN_mes_epi_signed_logP_labels.png)

<br>

<br>

## CC vs TT in the Non-Fibrotic group

### Volcano plots of TT

After employing the Wilcoxon test, we proceeded to create a volcano plot comparing the control group to the TGFb group within the mesenchymal dataset and the epithelial dataset. the X-axis represents the Log2 fold change, while the Y-axis corresponds to the -Log10 adjusted p-value.

To enhance interpretability, we manually set the X-axis(Log2 fold change) threshold at an absolute value of 0.5 and adjusted the Y-axis(-Log10(FDR)) threshold to a value greater than 2 in the plots. For a comprehensive review of all pertinent details, please refer to the master spreadsheet above.

<br>

##### MES_CCvsTT

![](README_Fig2_Non_Fibrotic/volcano_plots/043024_mes_NF_CCvsTT_Volcano.png)

<br>

##### EPI_CCvsTT

![](README_Fig2_Non_Fibrotic/volcano_plots/043024_epi_NF_CCvsTT_Volcano.png)

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

Here is the link to the html file.[html](Masters/Pathway_analysis_NF_CCvsTT/AnalysisReport.html)

Here is the Excel file containing the results of the pathway analysis.[metascape\_result\_CCvsTT](Masters/metascape_result_CCvsTT.xlsx)

![](README_Fig2_Non_Fibrotic/HeatmapSelectedGO_NF_CCvsTT.png)

<br>

### Top 10 up\_common\_genes of TT 

![](README_Fig2_Non_Fibrotic/up_common_genes_NF_CCvsTT.png)

<br>

### Top 10 down\_common\_genes of TT

![](README_Fig2_Non_Fibrotic/down_common_genes_NF_CCvsTT.png)

<br>

### Top 10 up\_mes\_only\_genes of TT

![](README_Fig2_Non_Fibrotic/up_mes_only_genes_NF_CCvsTT.png)

<br>

### Top 10 down\_mes\_only\_genes of TT

![](README_Fig2_Non_Fibrotic/down_mes_only_genes_NF_CCvsTT.png)

<br>

### Top 10 up\_epi\_only\_genes of TT

![](README_Fig2_Non_Fibrotic/up_epi_only_genes_NF_CCvsTT.png)

<br>

### Top 10 down\_epi\_only\_genes of TT

![](README_Fig2_Non_Fibrotic/down_epi_only_genes_NF_CCvsTT.png)

<br>

### Top 10 up\_mes\_down\_epi\_genes of TT

![](README_Fig2_Non_Fibrotic/up_mes_down_epi_genes_NF_CCcsTT.png)

<br>

### Top 10 down\_mes\_up\_epi\_genes of TT

![](README_Fig2_Non_Fibrotic/down_mes_up_epi_genes_NF_CCcsTT.png)

<br>

### Scatter plots of TT

![](README_Fig2_Non_Fibrotic/scatter_plots/Scatterplot_NF_CCvsTT_mes_epi_signed_logP_labels.png)

The x-axis illustrates the -log10(FDR) values for the mesenchymal dataset, while the y-axis represents the -log10(FDR) values for the epithelial dataset. Each point on the plot corresponds to an individual gene. The gradient within the central region indicates the density of genes located within those areas.

<br>

<br>
