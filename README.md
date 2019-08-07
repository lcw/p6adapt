This is an example of computing the global node numbers of adapted cubesphere
elements using `p6est`.  Each rank dumps the global node numbers for its local
elements to a file.

## Build and run

This build assumes you have [GNU Make][1].  To build the code you can run
something like:
```sh
make -j
```

The code can be run in parallel simply with
```sh
mpirun -np 2 ./p6adapt
```
The global node numbers are written out `rank_*.txt` files.

[1]: https://www.gnu.org/software/make
