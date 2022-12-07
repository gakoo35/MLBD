The file is organized as follows:

- The first lines describe relevant information about the experiment and the samples, each line starts with a "!" character. Among these lines:
	- !Sample\_geo\_accession  --> Contains the identifier of the samples (should correspond exactly to the line ID_REF of the data matrix)
	- !Sample\_characteristics\_ch1  --> Contains the type of disease for each samplewhich is the variable (class) to be predicted
	- !Sample\_data\_row\_count  --> Tells the number of genes described for each sample. Usually it is the same for all samples
	
- In general, columns correspond to the samples (cases) of the experiment

- The data matrix starts at the line indicated by !series\_matrix\_table\_begin
	- Here also, the columns correspond to the samples (cases) and not to the variables (genes)
	- Subsequent lines correspond thus to the genes
	- The matrix is thus transposed wrt the common data representation

