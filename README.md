# Hashtables Introduction
## By Tong Wang and Xin Ai

![Alt](https://github.com/tong-sf/msds610_final/blob/main/imagesforreadme/slides_image1.png)
In the real world, we always need to extract information from millions of records. However, the most common searching method, linear search, is not sufficient in such a situation. Then we need a Hash Table, which partitions the search space into many regions (termed as buckets) and assigns values to the corresponding regions using the modulo operator. If we want to search a specific value from that, we just need to do a linear search within the target bucket after locating it, instead of going through the whole dataset. Thus we can find the desired value efficiently:

![Alt](https://github.com/tong-sf/msds610_final/blob/main/imagesforreadme/slides_image2.png)

If we use time complexity to compare the efficiency of the linear search and the hashtable search, it is obvious that the time complexity of hashtable search O[n/b] (n is the length of the dataset and b is the number of buckets) is much better than the time complexity of linear search O[n].

# Slides and Code
Hashtables_Slides.pdf contains the slides we used in our presentation. In Hashtables_Introduction.ipynb in this repository, we present the fundamental steps for implementing hashtables and hashsearch on integers and strings. We also use lolviz package to illustrate the idea of hashtables:

![Alt](https://github.com/tong-sf/msds610_final/blob/main/imagesforreadme/code_image.png)

# Summary
Hashtables are used to significantly increase the searching efficiency. In the process of implementing hash search, the most important step is to construct the hashtable based on the method in which we decide to generate the hashcode.

