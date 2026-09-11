## Global Treatments

After generating PCA plots to confirm distinct groupings among samples exposed to various treatments, we conducted pairwise comparisons within both the mesenchymal and epithelial datasets. Specifically, we contrasted the control group against the TGFb group, the control group against the TNFa group and the control group against the TGFb + TNFa group. Our main objective was to identify genes exhibiting notable differences under these treatment scenarios, thereby facilitating the elucidation of variations and similarities between the mesenchymal and epithelial datasets. However, we have since refined our analysis by employing the Wilcoxon test, which is better suited to our gene expression dataset, particularly in its ability to disregard lowly expressed signals.

<br>

## Workflow

In our analysis, we utilize batch-corrected count matrices as our inputs. Subsequently, each matrix undergoes filtration based on three criteria: a minimum requirement of 10 counts in some samples, a minimum total count threshold of 15, and the presence of minimum expression in 70% of samples within the smallest group. Finally, TMM normalization is performed, followed by the transformation of counts to CPM (Counts Per Million).

#### TGFb matrix

In the control and TGFb matrices, a total of 76 samples were initially present, evenly distributed with 38 samples in each group. This distribution was consistent across both the mesenchymal and epithelial datasets. Post-filtration, we preserved 12,135 genes within the mesenchymal dataset and 14,000 genes within the epithelial dataset.

![](README_Fig2/workflow_TG.png)

#### TNFa matrix

In the control and TNFa matrices, our dataset comprised 75 samples in the mesenchymal datasets (38 from the control group and 37 from the TNFa group), while in the epithelial datasets, we had 76 samples (38 from the control group and 38 from the TNFa group). Post-filtration, we retained 12,343 genes within the mesenchymal dataset and 14,011 genes within the epithelial dataset.

![](README_Fig2/workflow_TN.png)

#### the TGFb + TNFa matrix

In the control and the TGFb + TNFa matrices, our dataset comprised 76 samples in the mesenchymal datasets (38 from the control group and 38 from the combination group), while in the epithelial datasets, we had 75 samples (38 from the control group and 37 from the combination group). Post-filtration, we retained 12,328 genes within the mesenchymal dataset and 14,080 genes within the epithelial dataset.

![](README_Fig2/workflow_TT.png)

<br>

## Master spreadsheets

We've compiled comprehensive master spreadsheet excel files containing log2foldChnage, pValues, and FDR. These files serve as a centralized reference point, offering easy access to key data.

[Master_spreadsheet\_CCvsTG](Masters/Master_spreadsheet_CCvsTG.xlsx)

[Master_spreadsheet\_CCvsTN](Masters/Master_spreadsheet_CCvsTN.xlsx)

[Master_spreadsheet\_CCvsTT](Masters/Master_spreadsheet_CCvsTT.xlsx)

<br>

## CC vs TG

### Volcano plots of TG

After employing the Wilcoxon test, we proceeded to create a volcano plot comparing the control group to the TGFb group within the mesenchymal dataset and the epithelial dataset. the X-axis represents the Log2 fold change, while the Y-axis corresponds to the -Log10 adjusted p-value.

To enhance interpretability, we manually set the X-axis(Log2 fold change) threshold at an absolute value of 0.5 and adjusted the Y-axis(-Log10(FDR)) threshold to a value greater than 2 in the plots. For a comprehensive review of all pertinent details, please refer to the master spreadsheet above.

<br>

##### MES_CCvsTG

![](README_Fig2/volcano_plots/041724_mes_CCvsTG_Volcano.png)

<br>

##### EPI_CCvsTG

![](README_Fig2/volcano_plots/041724_epi_CCvsTG_Volcano.png)

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

Here is the link to the html file.[html](Masters/Pathway_analysis_CCvsTG/AnalysisReport.html)

Here is the Excel file containing the results of the pathway analysis.[metascape\_result\_CCvsTG](Masters/metascape_result_CCvsTG.xlsx)

![](README_Fig2/HeatmapSelectedGO_TG.png)

<br>

### Top 10 up\_common\_genes of TG 

![](README_Fig2/up_common_genes_TG.png)

