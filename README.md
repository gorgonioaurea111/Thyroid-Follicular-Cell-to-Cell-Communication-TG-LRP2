# Cell-to-Cell Communication Analysis: Thyroglobulin Processing via LRP2 in Thyroid Follicular Homeostasis
## Name: Gorgonio A. Aurea lll

## Title and Biological Question
* **Title:** Autocrine and Endocrine Regulation of Thyroid Hormone Synthesis via Thyroglobulin Reuptake
* **Biological Question:** How do thyroid follicular cells use the endocytic receptor LRP2 (Megalin) to reabsorb extracellular thyroglobulin (TG) from the follicular lumen to drive thyroid hormone production and maintain endocrine homeostasis?

---

## Chosen Sender Cell and Biological Context
* **Sender Cell:** Thyroid Follicular Epithelial Cell.
* **Biological Context:** In the thyroid gland, follicular cells synthesize thyroglobulin and secrete it into the follicular lumen (colloid space). Upon endocrine stimulation, these same cells reinternalize stored thyroglobulin from the lumen via receptor-mediated endocytosis to cleave active thyroid hormones ($T_3$ and $T_4$).

---

## Candidate Ligand and Evidence for Sender-Cell Expression
* **Candidate Ligand:** Thyroglobulin (`TG` - UniProt: P01266).
* **Sender-Cell Expression Evidence:** Human Protein Atlas (HPA) immunohistochemistry and RNA sequencing data confirm that `TG` expression is extremely high and restricted to thyroid follicular cells.
* **Evidence Screenshot:** <img width="1280" height="720" alt="01_sender_cell_evidence" src="https://github.com/user-attachments/assets/fc5ef146-e9ed-4f1f-a85b-36b70fa3f263" />


---

## Receptor and Receiver Cell with Supporting Evidence
* **Receptor:** Low-Density Lipoprotein Receptor-Related Protein 2 (`LRP2` / Megalin - UniProt: P98164) and co-receptor Cubilin (`CUBN`).
* **Receiver Cell:** Thyroid Follicular Epithelial Cell (Apical Membrane Surface).
* **Supporting Evidence:** HPA and UniProt entry annotations demonstrate high transcript expression of `LRP2` on the apical membrane of thyroid epithelial cells, where it functions as a endocytic receptor for luminally stored proteins.
* **Checkpoint Sentence:** The **thyroid follicular cell** produces/presents **thyroglobulin (TG)**, which can signal through **LRP2 (megalin)** on **thyroid follicular cells** in the context of **thyroid hormone synthesis and endocrine homeostasis**.

---

## OmniPath Findings
* **Intercellular Role:** OmniPath classifies `TG` as a secreted ligand and `LRP2` as a cell-surface transmembrane endocytic receptor.
* **Signaling Link:** OmniPath curates `TG` $\rightarrow$ `LRP2` interaction records sourced from HPRD, LRdb, connectomeDB2020, and CellTalkDB.
* **Evidence Screenshot:** <img width="720" height="1280" alt="02_omnipath_evidence" src="https://github.com/user-attachments/assets/5b593838-4979-4299-a6a6-a9c26dd88618" />


---

## STRING Network Interpretation
* **Network Components (6 Proteins):** `TG` (Ligand), `LRP2` (Receptor), `LRPAP1` (Chaperone), `CUBN` (Co-receptor), `TPO` (Thyroid Peroxidase), and `TSHR` (TSH Receptor).
* **Enriched Pathway / Process:** GO Biological Process: *Receptor-mediated endocytosis* (GO:0006898) / *Thyroid hormone synthesis* (GO:0042446) with significant enrichment ($p = 6.12 \times 10^{-11}$).
* **Connecting Proteins:**
  1. `LRPAP1`: Chaperone ensuring proper folding and apical targeting of LRP2.
  2. `CUBN`: Forms dual-receptor complexes with LRP2 for high-affinity ligand uptake.
  3. `TPO`: Catalyzes iodination of TG prior to reabsorption.
* **Evidence Screenshot:** <img width="720" height="1280" alt="03_string_network" src="https://github.com/user-attachments/assets/f27fe0e1-9933-4a47-af2d-c4c54415123c" />


---

## IntAct Validation
* **Primary Pair (`TG`–`LRP2`):** Tested; no direct physical interaction record was curated in IntAct (represents an evidence-based inference).
* **Core Network Pair (`LRPAP1`–`LRP2`):** Validated with direct experimental evidence in IntAct.
* **Organism & Method:** *Homo sapiens*; validated via biophysical binding assays (SPR/pull-down).
* **Conclusion:** IntAct confirms direct physical interaction between LRP2 and its receptor chaperone LRPAP1, validating the functional network required for receptor surface availability.
* **Evidence Screenshot:** <img width="720" height="1280" alt="04_intact_evidence" src="https://github.com/user-attachments/assets/87870da2-82b6-4025-a005-e963ffff3501" />


---

## Final Model and 150–250 Word Interpretation

<img width="2440" height="3188" alt="05_final_model" src="https://github.com/user-attachments/assets/708d2f14-148c-4460-9358-67f1e03e60fd" />


> Thyroid follicular cells regulate endocrine homeostasis through the synthesis, secretion, and receptor-mediated endocytosis of thyroglobulin (TG). Human Protein Atlas immunohistochemistry confirms that TG is selectively produced and secreted into the follicular lumen by thyroid epithelial cells. OmniPath database annotations support that extracellular TG acts as an intercellular ligand targeting Low-Density Lipoprotein Receptor-Related Protein 2 (LRP2/Megalin). On the apical surface of the receiving thyroid follicular cell, LRP2 functions alongside co-receptors such as Cubilin (CUBN) to form an endocytic receptor complex. Functional network analysis in STRING demonstrates strong protein association ($p = 6.12 \times 10^{-11}$) connecting LRP2, TG, thyroid peroxidase (TPO), and receptor-associated protein (LRPAP1), highlighting enriched pathways in receptor-mediated endocytosis and thyroid hormone synthesis. IntAct experimental evidence validates the direct physical interaction between LRP2 and its chaperone LRPAP1, which is necessary for proper receptor folding and cell-surface delivery. While OmniPath cites TG–LRP2 signaling, IntAct lacks a direct curated record for this specific pair, representing an evidence-based inference. Overall, TG binding to LRP2 drives endocytosis and lysosomal degradation, yielding active thyroid hormones to maintain metabolic homeostasis.


---


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


---


## References and Database Links
* **Human Protein Atlas (HPA):** [https://www.proteinatlas.org/](https://www.proteinatlas.org/)
* **OmniPath Database:** [https://explore.omnipathdb.org/](https://explore.omnipathdb.org/)
* **STRING Database:** [https://string-db.org/](https://string-db.org/)
* **IntAct Molecular Interaction Database:** [https://www.ebi.ac.uk/intact/](https://www.ebi.ac.uk/intact/)
* **UniProt Consortium:** [https://www.uniprot.org/](https://www.uniprot.org/)
