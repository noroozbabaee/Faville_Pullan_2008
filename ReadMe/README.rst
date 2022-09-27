Original Paper
==============

:Original publication:  "A Biophysically Based Mathematical Model of Unitary Potential Activity in
Interstitial Cells of Cajal"

:DOI: 10.1529/biophysj.107.122507


Model status
=============
The original CellML model is divided into eighteen sub-modules presenting a modularized version of various ion channels.

Model Summary
==============
Unitary potential (UP) depolarizations are the primary intracellular events responsible for pacemaker activity in
interstitial cells of Cajal (ICCs) and are generated at intracellular sites termed pacemaker units. In the current study, the authors present a
mathematical model of the transmembrane ion flows and intracellular Ca2+ dynamics from a single ICC pacemaker unit acting at
near-resting membrane potential. This model quantitatively formalizes the framework of a novel ICC pacemaking mechanism that
has recently been proposed. The model predicts that the main inward currents, carried by a Ca2+-inhibited nonselective cation
conductance, are activated by depletion of sub-plasma-membrane [Ca2+] caused by sarcoendoplasmic reticulum calcium
ATPase Ca2+ sequestration. Furthermore, pacemaker activity predicted by the current model persists under simulated voltage clamp and
is independent of [IP3] oscillations.

.. image:: ReadMe/Faville_2008.png
   :width: 70%
   :alt: Schematic diagram.


Schematic diagram of the ICC pacemaker unit showing all the components involved in the modelling framework. The ionic conductances
and their respective interactions with the intracellular organelles and cytoplasmic subspaces are displayed. The compartmental volumes comprising the pacemaker unit are


1. The dynamics of the endoplasmic reticulum (ER),
2. The  dynamics of the mitochondria,
3. The dynamics of cytoplasmic subspace 1,
4. The dynamics of cytoplasmic subspace 2,
5. The dynamics of membrane potential.


The model is implemented using a Hodgkin-Huxley type formulation. The cell membrane lipid bilayer is represented as a capacitance (Cm),
and the ion channels in the membrane are represented as conductance. The change in the transmembrane potential (Vm) over time depends on
the sum of the individual ion currents through each class of ion channel in the cell current:


:math:` \frac{dVm}{dt} = - \frac{I_{tot}}{C_{m}}`.


Where there are five different ion channels that regulate cellular
electrophysiology:

1. The inward Ca2+ current (ICa),

2.  The nonselective cation conductance (INSCC {Na}),

3.  The nonselective cation conductance (INSCC {Ca}),

4. The plasma membrane Ca2+-ATPase (IPM),

5. The outward Na+ current (INa).

The five Ca2+ fluxes responsible for controlling intracellular Ca2+ movement are

1. The mitochondrial Ca2+ uniporter (JMCU);
2. The mitochondrial Na+/Ca2+  exchanger (JNCX);
3. Sarcoendoplasmic reticulum Ca2+-ATPase (JSERCA);
4. The IP3R Ca21 flux (JIPR);
5. The intercytoplasmic subspace Ca21 flux (JS1S2).


Model Workspace
=======================
1. Doc: A ReadMe file that includes all the information about the article and curation (simulations and components).
2. Simulation: CellML file that reproduces the overall mathematical model.
3. Components: The modular version of each component of the primary model.
4. Common: Includes environment, units and parameters files.
