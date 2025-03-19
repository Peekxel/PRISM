# 📊 PRISM: Perturbation Response Integration of Single-cell Measurements

Welcome to **PRISM** (**Perturbation Response Integration of Single-cell Measurements**), a collection of over 70 harmonized single-cell datasets with over 10 million cells in **.h5ad** format. These datasets have been processed and integrated into a unified dataset named **PRISM**, ensuring consistency in metadata annotations. All scripts used for processing and analysis are available in the `Preprocessing Scripts/` folder.

If you want to run **perturbation experiments** using an AI model trained on these datasets, visit [**this page**](https://peek.art/projects/heatmap/2-3). The AI model utilizes flow matching technique and [GenePT](https://github.com/yiqunchen/GenePT) for gene embedding. The code used to train the AI model can be found in the `AI model` folder.

## 📂 PRISM Dataset Composition

### Organism Breakdown
The PRISM collection includes data from the following organisms:
* 🧬 **Humans** (*Homo sapiens*): 57 datasets (74.0%)
* 🐭 **Mice** (*Mus musculus*): 15 datasets (19.5%)
* 🐟 **Zebrafish** (*Danio rerio*): 1 dataset (1.3%)
* 🦠 **Human Cytomegalovirus** (HCMV): 1 dataset (1.3%)
* 🪰 **Drosophila melanogaster**: 1 dataset (1.3%)
* 🧫 **Mixed**: 2 datasets (2.6%)

### Cell Type Breakdown
The datasets encompass a diverse range of cell types:
* **Cancer/Leukemia Cells**: 24 datasets (including K562, THP-1, lung cancer cells)
* **Stem/Progenitor Cells**: 14 datasets (including iPSCs, embryonic stem cells, neural stem cells)
* **T Cells**: 12 datasets (including CAR-T cells, naïve, memory, and regulatory T cells)
* **Neural Cells**: 11 datasets (neurons, cortical organoids, neural progenitors)
* **Other Cell Types**: 16 datasets (including adipocytes, fibroblasts, osteoblasts, endothelial cells)

| CRISPR Type | Count | Percentage |
|-------------|-------|------------|
| CRISPR KO | 38 | 49.4% |
| CRISPRi | 28 | 36.4% |
| CRISPRa | 5 | 6.5% |
| None | 5 | 6.5% |
| Mixed/Other | 4 | 5.2% |

## Cancer Type Distribution

| Cancer Type | Count | Percentage |
|-------------|-------|------------|
| Non-Cancer | 38 | 49.4% |
| Leukemia (various types) | 15 | 19.5% |
| Multiple cancer types | 9 | 11.7% |
| Glioblastoma/Brain tumors | 4 | 5.2% |
| Colorectal cancer | 4 | 5.2% |
| Lung Cancer | 3 | 3.9% |
| Other cancer types | 7 | 9.1% |


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
* **CRISPR Type**: *CRISPRi*, *CRISPRa*, *CRISPR KO*, etc.
* **Cancer Type**: Categorized as Melanoma, Lung Cancer, Non-Cancer, etc.
* **Conditions**: IFNγ stimulated, Control, Test, etc.
* **Perturbation Name**: The target gene(s), e.g., *Gene A* for single perturbations or *Gene A + Gene B* for multiple perturbations.

## 📂 Available Datasets

Below is the list of individual datasets included in PRISM, along with their respective download links:

| Dataset ID | Organism | Cell Type | CRISPR Type | Cancer Type | Unique Conditions | Unique Perturbations | # of Cells | h5ad file |
|------------|----------|-----------|-------------|-------------|-------------------|---------------------|------------|-----------|
| [GSE124703](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE124703) | Humans (Homo sapiens) | induced pluripotent stem cell, neuron | CRISPRi | non-cancer | 2 (test, control) | 68 | 24,960 | [Download](https://drive.google.com/file/d/1R6ZgPNC3KDj1OD48RJGPZ8hRJHDeNtU-/view?usp=sharing) |
| [GSE90063_mouse](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE90063) | Mice (Mus musculus) | embryonic stem cells | CRISPR KO | non-cancer | 2 (test, control) | 1,557 | 65,840 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE132080](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE132080) | Humans (Homo sapiens) | leukemia cell | CRISPRi | Leukemia | 2 (test, control) | 27 | 23,608 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE217812](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE217812) | human adipocytes | Human Preadipocyte SGBS Cells, Adipocytes | CRISPRi | non-cancer | 2 (test, control) | 5,654 | 29,889 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE207360](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE207360) | Mice (Mus musculus) | mesenchymal glioma stem cell | CRISPR KO | Glioblastoma | 2 (test, control) | 2 | 12,487 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE214844](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE214844) | Mice (Mus musculus) | mesenchymal glioma stem cell | CRISPR KO | Glioblastoma | 2 (test, control) | 2 | 12,487 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE247274](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE247274) | Humans (Homo sapiens) | Multiple T cell types | CRISPR KO | non-cancer | 2 (test, control) | 1 | 69,907 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE241683_carT](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE241683) | Humans (Homo sapiens) | CAR T cell | CRISPR KO | non-cancer | 2 (test, control) | 2 | 55,213 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE196142](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE196142) | Mice (Mus musculus) | B-ALL cell | CRISPR KO | Leukemia | 1 (control) | 1 | 13,220 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE219317](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE219317) | Humans (Homo sapiens) | cortical organoid | CRISPR KO | non-cancer | 2 (test, control) | 2 | 95,279 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE267982](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE267982) | Mice (Mus musculus) | disseminated tumour cell | CRISPRa | Colorectal cancer | 1 (control) | 1 | 45,808 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE246714](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE246714) | Zebrafish (Danio rerio) | neural stem cells | CRISPR KO | non-cancer | 1 (control) | 1 | 210,314 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE250378-016](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE250378) | Humans (Homo sapiens) | neural progenitor cells and neurons | CRISPRi | non-cancer | 2 (test, control) | 4,867 | 141,290 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE90063_human-004](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE90063) | Humans (Homo sapiens) | erythroleukemia cell | CRISPR KO | Erythroleukemia | 2 (test, control) | 1,086 | 130,150 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE261283](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE261283) | Humans (Homo sapiens) | human fetal osteoblast 1.19 cells (hFOBs) | CRISPRi | non-cancer | 2 (test, control) | 3,883 | 33,038 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE264667](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE264667) | Humans (Homo sapiens) | Jurkat, Hep G2 | CRISPRi | T-cell Leukemia, Hepatocellular carcinoma | 2 (test, control) | 2,395 | 408,429 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE269596](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE269596) | Humans (Homo sapiens) | embryonic kidney cell, erythroleukemia | CRISPRi | non-cancer, leukemia | 2 (test, control) | 38 | 74,312 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE270828](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE270828) | Humans (Homo sapiens) | Human iPSCs, Human NSCs | CRISPRi | Non-cancer | 2 (test, control) | 166 | 87,896 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE241683_cropseq](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE241683) | Humans (Homo sapiens) | CAR T cell | CRISPR KO | non-cancer | 2 (test, control) | 187,357 | 204,374 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE241683_pilot](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE241683) | Humans (Homo sapiens) | T cell | CRISPR KO | non-cancer | 2 (test, control) | 2 | 24,483 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE235325](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE235325) | Mice (Mus musculus) | skin cell | CRISPR KO | skin squamous cell carcinoma | 2 (test, control) | 151 | 303,159 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE225775](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE225775) | Humans (Homo sapiens) | Multiple cell lines (A172, T98G, U87MG) | CRISPRi, CRISPRa (mixed) | Glioblastoma | 2 (test, control) | 83,015 | 1,356,998 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE221321](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE221321) | Humans (Homo sapiens) | THP-1 cell | CRISPR KO, CRISPRi | Leukemia | 2 (test, control) | 40,409 | 210,131 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE215253](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE215253) | Humans (Homo sapiens) | hematopoietic stem and progenitor cell | CRISPR Base Editing, CRISPR KO | non-cancer | 1 (test) | 3 | 370,636 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE210681](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE210681) | Humans (Homo sapiens) | Endothelial Cells | CRISPRi | Non-cancer | 2 (test, control) | 2,621 | 794,783 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE182308](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE182308) | Humans (Homo sapiens) | astrocytes | CRISPRi | non-cancer | 2 (test, control) | 18,839 | 94,962 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE165291](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE165291) | Humans (Homo sapiens), Human Cytomegalovirus (HCMV) | human foreskin fibroblasts (HFFs) | CRISPRi, CRISPRn | non-cancer | 2 (test, control) | 96 | 101,670 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE161824](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE161824) | Humans (Homo sapiens) | lung cancer cell | CRISPRa | Lung | 2 (test, control) | 1,994 | 176,040 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE150062](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE150062) | Humans (Homo sapiens) | iPSCs (induced pluripotent stem cells) | CRISPRi | non-cancer | 2 (test, control) | 241 | 78,393 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE146194](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE146194) | Humans (Homo sapiens) | leukemia cell | CRISPRi, CRISPRa | Leukemia | 2 (test, control) | 373 | 259,673 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE133344](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE133344) | Humans (Homo sapiens) | K562 chronic myelogenous leukemia cell | CRISPRi | Leukemiaa | 2 (test, control) | 108 | 111,445 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE252589](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE252589) | Mus musculus | 143B | None | Osteosarcoma | 2 (Control, Test) | 2 | 23,297 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE283614](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE283614) | Homo sapiens | Embryonic Stem Cells | CRISPR KO | Non-Cancer | 2 (Test, Control) | 2 | 12,844 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE278572](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE278572) | Homo sapiens | CD4+ T Cells | CRISPRi | Non-Cancer | 2 (Test, Control) | 4,712 | 249,799 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE274751](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE274751) | Homo sapiens | Multiple T cell types | CRISPR KO | Non-Cancer | 1 (Test) | 32,178 | 173,018 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE254100](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE254100) | Mus musculus | Tracheal Epithelial Cells | none | Non-Cancer | 2 (test, control) | 4 | 21,667 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE261025](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE261025) | Homo sapiens | Hepatocyte | None, CRISPRi | Non-Cancer | 2 (Control, Test) | 349 | 69,977 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE220974](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE220974) | Homo sapiens | K562 | CRISPRa, CRISPRi, CRISPRai | Leukemia | 2 (test, control) | 48 | 24,661 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE247599](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE247599) | Homo sapiens | Jurkat T Cells | CRISPR KO | T-cell leukemia | 2 (Test, Control) | 814 | 24,435 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE273271](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE273271) | Mus musculus | Neural Cells | None | Non-Cancer | 2 (Test, Control) | 2 | 145,082 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE247598](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE247598) | Homo sapiens | Pancreatic cells | CRISPR KO | Non-Cancer | 1 (Control) | 1 | 24,491 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE153056](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE153056) | Homo sapiens | THP-1 | CRISPR KO | Leukemia | 2 (Test, Control) | 26 | 20,729 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE120861](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE120861) | Homo sapiens | K562 | CRISPRi | Chronic myelogenous leukemia | 2 (Test, Control) | 104,973 | 174,711 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE225807](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE225807) | Homo sapiens | K562 | CRISPRi | Leukemia | 2 (Control, Test) | 95 | 17,424 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE236304](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE236304) | Homo sapiens | A549 | CRISPRi | Lung Cancer | 2 (test, control) | 13,209 | 25,220 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE250558](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE250558) | Homo sapiens | HEK293 | CRISPR KO | Non-Cancer | 2 (Test, Control) | 24 | 59,837 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE281048_TGFB_Perturb_seq](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE281048) | Homo sapiens | Multiple cell lines | CRISPR KO | Multiple cancer types | 2 (Test, Control) | 53 | 236,606 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE251715](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE251715) | Drosophila melanogaster | Multiple renal cell types | CRISPRa | Gut Tumor, Non-Cancer | 2 (Test, Control) | 3 | 21,371 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE281048_INS_Perturb_seq](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE281048) | Homo sapiens | Multiple cell lines | CRISPR KO | Multiple cancer types | 2 (Test, Control) | 45 | 431,457 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE281048_TNFA_Perturb_seq](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE281048) | Homo sapiens | Multiple cell lines | CRISPR KO | Multiple cancer types | 2 (Test, Control) | 56 | 386,631 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE281048_IFNG_Perturb_seq](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE281048) | Homo sapiens | Multiple cell lines | CRISPR KO | Multiple cancer types | 2 (Test, Control) | 60 | 245,240 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE281048_IFNB_Perturb_seq](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE281048) | Homo sapiens | Multiple cell lines | CRISPR KO | Multiple cancer types | 2 (Test, Control) | 62 | 328,542 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE208240](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE208240) | Homo sapiens | Lung epithelial cells | CRISPRi | Lung Cancer | 2 (test, control) | 25,728 | 73,989 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE205310](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE205310) | Homo sapiens | K562 | CRISPRi | Chronic myelogenous leukemia | 2 (test, control) | 151 | 124,963 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE197452_Perturb-seq](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE197452) | Homo sapiens | K562 | CRISPR KO, None | Leukemia | 3 (test, control, unknown) | 1,853 | 20,811 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE213921](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE213921) | Mus musculus | CD8+ T Cells | CRISPR KO | EG.7-OVA tumor | 2 (test, Control) | 34 | 9,797 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE243244](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE243244) | Mus musculus | Multiple cell types | CRISPR KO | Non-Cancer, Melanoma | 2 (Test, Control) | 3,406 | 48,587 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE203592](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE203592) | Mus musculus | CD8+ tumor infiltrating T cells | CRISPR KO | Colon Cancer | 2 (test, control) | 11 | 70,646 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE229505](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE229505) | Homo sapiens | Human foreskin fibroblast | CRISPR KO | Non-Cancer | 2 (Unstimulated, IFNγ stimulated) | 20 | 126,495 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE206107](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE206107) | Mus musculus | MC38 colon cancer cells | CRISPR KO | Colon Cancer | 2 (Test, Control) | 23 | 51,055 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE213511](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE213511) | Mice (Mus musculus) | Multiple blood cell lineages | CRISPR KO | Non-Cancer, Leukemia | 3 (Test, Control, Unknown) | 59 | 181,177 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE212396](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE212396) | Homo sapiens | Endothelial cells | CRISPRi | Non-Cancer | 2 (Test, Control) | 311 | 103,155 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE255832](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE255832) | Mus musculus | CD8+ T cells | CRISPR KO | Pancreatic cancer | 3 (IgG control, anti-PD-1, Control) | 2,576 | 27,912 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE236519](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE236519) | Mus musculus | Multiple neural cell types | CRISPRi, CRISPR KO | Non-Cancer | 2 (test, control) | 32 | 98,883 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE272093](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE272093) | Homo sapiens | Neurons, Mixed (Neurons, Astrocytes, Microglia) | CRISPRi | Non-Cancer | 1 (Test) | 128,770 | 241,187 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE282731](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE282731) | Mus musculus | Neocortex cells | CRISPR KO | Non-Cancer | 2 (Test, Control) | 3 | 113,874 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE236057](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE236057) | Homo sapiens | Astrocyte | CRISPRi | Non-Cancer | 2 (Test, Control) | 5,086 | 15,866 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE263747](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE263747) | Homo sapiens | SNU-761 liver cancer cells | CRISPR KO | Liver Cancer | 3 (day5, day10, Control) | 110 | 44,178 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE272457](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE272457) | Mixed, Homo sapiens, Mus musculus | Mixed, NIH3T3, HEK293T | CRISPRi | Non-Cancer | 1 (Control) | 1 | 82,731 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE164996](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE164996) | Homo sapiens | MCF10A | CRISPR KO | Non-Cancer | 2 (Test, Control) | 398 | 25,794 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE190604](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE190604) | Homo sapiens | T Cells | CRISPRa | Non-Cancer | 2 (Test, Control) | 8,466 | 103,805 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE263524](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE263524) | Mus musculus | MC38 tumor cell | CRISPR KO | Colorectal cancer | 2 (Knockout, Control) | 2 | 42,289 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE195510](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE195510) | Homo sapiens | iPSC-derived forebrain organoid cells | CRISPR KO | Non-Cancer | 2 (Test, Control) | 2 | 140,709 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE261157](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE261157) | Homo sapiens | Multiple neural cell types | None | Non-Cancer | 3 (Control, AxD_Cerebral, AxD_Cortical) | 2 | 30,656 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE216673](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE216673) | Homo sapiens | Microglia | CRISPR KO | Non-Cancer | 2 (Control, Test) | 2 | 55,156 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE221882](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE221882) | Homo sapiens | iPSC-derived cortical organoid | None, CRISPR_correction | Non-Cancer | 2 (Test, Control) | 2 | 25,241 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |
| [GSE280767](https://www.ncbi.nlm.nih.gov/geo/query/acc.cgi?acc=GSE280767) | Homo sapiens | T Cells, Huh7 | CRISPR Cas9, ABE, ABE-V106W | Non-Cancer, Hepatocellular carcinoma | 5 (Unknown, Control, Day 3, Day 7, Day 21) | 3 | 246,027 | [Download](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing) |.cgi?acc# PRISM: Perturbation Response Integration of Single-cell Measurements


## 📥 Download Options

You can access the data from the link provided below:

**Individual Datasets**: Download h5ad files separately based on study from [this Google Drive folder](https://drive.google.com/drive/folders/1Y0Z19JhiTmTch65kvBNNMdVtosH6QHfi?usp=sharing).


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
