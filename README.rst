nvidia CUDA runtime 
*******************

singularity container with a nvidia cuda runtime.
Current Container is based on CentOS 6
Originally intended for providing a container to run CUDA programs setup on CentOS 6 to run in a CentOS 7 host env.

May deploy different branch for different version on different OS as needed.


To run::

	singularity pull shub://tin6150/cuda


Ref: 

- https://www.singularity-hub.org/collections/382
- https://github.com/tin6150/cuda


~~~~

Dev/Build instructions 

.. code:: bash

	SING_VER=2.4.1
	module load container/singularity/${SING_VER}
	Singularity=$( which singularity )
	sudo    $Singularity build -w tba.simg ./Singularity
	-or-
	mkdir ./sandbox
	sudo    $Singularity build --sandbox ./sandbox ./Singularity


