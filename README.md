# phylogenetic-diversity-in-EC-GECCO-2022
This repository contains all code and supplimental material for "Untangling phylogenetic diversity's role in evolutionary computation using a suite of diagnostic fitness landscapes" which was presented at <a href="https://gecco-2022.sigevo.org/HomePage">The Genetic and Evolutionary Computation Conference</a>, 2022. 

  **Contents:**
  - [Abstract](https://github.com/emilydolson/phylodiversity-metrics-in-EC-GPTP-2021#abstract)
  - [Supplemental information](https://github.com/emilydolson/phylodiversity-metrics-in-EC-GPTP-2021#supplemental-information)
  - [Dependencies](https://github.com/emilydolson/phylodiversity-metrics-in-EC-GPTP-2021#dependencies)
  - [Compilation](https://github.com/emilydolson/phylodiversity-metrics-in-EC-GPTP-2021#compilation)
  - [Authors](https://github.com/emilydolson/phylodiversity-metrics-in-EC-GPTP-2021#authors)
  - [Research overview](https://github.com/emilydolson/phylodiversity-metrics-in-EC-GPTP-2021#research-overview)
  - [Repository contents](https://github.com/emilydolson/phylodiversity-metrics-in-EC-GPTP-2021#repository-contents)

## Abstract
Diversity is associated with success in evolutionary algorithms. To date, diversity in evolutionary computation research has mostly been measured by counting the number of distinct candidate solutions in the population at a given time point. Here, we aim to investigate the value of phylogenetic diversity, which takes into account the evolutionary history of a population. To understand how informative phylogenetic diversity is, we run experiments on a set of diagnostic fitness landscapes under a range of different selection schemes. We find that phylogenetic diversity can be more predictive of future success than traditional diversity metrics under some conditions, particularly for fitness landscapes with a single, challenging-to-find global optimum. 

## Supplemental information
The supplimental information for this paper can be found here. 

## Dependencies
To run these experiments, the Modular Agent Based Evolver (MABE2) is required: 
- [MABE2](https://github.com/mercere99/MABE2)

## Compilation
To complie and run the code used in this paper, take the following steps:

```{bash, shell_installation}
# Clone MABE2
git clone --recursive https://github.com/mercere99/MABE2.git

# Clone the repo for this project
git clone --recursive 

### Complex fitness landscapes

# Compile MABE2
cd MABE2/build
make

# Tell MABE which configeration file to run
cd build
./MABE -f ../settings/PhylodiversityDiagnostics.mabe

# To set parameters, use command line flags
# e.g. to set the selection scheme, run --set selection_type = 0
# or to set the diagnostic suite, run --set diagnostic = 1

```
## Authors
- [Shakiba Shahbandegan](https://github.com/shakiba-shb)
- [Jose Guadalupe Hernandez](https://jgh9094.github.io/)
- [Alexander Lalejini](https://lalejini.com/)
- [Emily Dolson](http://emilyldolson.com/)

