# What is PIPS?

PIPS is a suite of parallel optimization solvers mainly for stochastic optimization problems consisting of the following solvers:
 * PIPS-IPM - parallel MPI+OpenMP interior-point for stochastic LPs and convex QPs
 * PIPS-S   - parallel MPI implementation of the revised simplex method
 * PIPS-NLP - parallel MPI interior-point for structured NLPs

[StructJuMP](https://github.com/StructJuMP/StructJuMP.jl) provides an interface
for modelling block structured optimization problems in Julia while using PIPS
as a solver (see specific [setup instructions](./structjump.md)).

# License

See LICENSE file.

# Contributions

## PIPS-IPM

### Developed by:
  * Cosmin G. Petra - Lawrence Livermore / Argonne National Laboratory

### Contributions from:
  * Miles Lubin - Argonne National Laboratory
  * Naiyuan Chiang - Argonne National Laboratory

## PIPS-S

### Developed by: 
  * Miles Lubin - Argonne National Laboratory
  * Cosmin G. Petra - Lawrence Livermore / Argonne National Laboratory

### Contributions from:
  * Geoffrey Oxberry - Lawrence Livermore National Laboratory
  * Julian Hall - U. of Edinburgh

## PIPS-NLP 

### Developed by:
 * Naiyuan Chiang - Argonne National Laboratory
 * Victor Zavala - Argonne National Laboratory and Univ. of Wisconsin-Madison
 * Cosmin G. Petra - Lawrence Livermore / Argonne National Laboratory	 

### [Doxygen documentation](./PIPS-NLP/)

# [INSTALLATION INSTRUCTIONS](./installation.md)

# ACKNOWLEDGMENTS

PIPS has been developed under the financial support of: 
- Department of Energy, Office of Advanced Scientific Computing Research
- Department of Energy, Early Career Program 
- Department of Energy, Office of Electricity Delivery and Energy Reliability

PIPS-IPM and PIPS-NLP are derivative works of OOQP (http://pages.cs.wisc.edu/~swright/ooqp/) by E. Michael Gertz and Stephen. Wright

