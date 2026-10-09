## 8. Laboratory Report & README Questions

### 1. What sender cell did you choose, and in what tissue or biological context does it act?
* **Answer:** The chosen sender cell is the **thyroid follicular epithelial cell** located in the thyroid gland. It acts in the biological context of synthesizing, iodinating, and secreting thyroglobulin into the extracellular colloid space (follicular lumen) to store precursor thyroid hormones.

### 2. What signaling molecule did you identify, and what evidence supports its production or presentation by the sender cell?
* **Answer:** The signaling molecule identified is **Thyroglobulin (`TG`)** (UniProt: P01266). Production is supported by Human Protein Atlas (HPA) immunohistochemistry and RNA sequencing data, which confirm extremely high expression and selective secretion of `TG` by thyroid follicular epithelial cells.

### 3. What receptor receives the signal, and which receiver cell did you select?
* **Answer:** The receiving receptor is **Low-Density Lipoprotein Receptor-Related Protein 2 (`LRP2` / Megalin)** acting alongside co-receptor **Cubilin (`CUBN`)**. The receiver cell is also the **thyroid follicular epithelial cell** (specifically its apical membrane facing the follicular lumen).

### 4. What type of cell-to-cell signaling is represented: paracrine, endocrine, autocrine, or contact-dependent?
* **Answer:** This represents **autocrine signaling** (with luminal storage/feedback dynamics), as the same thyroid follicular cell type produces/secretes `TG` into the lumen and subsequently reabsorbs it via apical `LRP2` receptors on its own cell surface.

### 5. Which proteins in your STRING network appear most relevant to the receptor-associated response? Explain briefly.
* **Answer:** 
  * **`LRPAP1` (Receptor-Associated Protein):** Functions as an essential molecular chaperone that ensures proper folding, maturation, and apical membrane delivery of `LRP2`.
  * **`CUBN` (Cubilin):** Forms an endocytic co-receptor complex with `LRP2` to facilitate high-affinity ligand uptake.
  * **`TPO` (Thyroid Peroxidase):** Catalyzes the iodination of `TG` prior to endocytosis, ensuring functional thyroid hormone precursors are present.

### 6. What enriched pathway or biological process is consistent with your proposed mechanism?
* **Answer:** The STRING network revealed significant enrichment ($p = 6.12 \times 10^{-11}$) for Gene Ontology terms: **Receptor-mediated endocytosis** (GO:0006898) and **Thyroid hormone synthesis** (GO:0042446).

### 7. What did IntAct show for the molecular interaction you examined? What type of evidence was reported?
* **Answer:** For the primary pair (`TG`–`LRP2`), IntAct showed no direct curated physical interaction entry. However, testing the core network pair (**`LRPAP1`–`LRP2`**) yielded a curated record in IntAct. The reported evidence supports direct physical binding (determined via biophysical binding assays such as surface plasmon resonance and pull-down assays in *Homo sapiens*).

### 8. Which parts of your final model are strongly supported, and which parts remain an inference?
* **Answer:** 
  * **Strongly Supported:** High `TG` expression in thyroid cells (HPA), `LRPAP1` physical binding to `LRP2` (IntAct), and functional network connectivity across the 6 core proteins (STRING).
  * **Inference:** The direct physical binding of extracellular `TG` to `LRP2` on the apical membrane, which is well-supported by literature annotations in OmniPath/HPRD but lacks a direct curated entry in IntAct.

### 9. What cellular response is expected in the receiver cell, and why?
* **Answer:** The expected cellular response is **apical receptor-mediated endocytosis of `TG` followed by lysosomal proteolysis and the release of active thyroid hormones ($T_3$ and $T_4$)**. This response occurs to deliver thyroid hormones into systemic circulation to regulate baseline metabolic rate and body temperature.
