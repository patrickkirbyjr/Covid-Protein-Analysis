# COVID-19 Genome Analysis with Biopython

This project analyzes the SARS-CoV-2 (COVID-19) reference genome using **Biopython**. The workflow includes:

1. **Downloading and reading the genome** (FASTA format).  
2. **Identifying the largest protein** encoded in the genome.  
3. **Matching the largest protein to known structures** using **BLAST (blastp)** against the PDB database.

---

## Requirements
- Python 3.x  
- [Biopython](https://biopython.org/) (`pip install biopython`)  
- Internet access for NCBI BLAST queries  

---

## How to Run
1. Download the SARS-CoV-2 genome (e.g., [NCBI NC_045512.2](https://www.ncbi.nlm.nih.gov/nuccore/NC_045512.2)).  
2. Run the provided scripts to:  
   - Parse the genome and extract proteins.  
   - Find the largest protein sequence.  
   - Perform a BLAST search to identify similar proteins in the Protein Data Bank (PDB).  

---

## Output
- **Largest protein sequence** (FASTA).  
- **BLAST results** including hit descriptions, E-values, and bit scores.

---

## Notes
- BLAST queries via `NCBIWWW.qblast()` are rate-limited; use responsibly.  
- E-values indicate match significance (lower is better).  
- This project follows a tutorial-based learning approach to practice genome analysis and sequence alignment.
