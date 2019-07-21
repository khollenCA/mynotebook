**Homework 1**
-----------

1. Prepare working environment and run examples.
========

.. code-block:: bash

 	$ git clone https://github.com/EvolutionaryGenomics/scalability-reproducibility-chapter.git
  	cd scalability-reproducibility-chapter
  	cd Docker
  	docker build -t scalability
..
 
 For Snakemake:
 
 .. code block:: bash
 	docker run -t -v ${pwd}/scalability-reproducibility-chapter:/analysis evolutionarygenomics/scalability_snakemake snakemake -j 2 --timestamp -s /analysis/Snakemake/Snakefile -d /analysis/scalability-reproducibility-chapter

For CWL:

2. Compare syntaxes.
========

3. Cost
========
