# Molecular Docking and Virtual Screening Workflow

This project demonstrates how to set up and run molecular docking, ligand preparation, and receptor-ligand visualization using PyMOL, RDKit, and Smina in Google Colab. The workflow covers ligand and receptor preparation, docking with Smina, and post-docking analysis.

## Project Overview

The main steps in this workflow are:
1. **Set up the environment** using Google Colab with the necessary libraries for molecular docking and visualization.
2. **Download receptor and ligand data**, and set up the PyMOL educational license.
3. **Prepare ligands** using RDKit and convert them to 3D structures.
4. **Run molecular docking** using Smina.
5. **Post-docking analysis** includes generating 3D visualizations of the receptor-ligand complexes and calculating docking scores.
6. **Evaluate results** using ROC curves based on the docking affinity and the ligand activity.

## Requirements

This project is intended to be run on **Google Colab**. The following packages and tools are required:
- PyMOL (Schrodinger)
- RDKit
- Py3Dmol
- Smina
- Pandas, NumPy, Matplotlib
- Conda and Mamba for installing packages

You can install these dependencies directly in Colab via `condacolab` and `mamba`.

### Installation Commands in Colab:
```python
# Install necessary packages using Conda
!pip install -q condacolab
import condacolab
condacolab.install()

# Install PyMOL, RDKit, and other tools
!mamba install -c schrodinger pymol-bundle --yes
!mamba install -c conda-forge mols2grid --yes
!mamba install rdkit --yes
!mamba install py3Dmol --yes
