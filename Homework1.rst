**Homework 1**
-----------

1. Prepare working environment and run examples.
========

Clone the Github repository and build the container.

.. code-block:: bash

 	$ git clone https://github.com/EvolutionaryGenomics/scalability-reproducibility-chapter.git
  	cd scalability-reproducibility-chapter
  	cd Docker
  	docker build -t scalability
..
 
For Snakemake:
 
.. code-block:: bash

  docker run -t -v ${pwd}/scalability-reproducibility-chapter:/analysis evolutionarygenomics/scalability_snakemake snakemake -j 2 --timestamp -s /analysis/Snakemake/Snakefile -d /analysis/scalability-reproducibility-chapter

For CWL:

.. code-block:: bash

 docker pull nvk747/cwl_docker2
 docker run -it --name cwl -v /home/carlos88/scalability-reproducibility-chapter/:/cwl_analysis nvk747/cwl_docker:latest
 docker run -it -v /home/carlos88/scalability-reproducibility-chapter/data/:/data -v /home/carlos88/scalability-reproducibility-chapter/CWL/:/cwl nvk747/cwl_docker2:latest
 cwl-runner /cwl/workflow_simple.cwl /cwl/workflow_simple-job.yaml

2. Compare syntaxes.
========

3. Cost
========
