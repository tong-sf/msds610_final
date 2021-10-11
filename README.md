# Hashtables Introduction
## By Tong Wang and Xin Ai

In the real world, we always need to extract information from millions of records. However, the most common searching method, linear search, is not sufficient in such a situation. Then we need a Hash Table, which partitions the search space into many regions (termed as buckets) and assigns values to the corresponding regions using the modulo operator. If we want to search a specific value from that, we just need to do a linear search within the target bucket after locating it, instead of going through the whole dataset. Thus we can find the desired value efficiently.

![Alt](https://github.com/tong-sf/msds610_final/blob/main/imagesforreadme/slides_image2.png)

If we use time complexity to compare the efficiency of the linear search and the hashtable search, it is obvious that the time complexity of hashtable search O[n/b] (n is the length of the dataset and b is the number of buckets) is much better than the time complexity of linear search O[n].

# Code
In 

![Alt](https://github.com/tong-sf/msds610_final/blob/main/imagesforreadme/code_image.png)

