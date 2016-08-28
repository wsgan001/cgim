# cgim
Community-based Greedy Influence Maximization

# About

CGIM is an efficient algorithm for find a set of top-k influential nodes
in complex networks with community structure written in Java. 

# How to run

To run this algorithm, use the following command: 

    java joonion.CGIM.main.Main -k 10 -i [infile]

    -k [n] : n is the number of seed nodes for initiating influence spreading
    -i [infile] : infile is a graph that contains edge lists

The algorithm would produce three intermediat output files:
    
    [infile.index2node] an index file that indicate the name of nodes
    [infile.index2index] a graph that contains edge lists replaced with indices of vertices
    [infile.comm2index] a set of community that lists a community at each line

The output of the algorithm show top-k influential nodes:

     Example: java joonion.CGIM.main.Main -k2 -i karate.pairs
     0 1
     
The format of input file:

    Input file should constains an indexed edge at each line, separated by space of tab.
    0 1
    0 2
    ...
    
August 29,  2016. 

# References 

Joonhyun Bae. "Efficient detection of top-k influential spreaders ini social networks 
with community structure", Under Review.
