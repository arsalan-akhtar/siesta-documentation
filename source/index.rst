.. SIESTA documentation master file, created by
   sphinx-quickstart on Thu Jan 23 01:19:50 2020.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

Welcome to SIESTA's documentation!
==================================
SIESTA (Spanish Initiative for Electronic Simulations with Thousands of Atoms) is both a method and its computer program implementation, to perform electronic structure calculations and ab initio molecular dynamics simulations of molecules and solids. Its main characteristics are:
* It uses the standard Kohn-Sham selfconsistent density functional method in the local den-
sity (LDA-LSD) and generalized gradient (GGA) approximations, as well as in a non local
functional that includes van der Waals interactions (VDW-DF).
* It uses norm-conserving pseudopotentials in their fully nonlocal (Kleinman-Bylander) form.
* It uses atomic orbitals as a basis set, allowing unlimited multiple-zeta and angular momenta,
polarization and off-site orbitals. The radial shape of every orbital is numerical and any shape
can be used and provided by the user, with the only condition that it has to be of finite support,
i.e., it has to be strictly zero beyond a user-provided distance from the corresponding nucleus.
Finite-support basis sets are the key for calculating the Hamiltonian and overlap matrices in
O(N ) operations.
* Projects the electron wavefunctions and density onto a real-space grid in order to calculate the
Hartree and exchange-correlation potentials and their matrix elements.
* Besides the standard Rayleigh-Ritz eigenstate method, it allows the use of localized linear
combinations of the occupied orbitals (valence-bond or Wannier-like functions), making the
computer time and memory scale linearly with the number of atoms. Simulations with several
hundred atoms are feasible with modest workstations.
* It is written in Fortran 95 and memory is allocated dynamically.
* It may be compiled for serial or parallel execution (under MPI).
It routinely provides:
* Total and partial energies.
* Atomic forces.
* Stress tensor.
* Electric dipole moment.
* Atomic, orbital and bond populations (Mulliken).
* Electron density.
And also (though not all options are compatible):





















.. toctree::
   :maxdepth: 2
   :caption: Contents:

   authors-siesta
   compiling


