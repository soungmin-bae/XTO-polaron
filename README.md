# XTO-polaron: Structural data for polaron self-trapping in titanate oxides

This repository provides structural and input data associated with the study:

**“Koopmans-compliant density functional framework for polaron self-trapping in titanate oxides”**

The dataset contains relaxed atomic structures corresponding to self-trapped electron (STE) and self-trapped hole (STH) states in a series of titanate oxides, obtained from first-principles density-functional theory calculations. In addition, representative VASP input files used for PBEsol+U_KC calculations are provided to facilitate reproducibility.

---

## Repository structure

The repository is organized by material and crystal structure:

01-STO-I4mcm                 SrTiO3 (I4/mcm)  
02-CTO-Pnma                  CaTiO3 (Pnma)  
03-TiO2-rutile-P42_mnm       TiO2 (rutile, P42/mnm)  
04-TiO2-anatase-I41_amd      TiO2 (anatase, I41/amd)  
05-BTO-R3m                   BaTiO3 (rhombohedral, R3m)  
06-BTO-Pm-3m                 BaTiO3 (cubic, Pm-3m)  

Each directory contains data for both self-trapped electron and self-trapped hole configurations.

---

## File contents

Each material directory includes the following file types:

- `*.mcif`  
  Crystallographic information files containing relaxed atomic positions.

- `*.vasp`  
  VASP POSCAR-format files for the same relaxed structures.

- `*.vesta`  
  VESTA visualization files used to reproduce the figures of polaron localization and atomic displacements presented in the main text and Supplementary Information.

In addition, this repository includes representative **VASP input files (INCAR, KPOINTS, and POTCAR specifications)** used for the **PBEsol+U_KC** calculations reported in the manuscript. These inputs document the choice of exchange–correlation functional, Hubbard U_KC parameters, and relevant computational settings.

---

## Naming convention

File names follow the format:

[material]-[structure]-self-trapped-[electron/hole]-@[site].[extension]

Examples:
- STO-I4mcm-self-trapped-electron-@Ti1.vasp  
- TiO2-rutile-P42_mnm-self-trapped-hole@O.mcif  

Here, `@Ti1` or `@O` denotes the atomic site on which the electron or hole is localized.

---

## Reproducibility

The structural data and VASP input files provided in this repository are sufficient to reproduce the carrier self-trapping configurations, atomic displacements associated with self-trapped states, and the visualization of localized electron and hole polarons reported in the main manuscript and Supplementary Information.

Further details of the Koopmans-compliant framework, including the determination of U_KC parameters and the application of GKFO corrections, are described in the Methods section of the manuscript.

---

## Software

The data were generated and visualized using the following software:

- **VASP** (Vienna Ab initio Simulation Package)  
- **VESTA** for visualization of atomic structures and polaron localization  

---

## License and usage

This dataset is provided for academic and non-commercial research use. If you use this data in your work, please cite the corresponding publication.

---

## Contact

For questions regarding the data or requests for additional information, please contact:

Soungmin Bae  
Institute for Materials Research, Tohoku University  
E-mail: bae.soungmin.d6@tohoku.ac.jp
