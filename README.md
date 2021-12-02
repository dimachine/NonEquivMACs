# NonEquivMACs
This is a supporing file for OEIS on computation of inequivalent maximal antichains and related sequences

## Outline 

### 0. The basic code with the class for managing generation of formal concepts via NextClosure algorithm
### 1. Generation of inequivalent maximal antichains for n in {1,2,3,4,5,6,7} (https://oeis.org/draft/A348260)
### 2. Extraction of maximal antichains from order ideals
### 3. Generating non-singleton maximal antichains for A326360 with n in {5,6,7} (https://oeis.org/draft/A326360)
### 4. Generation of dictionaries with all inequivalent maximal antichains along with their orbits' cardinalities for n in {1,2,3,4,5,6}


#### Comment to Section 3.

The value a(7) has been computed with my code in Python provided in Section 3. To reproduce the result one needs the whole set of maximal antichains of the powerset of {1,...,7} encoded as list of integers. All the maximal antichains for n=7 in a zip archive are available in my dropbox: https://www.dropbox.com/s/uoqt939rokphnmx/allMAC7.pickle.zip (1.42 GiB). They were pickled first. To unpickle their list you need to execute the line of code: MACs7=pickle.load(open("allMAC7.pickle","rb")). Then, all the antichains with signle-element sets (i.e. single-bit integers smaller than 128) and the empty set (i.e. 0) are subject to elimination. The code has been tested for n=5 and n=6 as well.

To check a(4) and a(5) one needs the lists of maximal antichains precomputed and encoded as a list of integers each. They are available in my dropbox as well: https://www.dropbox.com/s/lk43sn319fh9kx3/allMAC5.pickle and https://www.dropbox.com/s/03e76x890sd0eso/allMAC6.pickle . To unpickle one needs to execute two lines: MACs5=pickle.load(open("allMAC5.pickle","rb")) MACs6=pickle.load(open("allMAC6.pickle","rb")).


## References

* Bernhard Ganter, Rudolf Wille:
Formal Concept Analysis - Mathematical Foundations. Springer 1999, ISBN 978-3-540-62771-5, pp. I-X, 1-284

* Klaus Reuter: The jump number and the lattice of maximal antichains. Discret. Math. 88(2-3): 289-307 (1991)
https://core.ac.uk/download/pdf/82019205.pdf