<br>

### Top 10 down\_common\_genes of TG

![](README_Fig2/down_common_genes_TG.png)

<br>

### Top 10 up\_mes\_only\_genes of TG

![](README_Fig2/up_mes_only_genes_TG.png)

<br>

### Top 10 down\_mes\_only\_genes of TG

![](README_Fig2/down_mes_only_genes_TG.png)

<br>

### Top 10 up\_epi\_only\_genes of TG

![](README_Fig2/up_epi_only_genes_TG.png)

<br>

### Top 10 down\_epi\_only\_genes of TG

![](README_Fig2/down_epi_only_genes_TG.png)

<br>

### Top 10 up\_mes\_down\_epi\_genes of TG

![](README_Fig2/up_mes_down_epi_genes_TG.png)

<br>

### Top 10 down\_mes\_up\_epi\_genes of TG

![](README_Fig2/down_mes_up_epi_genes_TG.png)

<br>

### Scatter plots of TG

![](README_Fig2/scatter_plots/Scatterplot_TG_mes_epi_signed_logP_labels.png)

The x-axis illustrates the -log10(FDR) values for the mesenchymal dataset, while the y-axis represents the -log10(FDR) values for the epithelial dataset. Each point on the plot corresponds to an individual gene. The gradient within the central region indicates the density of genes located within those areas.

<br>

<br>

## CC vs TN

### Volcano plots of TN

We proceeded to create a volcano plot comparing the control group to the TNFa group within the mesenchymal dataset and the epithelial dataset. the X-axis represents the Log2 fold change, while the Y-axis corresponds to the -Log10 adjusted p-value.

To enhance interpretability, we manually set the X-axis(Log2 fold change) threshold at an absolute value of 0.5 and adjusted the Y-axis(-Log10(FDR)) threshold to a value greater than 2 in the plots. For a comprehensive review of all pertinent details, please refer to the master spreadsheet above.

##### MES_CCvsTN

![](README_Fig2/volcano_plots/041724_mes_CCvsTN_Volcano.png)

<br>

##### EPI_CCvsTN

![](README_Fig2/volcano_plots/041724_epi_CCvsTN_Volcano.png)

<br>

### heatmap of TN

We merged the result datasets from both the mesenchymal and epithelial analyses. Subsequently, we categorized the gene list into eight distinct groups, all of which are conveniently available in the master spreadsheet.

Here is the link to the html file.[html](Masters/Pathway_analysis_CCvsTN/AnalysisReport.html)

Here is the Excel file containing the results of the pathway analysis.[metascape\_result\_CCvsTN](Masters/metascape_result_CCvsTN.xlsx)

![](README_Fig2/HeatmapSelectedGO_TN.png)

<br>

### Top 10 up\_common\_gene of TN

![](README_Fig2/up_common_genes_TN.png)

<br>

### Top 10 down\_common\_gene of TN

![](README_Fig2/down_common_genes_TN.png)

<br>

### Top 10 up\_mes\_only\_genes of TN

![](README_Fig2/up_mes_only_genes_TN.png)

<br>

### Top 10 down\_mes\_only\_genes of TN

![](README_Fig2/down_mes_only_genes_TN.png)

<br>

### Top 10 up\_epi\_only\_genes of TN

![](README_Fig2/up_epi_only_genes_TN.png)

<br>

### Top 10 down\_epi\_only\_genes of TN

![](README_Fig2/down_epi_only_genes_TN.png)

<br>

### Top 10 up\_mes\_down\_epi\_genes of TN

![](README_Fig2/up_mes_down_epi_genes_TN.png)

<br>

### Top 10 down\_mes\_up\_epi\_genes of TN

![](README_Fig2/down_mes_up_epi_genes_TN.png)

<br>

### Scatter plots of TN

The x-axis depicts the -log10(FDR) values for mesenchymal, and the y-axis represents the -log10(FDR) values for epithelial. Each point on the plot corresponds to an individual gene. 

![](README_Fig2/scatter_plots/Scatterplot_TN_mes_epi_signed_logP_labels.png)

<br>

<br>

