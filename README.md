Code modified based on code provided in quicksort project of CS214. 
Some of code obtained from https://github.com/ucrparlay/Parallel-Strong-Connectivity


hash_table_d.h --> deterministic hash table
hash_table_nd.h --> nondeterministic hash table
ht_test_sq.cpp -> test file for sequential operations
ht_test_3r.cpp -> test file that repeats 3 rounds
ht_test_12.cpp -> test file for 12 inserts example
ht_test_sp1.cpp -> test file for nondeterministic hashtable efficiency 1e8 inserts
ht_test_sp2.cpp -> test file for deterministic hashtable efficiency 1e8 inserts





## Compiling the code  
A Makefile is given in the directory, simply use ``make`` to compile the code. If you're compiling the code on a M-series Mac, add the ``MXMAC=1`` option:  
```bash
make MXMAC=1  
```
## Running the code  
Enter the course environment by typing ``cs214`` in command line. Then you can run the code with:  
```bash
numactl -i all ./quicksort [num_elements] [num_rounds] [random_seed]  
```
If not specified, the default values are ``num_elements=100000000``, ``num_rounds=3`` and ``random_seed=1``.  
``numactl`` can help distribute memory pages evenly on multiple sockets. More information can be found in [Linux man page](https://linux.die.net/man/8/numactl).  



