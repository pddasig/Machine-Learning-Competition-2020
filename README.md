# PDDA-Machine-Learning-Competition-2020

## SPWLA PDDA’s 1st Petrophysical Data-Driven Analytics Contest -- Sonic Log Synthesis

### Background
Well logs are interpreted/processed to estimate the in-situ petrophysical and geomechanical properties, which is essential for subsurface characterization. Various types of logs exist, and each provides distinct information about subsurface properties. Certain well logs, like gamma ray (GR), resistivity, density, and neutron logs, are considered as “easy-to-acquire” conventional well logs that are run in most of the wells. Other well logs, like nuclear magnetic resonance, dielectric dispersion, elemental spectroscopy, and sometimes sonic logs, are only run in limited number of wells.

Sonic travel-time logs contain critical geomechanical information for subsurface characterization around the wellbore. Often, sonic logs are required to complete the well-seismic tie workflow or geomechanical properties prediction. When sonic logs are absent in a well or an interval, a common practice is to synthesize them based on its neighboring wells that have sonic logs. This is referred to as sonic log synthesis or pseudo sonic log generation. 

### Problem Statement
Compressional travel-time (DTC) and shear travel-time (DTS) logs are not acquired in all the wells drilled in a field due to financial or operational constraints. Under such circumstances, machine learning techniques can be used to predict DTC and DTS logs to improve subsurface characterization. The goal of the “SPWLA’s 1st Petrophysical Data-Driven Analytics Contest” is to develop data-driven models by processing “easy-to-acquire” conventional logs from Well #1, and use the data-driven models to generate synthetic compressional and shear travel-time logs (DTC and DTS, respectively) in Well #2. A robust data-driven model for the desired sonic-log synthesis will result in low prediction errors, which can be quantified in terms of Mean Absolute Error by comparing the synthesized and the original DTC and DTS logs.

You are provided with two datasets: Well #1 dataset and Well #2 dataset. You need to build a generalizable data-driven models using Well #1 dataset. Following that, you will deploy the newly developed data-driven models on Well #2 dataset to synthesize DTS and DTC logs. The data-driven model should use feature sets derived from the following 8 logs: Caliper, Neutron, Gamma Ray, Deep Resistivity, Medium Resistivity, Shallow Resistivity, Photo-electric factor and density. The data-driven model should synthesize two target logs: DTC and DTS logs.

## About us
[Petrophysical Data-Driven Analytics (PDDA)](https://www.spwla.org/SPWLA/Chapters_SIGs/SIGs/PDDA/PDDA.aspx), a special interest group under society of Petrophysicists and Well Log Analysts (SPWLA), is announcing its first machine learning contest in 2020!
The contest is open to all SPWLA members (including student members) or whoever are interested in machine learning applications in petrophysics. Top winner teams will be awarded prizes and invited to present their work on the PDDA SIG annual meeting. If you or your teams are interested in this contest, please pre-register with Yanxiang Yu (pdda_sig@spwla.org) by submitting your team information including names, affiliations and contacts before January 31, 2020.

## Cometition Rules
We'll be releasing the compeition dataset and competition rule shortly...

## Sponsoring opportunities:
SPWLA PDDA SIG is accepting sponsorship for this event to award the top winning teams. Please contact Yanxiang Yu for details.

## SPWLA PDDA SIG Contest Committee:
Yanxiang Yu, Michael Ashby, Yan Xu, Oghenekaro Osogba, Siddharth Misra, Brendon Hall, Chicheng Xu, Weichang Li 


