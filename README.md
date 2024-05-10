## Polman_668_FinalProject

The attached csv file "gene_counts_data.csv" consists of varies tumor samples as the columns, and gene identified as the rows.

I wrote and attached a mapping file, "sohl_map.csv".
Sample group is the mutation.
Sample number is the assigned sampled number to the tumors.
Tumor type is the type of tumor the sample came from. 

In the Rmd file I created, the code reduces sparsity of genes that only contained zeros. 
There are two output files "trimmed_count_data.csv" and "ultratrim_count_data.csv".

"trimmed_count_data.csv" = dataset after trimming genes with only zeros and has gene lengths
"ultratrim_count_data.csv" = dataset after trimming genes with only zeros and does NOT has gene lengths

A data set without gene length numeric values was written so it does not affect the CurvCut script.

Here is the link to the CurvCut github for installation and instructions.
https://github.com/aortizsax/curvcut

After putting "ultratrim_count_data.csv" through CurvCut, there should now be an output file labeled "ultratrim_count_datatable.zerofiltered.csv".
This was then be transposed, and the transposed data set was used for CLR transformation. 

The CLR transformed data was used for PCA analysis and plotting. 
