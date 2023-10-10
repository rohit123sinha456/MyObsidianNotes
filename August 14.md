## Optimising Neural Networks
### Locality of Reference
Instruction and data in a loop and in a functions are likely to referenced repeatedly. [Temporal Locality]
Locations that are nearby are likely to be accessed multiple times. fr example an array.[spatial locality]
in short, locus of a memory is small in a short window of time.
These are typical observation and not rules or something
For example heaps and linked list violates these things

We have a memory hierarchy like from registers the fastest to hard list the slowest. We normally distribute the usage to justify the cost of the system using the memories.

For faster data access 
- we can use the temporal locality and move data to cache for faster access -> aka caching.
- Pre-fetching of data. using data spatial locality we anticipate and prefetch the data.
- Blocked access -> access data in bulk. like access one of two tracks of HDD and store in RAM. This helps in quick access of the data.

Matrix ( multi dimensional array ) is stored in row major format. However for Matrix multiplication we are accessing one matrix in colom major format. This is unoptimised and cannot use the locality of the reference. So Access to one matrix in matrix multiplication ( one that is accessed row major wise) is efficient in accessing elements, the other one is not.

Now if we use cache aware matrix multiplication algorithm we optimise the above mentioned problem.

test commit 2

