# Partition_ADG_UVVIS_Distribution
---

The ADG partitioning model separates the non-phytoplankton absorption coefficient, a<sub>dg</sub>, into the chromophoric dissolved organic matter (CDOM) absorption coefficient, a<sub>g</sub>(λ), and non-algal (depigmented) particulate absorption coefficient, a<sub>d</sub>. The model partitions an input spectrum of a<sub>dg</sub>(λ) using predefined libraries of spectral shape functions for a<sub>d</sub> and a<sub>g</sub>. This version of the model is configured for use in the near ultraviolet to visible spectral range (UVVIS, 350 to 700 nm) and utilizes spectral shape libraries specifically defined for this spectral range. The ADG partitioning model is described in Kehrli, M. D., Stramski, D., Reynolds, R. A., & Joshi, I. D. Model for partitioning the non-phytoplankton absorption coefficient of seawater in the ultraviolet and visible spectral range into the contributions of non-algal particulate and dissolved organic matter. Manuscript published in Applied Optics on June 1, 2024. The model source code is in MATLAB file format.

This README document provides information about the files within the Partition_ADG_UVVIS_Distribution repository.

---

## Partition_ADG_UVVIS.m:
MATLAB function implementing the ADG partitioning model to partition input a<sub>dg</sub>(λ) into a<sub>g</sub>(λ) and a<sub>d</sub>(λ) using predefined libraries of spectral shape functions defined in the UVVIS. Returns output wavelength (lambda_out), a<sub>d</sub>(λ) (adopt), and a<sub>g</sub>(λ) (agopt). See supporting documentation for further details.

## Partition_ADG_UVVIS_Test.m:
MATLAB script that executes Partition_ADG_UVVIS.m on one sample input of spectral a<sub>dg</sub>(λ) defined from 350 to 700 nm in 1 nm intervals. The code implements the model with the predefined UVVIS spectral shape function libraries to partition input a<sub>dg</sub>(λ) into a<sub>g</sub>(λ) and a<sub>d</sub>(λ) from 350 to 700 nm in 1 nm intervals.

## Partition_ADG_UVVIS_Test_Run.xls:
Microsoft Excel spreadsheet containing the input and resulting output data obtained from the application of the Partition_ADG_UVVIS.m on one sample input of a<sub>dg</sub>(λ) to estimate a<sub>g</sub>(λ) and a<sub>d</sub>(λ). The file is the original output file generated by Partition_ADG_UVVIS_Test.m.

## UVVIS_lib.mat:
MATLAB file containing the libraries of spectral shape functions defined in the near-UV through visible spectral region (from 350 to 700 nm with a 1 nm spectral interval). See the supporting publication (in preparation) for further details about the formation of the library.

---

Contributors: Matthew Kehrli, Dariusz Stramski, Rick A. Reynolds, and Ishan Joshi\
Contacts: Matthew Kehrli (mdkehrli@ucsd.edu | mdkehrli@gmail.com), Dariusz Stramski (dstramski@ucsd.edu), Rick Reynolds(rreynolds@ucsd.edu), Ishan Joshi(isjoshi@ucsd.edu)\
Ocean Optics Research Laboratory, Scripps Institution of Oceanography, University of California San Diego

---
