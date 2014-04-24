Sequence Analysis using Machine Learning 
========================================================

We want to develop a R Markdown document which will become a workflow and 
reside on the Bioconductor website. This README file provides detailed 
ideas and useful links which the workflow contributors can use while building
their workflows. 

Objectives of this workflow
--------------------------------
* The main aim of this workflow is to demonstrate different sequence analysis 
which can be done on 'BIG GENOMIC data' using  machine learning in a  parallel 
environment.

* We would like the workflow contributors to keep the following target audience 
in mind while building these workflows: 
 * a naive graduate student who is starting out in this field
 * a seasoned Bioinformatician who is wanting to fine tune his skills

* We would like to focus on Memory Management, run time and scalability and make
sure that each workflow can be run on a local laptop and scaled to a cluster
or super computer at the users institution. 

Analysis Type
----------------
We have identified the following analysis types

* RNA-Seq Analysis
* DNA-Seq Analysis
* ChIP-seq Analysis
* Phylo-Seq Analysis

Subsections for each Analysis Type
-------------------------------------
For each Analysis - we would like to have the following sections. 

#### 1. Introduction
define the analysis and list the goals/objectives. 

#### 2. Getting Data Ready for the analysis.  
Some ideas about what we would like to see here:
* identify data resources on the web or identify a data package in Bioconductor 
  to use for the analysis  
* steps taken on the raw data to obtain processed data which can be used 
for the analysis. 

#### 3. Data exploration
Some pointers:
* description of the data 
( For example, if the data is present as a data.frame, one can show a head of 
the data and describe variables - if the data is present as an 
ExperimentSet object, describe assayData, phenoData, experimentData and 
annotations in it.)
* unique properties of this data. 
* Why do we need machine learning techniques for this analysis? why will off 
the shelf techniques not work here ? ( Workflow contributors can focus on time
 taken, memory allocation and scalability.)

#### 4. Machine Learning Algorithms and their interpretation
* which machine learning algorithm is best ? why ?
* parameters used for analysis? why ? 
 
#### 5. Running the Machine Learning Algorithm on the data.
* different packages used for this analysis (especially Bioconductor based )
* comparing the analysis result from different packages
* running this analysis on local computer vs cluster ( using BiocParallel, 
  foreach ) - differences with respect to parameter tuning/setting up analysis
  /run time/ memeory management.  

#### 6. Downstream analysis
Downstream analysis of the results of each analysis will be specific to the 
analysis.One can also provide links to package vignettes. 

Useful Links to publications\literature at each step is higly recommended along
with the R version and Package version.

Useful Links
--------------
* how to create a workflow 
http://www.bioconductor.org/developers/how-to/workflows/
* link to existing workflow page 
http://www.bioconductor.org/help/workflows/
* for specific questions please contact : sarora@fhcrc.org



