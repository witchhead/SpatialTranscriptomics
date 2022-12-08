# SpatialTranscriptomics

## General structure

The code is separated into two pipelines: **Tangram_GPU** and **Tangram_CPU**. **Tangram_GPU** will be generating the map that can be used in **Tangram_CPU**. **Tangram_CPU** will be running all the experiments. The only requirement is to choose the same marker genes. 

## Tangram_GPU
### Input
Tangram_GPU only needs one input file: adata_sc(pasca.log1p_liger_med_singleR_noglyc.h5ad).
### Output
If you are using **Tangram_CPU**, you should have 2 output files: adata_st, ad_map1, ad_map2

If you are using **Tangram_CPU_Double**, you should have 3 output files: adata_st, ad_map1, ad_map2

## Tangram_CPU
### Input
**Tangram_CPU** needs 3 input files: adata_sc(pasca.log1p_liger_med_singleR_noglyc.h5ad), adata_st, ad_map

**Tangram_CPU_Double** needs 4 input files: adata_sc(pasca.log1p_liger_med_singleR_noglyc.h5ad), adata_st, ad_map1, ad_map2
### Output
Tangram_CPU pipeline has 0 output files.
