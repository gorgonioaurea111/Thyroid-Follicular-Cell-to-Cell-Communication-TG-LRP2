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

## References and Database Links
* **Human Protein Atlas (HPA):** [https://www.proteinatlas.org/](https://www.proteinatlas.org/)
* **OmniPath Database:** [https://explore.omnipathdb.org/](https://explore.omnipathdb.org/)
* **STRING Database:** [https://string-db.org/](https://string-db.org/)
* **IntAct Molecular Interaction Database:** [https://www.ebi.ac.uk/intact/](https://www.ebi.ac.uk/intact/)
* **UniProt Consortium:** [https://www.uniprot.org/](https://www.uniprot.org/)
