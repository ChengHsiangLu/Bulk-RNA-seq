## WGCNA

To uncover additive interactions between TGFb and TNFa and understand their combined response, we aim to identify interactions for each gene and categorize them based on behavior. Utilizing the Weighted Gene Co-expression Network Analysis (WGCNA) facilitates exploration of subtle behaviors within the TGFb + TNFa combination response. This integrated approach allows discernment of responses from various pathways, shedding light on intricate interactions and their implications.

WGCNA primarily aims to identify co-expression patterns among genes in large-scale genomic data, revealing modules or groups of genes with similar expression patterns. 

<br>

## Master spreadsheets

We employed VSD values across all samples (16284 x 151) for both mesenchymal and epithelial groups, compiling comprehensive master spreadsheets in Excel that encompass the top 300 genes for each module. Below are the links to access these spreadsheets. 

[Master\_spreadsheet\_mes\_modules](Masters/Master_spreadsheet_mes_modules.xlsx)

[Master\_spreadsheet\_epi\_modules](Masters/Master_spreadsheet_epi_modules.xlsx)

<br>

## Eigengenes

Eigengenes serve as condensed representations of gene expression patterns within a specific group or condition. For instance, consider the eigengene of one of our modules. In the visualization, the x-axis represents the sequencing order of samples, including the control, TGFb-treated, TNFa-treated, and combination-treated groups. A dividing line delineates the plot into two sections: the non-fibrotic group on the right and the fibrotic group on the left. Notably, the control and TGFb-treated groups exhibit similar expression levels, while both the TNFa-treated and combination-treated groups demonstrate substantially higher expression levels. This observation provides valuable insights into the differential gene expression patterns induced by these treatments.

![](README_Fig3/Eigengene_example.png)

<br>

## Mesenchymal modules

### Module black

Within the black module, it is evident that TNFa predominantly influences its behavior. When the experimental conditions involve TNFa treatment, there is a notable surge in expression levels across all samples.

![](README_Fig3/module_black_mes.png)

![](README_Fig3/top3_boxplots/modules_mes_black_top_genes.png)

<br>

### Module blue

Within the blue module, it becomes apparent that TGFb has the potential to decrease the expression levels of genes. However, in the presence of TNFa alone, the expression levels remain relatively constant. Notably, when both TGFb and TNFa are introduced, there is a substantial and pronounced increase in expression levels.

![](README_Fig3/module_blue_mes.png)

![](README_Fig3/top3_boxplots/modules_mes_blue_top_genes.png)

<br>

### Module green

Within the green module, it is observed that the introduction of either TGFb or TNFa independently leads to an elevation in the expression levels of samples. Interestingly, when both TGFb and TNFa are simultaneously introduced, the combined effect seems to mitigate or neutralize the individual impacts observed when each factor is introduced separately.

![](README_Fig3/module_green_mes.png)

![](README_Fig3/top3_boxplots/modules_mes_green_top_genes.png)

<br>

### Module grey

In the grey module, a contrasting pattern emerges compared to the green module. Individually introducing TGFb or TNFa leads to a reduction in the expression levels of samples. Surprisingly, when both TGFb and TNFa are introduced simultaneously, the combined effect seems to nullify or counteract the individual downward effects observed when each factor is introduced independently.

![](README_Fig3/module_grey_mes.png)

![](README_Fig3/top3_boxplots/modules_mes_grey_top_genes.png)

<br>

### Module pink


Within the pink module, it is evident that the introduction of any treatments results in a decrease in the expression levels of samples. Notably, when TNFa is introduced in isolation, the magnitude of the decrease is particularly significant.

![](README_Fig3/module_pink_mes.png)

![](README_Fig3/top3_boxplots/modules_mes_pink_top_genes.png)

<br>

### Module red

In the red module, akin to the green module, we observe an increase in expression levels upon the addition of either TGFb or TNFa, and a decrease when both are introduced simultaneously. However, it appears that TGFb exerts a more pronounced influence compared to the addition of TNFa.

![](README_Fig3/module_red_mes.png)

![](README_Fig3/top3_boxplots/modules_mes_red_top_genes.png)

<br>

### Pathways of mesenchymal modules

Analyzing the pathway results for mesenchymal modules reveals that the black and blue modules share similar pathways, as do the green and red modules.

Here is the link to the html file. [html](Masters/Modules_pathways_mes/AnalysisReport.html)

Here is the Excel file containing results for all pathways. [Pathway\_results](Masters/Modules_pathways_mes/metascape_result.xlsx)

![](README_Fig3/pathway_modules_mes.png)

<br>

<br>

## Epithelial modules

### Module black

Within the black module, we observe an elevation in expression levels upon the introduction of any treatment. Remarkably, the combination of TGFb and TNFa produces the most substantial increment.

![](README_Fig3/module_black_epi.png)

![](README_Fig3/top3_boxplots/modules_epi_black_top_genes.png)

<br>

### Module blue

In contrast, within the blue module, we observe a reduction in expression levels upon the introduction of any treatment. Interestingly, the combination of TGFb and TNFa results in the most significant decrease.

![](README_Fig3/module_blue_epi.png)

![](README_Fig3/top3_boxplots/modules_epi_blue_top_genes.png)

<br>

### Module pink

Within the pink module, we observe an increase in expression levels upon the introduction of any treatment. Notably, TNFa appears to exert the most substantial increment in this plot.

![](README_Fig3/module_pink_epi.png)

![](README_Fig3/top3_boxplots/modules_epi_pink_top_genes.png)

<br>

### Module red

In the red module, it is clear that TNFa significantly shapes its behavior. Under experimental conditions involving TNFa treatment, a noticeable decline in expression levels is observed across all samples.

![](README_Fig3/module_red_epi.png)

![](README_Fig3/top3_boxplots/modules_epi_red_top_genes.png)

<br>

### Module turquoise

Within the turquoise module, it is evident that the primary influence on its behavior comes from the addition of TGFb. Under experimental conditions involving TGFb treatment, a noteworthy increase in expression levels is observed.

![](README_Fig3/module_turquoise_epi.png)

![](README_Fig3/top3_boxplots/modules_epi_turquoise_top_genes.png)

<br>

### Module yellow

Within the yellow module, similar to the turquoise module, it is apparent that the predominant influence on its behavior stems from the addition of TGFb. Under experimental conditions involving TGFb treatment, there is a distinct and significant increase in expression levels.

![](README_Fig3/module_yellow_epi.png)

![](README_Fig3/top3_boxplots/modules_epi_yellow_top_genes.png)

<br>

### Pathways of epithelial modules

Analyzing the pathway results for epithelial modules reveals that the black and pink modules share similar pathways, as do the turquoise and yellow modules.

Here is the link to the html file. [html](Masters/Modules_pathways_epi/AnalysisReport.html)

Here is the Excel file containing results for all pathways. [Pathway\_results](Masters/Modules_pathways_epi/metascape_result.xlsx)



![](README_Fig3/pathway_modules_epi.png)

<br>

## Conclusion

In summary, our primary objectives were to explore the combined response of the treatments and pinpoint characteristic differences between non-fibrotic and fibrotic groups. While we did not uncover substantial disparities within the non-fibrotic and fibrotic groups, our analysis did unveil 6 distinct modules for mesenchymal and epithelial datasets. These modules exhibited various effects: some contributed additively to the combined group response, while others mitigated the effects observed in either the TGFb or TNFa groups.

<br>
