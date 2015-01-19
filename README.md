# rhdf5
This is an unofficial fork of the R rhdf5 package developed by Bernd Fischer and Gregoire Pau. 
This fork is based on rhdf5 version 2.10.0

Objective:

1. (Immediate) To fix the problems in the original package. For example the function *h5read* can not properly import int64 data from HDF5 files, 
even when its parameter *bit64conversion* has been explicitly specified as *"bit64"* as suggested by the function's warning output.

2. (Future) To enable the fully compatable data exchange between Python's Pandas data frames and R's data frames (or data table). 
Given the current stuation that rhdf5 as of version 2.10.0 can not handle data types other than numeric matrix and string. 
That makes it impossible to read and write data of datetime, factor types from HDF5 files.