## CC vs TT

### Volcano plots of TT

After employing the Wilcoxon test, we proceeded to create a volcano plot comparing the control group to the TGFb group within the mesenchymal dataset and the epithelial dataset. the X-axis represents the Log2 fold change, while the Y-axis corresponds to the -Log10 adjusted p-value.

To enhance interpretability, we manually set the X-axis(Log2 fold change) threshold at an absolute value of 0.5 and adjusted the Y-axis(-Log10(FDR)) threshold to a value greater than 2 in the plots. For a comprehensive review of all pertinent details, please refer to the master spreadsheet above.

<br>

##### MES_CCvsTT

![](README_Fig2/volcano_plots/042924_mes_CCvsTT_Volcano.png)

<br>

##### EPI_CCvsTT

![](README_Fig2/volcano_plots/042924_epi_CCvsTT_Volcano.png)

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

Here is the link to the html file.[html](Masters/Pathway_analysis_CCvsTT/AnalysisReport.html)

Here is the Excel file containing the results of the pathway analysis.[metascape\_result\_CCvsTT](Masters/metascape_result_CCvsTT.xlsx)

![](README_Fig2/HeatmapSelectedGO_TT.png)

<br>

### Top 10 up\_common\_genes of TT 

![](README_Fig2/up_common_genes_TT.png)

<br>

### Top 10 down\_common\_genes of TT

![](README_Fig2/down_common_genes_TT.png)

<br>

### Top 10 up\_mes\_only\_genes of TT

![](README_Fig2/up_mes_only_TT.png)

<br>

### Top 10 down\_mes\_only\_genes of TT

![](README_Fig2/down_mes_only_TT.png)

<br>

### Top 10 up\_epi\_only\_genes of TT

![](README_Fig2/up_epi_only_TT.png)

<br>

### Top 10 down\_epi\_only\_genes of TT

![](README_Fig2/down_epi_only_TT.png)

<br>

### Top 10 up\_mes\_down\_epi\_genes of TT

![](README_Fig2/up_mes_down_epi_TT.png)

<br>

### Top 10 down\_mes\_up\_epi\_genes of TT

![](README_Fig2/down_mes_up_epi_TT.png)

<br>

### Scatter plots of TT

![](README_Fig2/scatter_plots/Scatterplot_TT_mes_epi_signed_logP_labels.png)

The x-axis illustrates the -log10(FDR) values for the mesenchymal dataset, while the y-axis represents the -log10(FDR) values for the epithelial dataset. Each point on the plot corresponds to an individual gene. The gradient within the central region indicates the density of genes located within those areas.

<br>

<br>



## Conclusion

#### CCvsTG

Based on our findings, the up common genes following treatment with TGFb exhibit a notable enrichment in hallmark TGFb signaling, hallmark TNFa signaling via NFKB, and hallmark epithelial-mesenchymal transition pathways. The epithelial dataset treated with TGFb exhibits enrichments in pathways that closely mirror those observed in the up common genes. Conversely, the mesenchymal dataset subjected to TGFb treatment displays an enrichment in Asparagine N-linked glycosylation and Vesicle-mediated transport pathways. 

<br>

#### CCvsTN

Following treatment with TNFa, the upregulated common genes demonstrate significant enrichment in hallmark TNFa signaling via NFKB, hallmark interferon gamma response, and various other signaling pathways. Similarly, the epithelial dataset treated with TNFa exhibits enrichments in pathways that closely mirror those observed in the upregulated common genes. On the other hand, the mesenchymal dataset subjected to TNFa treatment displays enrichment primarily in Vesicle-mediated transport pathways.

<br>

#### CCvsTT

After administering the TGFb + TNFa treatment, analysis reveals a pronounced enrichment of upregulated common genes in several critical pathways, notably hallmark TNFa signaling via NFKB, hallmark interferon gamma response, and the TNF signaling pathway, alongside diverse other signaling pathways. Additionally, upon examination of the heatmap, a discernible pattern emerges: upregulated gene clusters distinctly segregate from downregulated ones, indicating a clear divergence in their expression profiles.

<br>
