**IMPORTANT NOTE:** I am not supporting this code any longer, but if you make a pull request with bug fixes and improvements I can surely take a glance and accept them.

Package: priority_queue 0.9
Date: 22 May 2009

priority_queue provides a minimal implementation of a priority queue for Matlab. The implementation can be used either inside MATLAB by means of MEX calls, or directly from a C/C++ program. The image on the website has been created with "pq_demo.m"

# Functions
- pq_create: 		        creates a priority queue
- pq_delete:		        frees the memory allocated
- pq_push:      		inserts a new element in the queue 
- pq_top:   			queries topmost element in the queue  
- pq_pop:           		retrieves and removes topmost element 
- pq_size:            		queries the queue size  

# File Structure
Everyone of the scripts/functions is complete of the following:
*.cpp:      the mex implementation of the sources
*.m:        the comments that you can browse with the "help" command

# Compile
IMPORTANT NOTE: I assume you have a correctly configured MEX environment.
You can compile directly inside MATLAB:
>> mex pq_create.cpp
>> mex pq_delete.cpp
>> % .... etc.
 
# Develop (C++)
As mentioned the *.cpp files contain a MEX interface for MATLAB. 
- a C++ test/demo program is provided in pq_demo.cpp
- a MATLAB test/demo program is provided in pq_demo.m

# Compatibility
priority_queue compiles correctly with the following compilers:  
- i686-apple-darwin9-g++-4.0.1 (GCC) 4.0.1 (Apple Inc. build 5484)
- Visual studio c++ 6.0 with Service pack 6