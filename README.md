1) Exact F2

Exact F2 was supposed to reduce the number of plate numbers that got multiple parking tickets. As a result, I mapped all the plate numbers and used the reducebykey function to reduce all the multiple plate numbers that received multiple tickets. This was done by mapping and reducing using the key and adding them up in order to reduce them and then to do reduce by key.

2) Tug of War

For Tug of War, I was supposed to find a 4-universal hash function, using the one provided by processing token (j,c) where z<-z+c*h(j) and the output is z^2. 
Using the four_universal_Radamacher_hash_function function, then since this is similar to tidemark algorithm but contains negative, I believed that the algorithm and thus coding would be similar as well. The parameters were width and depth and the max of each parameters. Then, I would aggregate these two and get the outcome of z^2. 

3) BJKST

For BJKST, the algorithm was meant to have 2 universal hash function and hash the data into buckets where B is the first bucket and also calculates increasing z by one if |B|>=c/epsilon^2 (frequency estimation). Finally it is supposed to remove all the data in the first bucket B after and give an output of |B|2^z. 
So, I used the hash function from tidemark but from 0 to numBuckets_in - 1 since it cannot be negative. Then, there were 4 parameters since there were 4 calculations I had to do. First, I found to min, since we are looking for zeros(h(j))>=z. Then, I merged it for B<-B U {zeros((h(j))}. Then, I did the max function for the |B|>=c/epsilon^2. Finally, I did the z+1 for increasing the bucket number. Then I aggregated these together and used that number to find the output which is |B|2^z.

4) My code did not run properly so I could not run the program locally or on the GCP. However, I was hoping that I could get some partial credit by explaining my logic behind my 3 functions. 
However, I am assuming that with the median boosting trick, the Tug of War estimation should be off by (epsilon, delta) and the BJKST should be off by (epsilon, 1/3) estimates. 