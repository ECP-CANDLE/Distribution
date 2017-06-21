# Distribution
Distributing CANDLE

This repository contains the definiton file and the dependencies required to
build a singularity container that can run the CANDLE benchmarks and the supervisor. 


To build the singularity image, first install singularity 2.3 Release:

* http://singularity.lbl.gov/all-releases

Once singularity is installed, you can create a singularity CANDLE image by running:

----
$ sudo singularity create -s 5000 candle.img 
$ sudo singularity bootstrap ./candle.img swift-hypervisor.def 
----
