# Protein_charge_pI_calculator
This repository contains a Google Colab notebook for calculating the net charge and isoelectric point (pI) of proteins from user-provided PDB codes.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mcathcarth/Protein_charge_pI_calculator/blob/main/Protein-Charge_Isoelectric-Point_Calculator.ipynb)

# Protein Charge and Isoelectric Point Calculator

**Author:** Marilina Cathcarth
  - Email: mcathcarth@gmail.com
  - GitHub: [mcathcarth](https://github.com/mcathcarth)
    
**Version:** 1.1
    
**Date:** Jun 10, 2024
    
**Description:** This script calculates the net charge and isoelectric point (pI) of proteins based on their sequences extracted from PDB files. The net charge of each protein is computed over a specified pH range, and the data is saved and visualized.

## Dependencies:

The script uses the following Python libraries:

- [Biopython](https://biopython.org/) (Bio) - Licensed under the Biopython License Agreement (BPLA)
- [NumPy](https://numpy.org/) - Licensed under the BSD License
- [Matplotlib](https://matplotlib.org/) - Licensed under the BSD License
- [requests](https://docs.python-requests.org/en/latest/) - Licensed under the Apache License 2.0

## Usage Instructions

1.  **Open the Colab Notebook:** Click on the "Open In Colab" badge above to open the notebook directly in Google Colab.
    
2.  **Modify Input Parameters:**
    
    *   Update the `pdb_codes` list with the [PDB](https://www.rcsb.org/) codes of the proteins you want to analyze.
        
    *   Optionally, provide user names (`usr_names`) and number of chains (`usr_nc`) if needed.
        
    *   Set the parameters for `pH_start`, `pH_end`, `pH_step`, and `target_pH` as per your requirements.
        
3.  **Run Each Cell Sequentially:** Ensure that you run each cell in order, as some cells depend on the outputs or definitions from previous cells.
  
4.  **View Results:** After running the final cell, view the output which includes the isoelectric point (pI) and the net charge of each protein at the target pH. Additionally, a plot showing the net charge vs. pH will be generated and saved.

5.  **Save Your Work:**

    *   To save your changes, you can either:
    
      -   Download the notebook to your local machine: `File -> Download .ipynb`

      -   Save a copy to your Google Drive: `File -> Save a copy in Drive`
  
6.  **Note:** Any changes you make in Google Colab will not affect the original notebook in this GitHub repository. Each user works on their own copy of the notebook.


### Example Parameters

*   `pdb_codes`: A list of PDB codes for the proteins to analyze (e.g., ["4F5S", "1CF3", "1OVA"]).
    
*   `usr_names`: Optional list of user-provided names for the proteins.
    
*   `usr_nc`: Optional list of the number of chains to consider for each protein.
    
*   `pH_start`: Starting pH value for the range (e.g., 3.0).
    
*   `pH_end`: Ending pH value for the range (e.g., 10.0).
    
*   `pH_step`: Step size for the pH range (e.g., 0.1).
    
*   `target_pH`: Specific pH value at which to calculate the net charge (e.g., 7.4).


## Citation

If you use this tool in your research, please cite this repository as:

[Cathcarth Marilina]. (2024). Protein Charge and Isoelectric Point Calculator [GitHub repository]. Retrieved from https://github.com/mcathcarth/Protein_charge_pI_calculator

