# 📊 PRISM: Perturbation Response Integration of Single-cell Measurements

Welcome to **PRISM** (**Perturbation Response Integration of Single-cell Measurements**), a collection of 28 harmonized single-cell datasets with over 5 million cells in **.h5ad** format. These datasets have been processed and integrated into a unified dataset named **PRISM**, ensuring consistency in metadata annotations. All scripts used for processing and analysis are available in the `scripts/` folder.

If you want to run **perturbation experiments** using an AI model trained on these datasets, visit [**this page**](https://peek.art/projects/heatmap/2-3). The code used to train the AI model can be found in the `AI model` folder.

## 📂 PRISM Dataset Composition

### Organism Breakdown
The PRISM collection includes data from the following organisms:
- 🧬 **Humans** (*Homo sapiens*): 25 datasets (78.1%)
- 🐭 **Mice** (*Mus musculus*): 5 datasets (15.6%)
- 🐟 **Zebrafish** (*Danio rerio*): 1 dataset (3.1%)
- 🦠 **Human Cytomegalovirus** (HCMV): 1 dataset (3.1%)

### Cell Type Breakdown
The datasets encompass a diverse range of cell types:
- **Cancer/Leukemia Cells**: 8 datasets (including K562, THP-1, lung cancer cells)
- **Stem/Progenitor Cells**: 7 datasets (including iPSCs, embryonic stem cells, neural stem cells)
- **T Cells**: 5 datasets (including CAR-T cells, naïve, memory, and regulatory T cells)
- **Neural Cells**: 4 datasets (neurons, cortical organoids, neural progenitors)
- **Other Cell Types**: 7 datasets (including adipocytes, fibroblasts, osteoblasts, endothelial cells)

## 📂 Dataset Metadata

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
* **Cell Type**: Includes various cell types such as T Cells, Lung Cells, Neural Cells, iPSCs, etc.
* **CRISPR Type**: One of *CRISPRi*, *CRISPRa*, or *CRISPR KO*.
* **Cancer Type**: Categorized as Melanoma, Lung Cancer, Non-Cancer, etc.
* **Conditions**: Control or test.
* **Perturbation Name**: The target gene(s), e.g., *Gene A* for single perturbations or *Gene A + Gene B* for multiple perturbations.

## 📂 Available Datasets

Below is the list of individual datasets included in PRISM, along with their respective download links:

| Dataset ID | Organism | Cell Type | # of Cells | h5ad file | Original Dataset Link |
|------------|----------|-----------|------------|--------------|------------------------|
| [GSE124703](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE124703) | Humans (*Homo sapiens*) | iPSCs, Neurons | 24,960 | [Download](https://drive.google.com/file/d/1R6ZgPNC3KDj1OD48RJGPZ8hRJHDeNtU-/view?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE124703) |
| [GSE132080](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE132080) | Humans (*Homo sapiens*) | Leukemia Cells | 23,608 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE132080) |
| [GSE133344](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE133344) | Humans (*Homo sapiens*) | K562 Chronic Myelogenous Leukemia Cells | 111,445 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE133344) |
| [GSE146194](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE146194) | Humans (*Homo sapiens*) | Leukemia Cells | 259,673 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE146194) |
| [GSE150062](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE150062) | Humans (*Homo sapiens*) | iPSCs | 78,393 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE150062) |
| [GSE161824](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE161824) | Humans (*Homo sapiens*) | Lung Cancer Cells | 176,040 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE161824) |
| [GSE165291](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE165291) | Humans/HCMV | Human Foreskin Fibroblasts | 101,670 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE165291) |
| [GSE182308](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE182308) | Humans (*Homo sapiens*) | Astrocytes | 94,962 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE182308) |
| [GSE196142](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE196142) | Mice (*Mus musculus*) | B-ALL Cells | 13,220 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE196142) |
| [GSE207360](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE207360) | Mice (*Mus musculus*) | Mesenchymal Glioma Stem Cells | 12,487 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE207360) |
| [GSE210681](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE210681) | Humans (*Homo sapiens*) | Endothelial Cells | 794,783 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE210681) |
| [GSE214844](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE214844) | Mice (*Mus musculus*) | Mesenchymal Glioma Stem Cells | 12,487 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE214844) |
| [GSE215253](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE215253) | Humans (*Homo sapiens*) | Hematopoietic Stem/Progenitor Cells | 370,636 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE215253) |
| [GSE217812](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE217812) | Humans (*Homo sapiens*) | Human Preadipocyte SGBS Cells | 29,889 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE217812) |
| [GSE219317](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE219317) | Humans (*Homo sapiens*) | Cortical Organoids | 95,279 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE219317) |
| [GSE221321](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE221321) | Humans (*Homo sapiens*) | THP-1 Cells | 210,131 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE221321) |
| [GSE225775](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE225775) | Humans (*Homo sapiens*) | Glioblastoma Cells | 1,356,998 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE225775) |
| [GSE235325](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE235325) | Mice (*Mus musculus*) | Skin Cells | 303,159 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE235325) |
| [GSE241683](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE241683) | Humans (*Homo sapiens*) | CAR-T Cells | 55,213 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE241683) |
| [GSE241683](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE241683) | Humans (*Homo sapiens*) | CAR-T Cells | 204,374 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE241683) |
| [GSE241683](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE241683) | Humans (*Homo sapiens*) | T Cells | 24,483 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE241683) |
| [GSE246714](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE246714) | Zebrafish (*Danio rerio*) | Neural Stem Cells | 210,314 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE246714) |
| [GSE247274](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE247274) | Humans (*Homo sapiens*) | Multiple T Cell Types | 69,907 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE247274) |
| [GSE250378](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE250378) | Humans (*Homo sapiens*) | Neural Progenitor Cells/Neurons | 141,290 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE250378) |
| [GSE261283](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE261283) | Humans (*Homo sapiens*) | Human Fetal Osteoblast Cells | 33,038 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE261283) |
| [GSE264667](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE264667) | Humans (*Homo sapiens*) | Jurkat Cells, Hep G2 Cells | 408,429 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE264667) |
| [GSE267982](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE267982) | Mice (*Mus musculus*) | Disseminated Tumour Cells | 45,808 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE267982) |
| [GSE269596](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE269596) | Humans (*Homo sapiens*) | Embryonic Kidney Cells, Erythroleukemia Cells | 74,312 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE269596) |
| [GSE270828](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE270828) | Humans (*Homo sapiens*) | Human iPSCs, Human NSCs | 87,896 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE270828) |
| [GSE90063](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE90063) | Humans (*Homo sapiens*) | Erythroleukemia Cells | 130,150 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE90063) |
| [GSE90063](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE90063) | Mice (*Mus musculus*) | Embryonic Stem Cells | 65,840 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) | [NCBI GEO](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE90063) |

## 📥 Download Options

You can access the data in two ways:

1. **Individual Datasets**: Download h5ad files separately based on study from [this Google Drive folder](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing).

2. **Combined Dataset**: Access all datasets combined as a single h5ad file from [this Google Drive folder](https://drive.google.com/drive/folders/1La6biPHHywSh_5eKE300eEvI0rekiqOi?usp=sharing).

## 📖 Citations

If you use PRISM or any individual datasets, please cite the original studies as well as the PRISM collection:

```
@misc{PRISM,
  author = {Peekxel},
  title = {PRISM: Perturbation Response Integration of Single-cell Measurements},
  year = {2025},
  url = {https://github.com/Peekxel/PRISM},
  version = {1.0.0}
}
```

## 📬 Contributing & Contact

If you would like to add a dataset to PRISM, please submit a **merge request** with the dataset details. For any inquiries, feel free to reach out via email at **thisfaraz@peek.art**.