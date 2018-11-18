# cache_replacement_policy
The title of this project is IMPLEMENTATION & EVALUATION OF CACHE REPLACEMENT POLICIES using ChampSim simulator.
ChampSim simulator is a is an extended version of the simulator used in the 2nd Data Prefetching Championship and recently used in the 2nd
Cache Replacement Championship. It simulates a simple multi-core out-of-order processor. ChampSim simulator can be cloned from the github repository :
https://github.com/ChampSim/ChampSim

ChampSim takes five parameters: Branch predictor, L1D prefetcher, L2C prefetcher, LLC replacement policy, and the number of cores.
This project has been done for single core systems. The replacement policies used are 
1. LRU(Least Recently Used)
2. SHIP(Signature-based Hit Predictor)
3. DRRIP(Dynamic Re- reference Interval Prediction) 
4. SRRIP(Static Re- reference Interval Prediction)

For the first set of simulations, no L1D and L2C pre-fetchers have been used.The branch predictor used is bimodal. The trace used for the simulation is bzip2_183B and number of instructions for the warmup run is 1 million and for the detailed simulation is 10 million.

For the second set of simulations, the branch predictor used is global History Counter or commonly called as gshare. Rest of the variables remain the same.

The output files of the above four replacement algorithms have been included. They give the result of the simulations at hardware level. The statistics for the 10 million instructions has been provided which show the number of hits and misses in the various levels of cache and in DRAM.

The findings, results and observations of this project is included in the PDF file named proj_findings.pdf
