# Jenkins Architecture

## Master & Slave Architecture
	
	* Master
		
		* Schedule Build job.
		* Dispatch builds to the slave for actual job execution.
		* Monitoring slave and recording the build results.
		
	* Slave
		
		* Execute build jobs dispatched by the master.
		* 

## What is Jenkins Job?
	
	* Runnable tasks that are controlled and monitored by jenkins.
	
## Slave/Node
	
	* Slaves or nodes are computers set up to build Projects for a master.
	* VMs or cloud machines.
	* Jenkins run seperate programs called `slave agents` on slaves.
	* When slaves are registered to the Master ,master starts distributing load to slaves.
	
## Executors
	
	* On a single Node/Slave we can define n number of Executors.
	* Executor can be said as stream of builds which need to be run in parallel.