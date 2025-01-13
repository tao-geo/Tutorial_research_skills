# My thoughts on this

## About projects design

### Folder dedicated for results for publishing

Being able to re-producing main figures and other results for publishing is important.

Separating "Code for Ploting/Making tables (for publication, or 'fancy-figures' as in this tutorial)" and "Code for Analyzing". 
Perpaps having a folder dedicated for main results - figures/tables for publications, only keep scripts for making figures/tables there. 
Those scripts will read data stored elsewhere, including data downloaded or processed by analyzing scripts.


An example folder:
TEMPLATE_PROJECT:
- ./main: folder for final figures/table for publications, and scripts that generated those results.
- ./lib: scripts for intermediate analysis and processes
  - ./lib/PART1:
  - ./lib/PART2: subfolder for "grouped processed"
  - ... generated intermediate data (files) can be stored in each subfolder or Data folder, if will be used by other PART or main.
- ./Data: data downloaded from elsewhere, e.g., from supercomputer.
- ./Doc: reports or technical documentation.
  - ./Doc/xxx.

