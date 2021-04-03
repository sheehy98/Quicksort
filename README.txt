Our project is dependent on words.english.txt from hw4

For every test T, 17 new data sets are created (doubles, strings, and ints from 0 to N/k from k = 2 to k = 16) and the three sorts are used on each data set

The set of doubles is created using StdRandom.uniform(), the set of strings is created by placing all of the words in the dictionary into an array and then
grabbing N words from random positions in the array using StdRandom.uniform(dict.length-1), and the sets of ints are created using StdRandom.uniform(SIZE/k)

Between each sort the sets are shuffled so pre-sorted sets are not passed into the sorts

The code takes a while to run when T is large (we used 100 to ensure our results were outlier proof) because it has to create all of the datasets every time.

The sorts were all taken from Sedgewick, our code is in the tester file

The code assumes good input for number of tests and data set size

To see the code in action, run tester.java and follow the prompts

Sample output from T = 100 and N from 2^14 to 2^18 is provided

Video link: https://youtu.be/75lyaxOiHMk