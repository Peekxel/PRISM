# 📊 PRISM: Perturbation Response Integration of Single-cell Measurements

Welcome to **PRISM** (**Perturbation Response Integration of Single-cell Measurements**), a collection of 28 harmonized single-cell datasets with over 5 million cells in **.h5ad** format. These datasets have been processed and integrated into a unified dataset named **PRISM**, ensuring consistency in metadata annotations. All scripts used for processing and analysis are available in the `scripts/` folder.

If you want to run **perturbation experiments** using an AI model trained on these datasets, visit [**this page**](https://peek.art/projects/heatmap/2-3). The code used to train the AI model can be found in the `AI model` folder.

## 📂 PRISM Dataset

Each dataset has been harmonized and includes standardized metadata in the `.obs` attribute with the following variables:

* **Organism**: One of the following species:
   * Humans (*Homo sapiens*)
   * Mice (*Mus musculus*)
   * Rats (*Rattus norvegicus*)
   * Zebrafish (*Danio rerio*)
   * Fruit flies (*Drosophila melanogaster*)
   * Nematodes (*Caenorhabditis elegans*)
   * Yeast (*Saccharomyces cerevisiae*)
   * Dogs (*Canis lupus familiaris*)
   * Pigs (*Sus scrofa*)
* **Cell Type**: Includes various cell types such as T cells, lung, neural, iPSC, etc.
* **CRISPR Type**: One of *CRISPRi*, *CRISPRa*, or *CRISPR KO*.
* **Cancer Type**: Categorized as melanoma, lung cancer, non-cancer, etc.
* **Conditions**: Control or test.
* **Perturbation Name**: The target gene(s), e.g., *Gene A* for single perturbations or *Gene A + Gene B* for multiple perturbations.

## 📂 Available Datasets

Below is the list of individual datasets included in PRISM, along with their respective download links:

| Dataset ID | Download Link |
|------------|--------------|
| GSE124703 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE124703) |
| GSE132080 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE132080) |
| GSE133344 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE133344) |
| GSE146194 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE146194) |
| GSE150062 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE150062) |
| GSE161824 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE161824) |
| GSE165291 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE165291) |
| GSE182308 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE182308) |
| GSE196142 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE196142) |
| GSE207360 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE207360) |
| GSE210681 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE210681) |
| GSE214844 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE214844) |
| GSE215253 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE215253) |
| GSE217812 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE217812) |
| GSE219317 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE219317) |
| GSE221321 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE221321) |
| GSE225775 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE225775) |
| GSE235325 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE235325) |
| GSE241683 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE241683) |
| GSE246714 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE246714) |
| GSE247274 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE247274) |
| GSE250378 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE250378) |
| GSE261283 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE261283) |
| GSE264667 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE264667) |
| GSE267982 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE267982) |
| GSE269596 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE269596) |
| GSE270828 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE270828) |
| GSE90063 | [🔗 Link](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE90063) |

## 📥 Download Options

You can access the data in two ways:

1. **Individual Datasets**: Download h5ad files separately based on study from [this Google Drive folder](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing).

2. **Combined Dataset**: Access all datasets combined as a single h5ad file from [this Google Drive folder](https://drive.google.com/drive/folders/1La6biPHHywSh_5eKE300eEvI0rekiqOi?usp=sharing).

## 📖 Citations

If you use PRISM or any individual datasets, please cite the original studies.

## 📬 Contributing & Contact

If you would like to add a dataset to PRISM, please submit a **merge request** with the dataset details. For any inquiries, feel free to reach out via email at **thisfaraz@peek.art**.