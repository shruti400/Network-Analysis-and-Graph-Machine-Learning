Human Protein-Protein Interaction (PPI) Dataset
===============================================

This dataset contains information on human protein-protein interactions, including both 
positive interactions (experimentally verified) and negative interactions (assumed or 
derived non-interacting pairs). It also includes protein identifiers and amino acid sequences.

File Descriptions
-----------------

1. proteinList.txt
   - Description: List of all unique proteins in the dataset.
   - Format: Plain text file with one protein ID per line.
   - Example:
     0    10968
     1    11542
     ...

2. sequenceList.txt
   - Description: Contains amino acid sequences for each protein listed in proteinList.txt.
   - Format: Plain text file where each line corresponds to the amino acid sequence of the 
     protein in the same line of proteinList.txt.
   - Note: Line i in sequenceList.txt is the sequence of the protein at line i in proteinList.txt.

3. PositiveEdges.txt
   - Description: Pairs of proteins that are known to interact (positive examples).
   - Format: Tab-separated file with two columns.
   - Example:
     0	5540
     1	441
     ...

4. NegativeEdges.txt
   - Description: Pairs of proteins that are assumed not to interact (negative examples).
   - Format: Tab-separated file with two columns.
   - Example:
     4565	6450
     6977	3142
     ...

Usage
-----
This dataset is suitable for tasks such as:
- Supervised learning for PPI prediction.
- Embedding protein sequences for interaction analysis.
- Evaluating performance of PPI prediction models.

Notes
-----
- All protein IDs follow the UniProt format.
- The sequences in sequenceList.txt should be parsed in order with proteinList.txt to 
  map sequences to protein IDs.
- Negative edges are generated using sampling methods and may contain false negatives.

License
-------
This dataset is intended for research and educational purposes only.
