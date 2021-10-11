# Hashtables Introduction
## By Tong Wang and Xin Ai

<img src="https://github.com/tong-sf/msds610_final/blob/main/imagesforreadme/slide_image1.png" width="500" height="400"/>

In the real world, we always need to extract information from millions of records. However, the most common searching method, linear search, is not sufficient in such a situation. Then we need hashtables, which partitions the search space into many regions (termed as buckets) and assigns values to the corresponding regions using the modulo operator. If we want to search a specific value from that, we just need to do a linear search within the target bucket after locating it, instead of going through the whole dataset. Thus we can find the desired value efficiently:

<img src="https://github.com/tong-sf/msds610_final/blob/main/imagesforreadme/slides_image2.png" width="800" height="400"/>

If we use time complexity to compare the efficiency of the linear search and the hashtable search, it is obvious that the time complexity of hashtable search O[n/b] (n is the length of the dataset and b is the number of buckets) is much better than the time complexity of linear search O[n].

Hash search entails creating the hashtable and perform linear search inside the specific bucket in the hashtable. To implement a hashtable, the followings are the main procedures:
1. Create empty lists (buckets) based on how we generate the hashcode.
2. Allocate the data into the corresponding buckets.

There are two situations included in this introduction:
* Searching for integers: We generate the hashcode based on the integer.
* Searching for strings: We use ord() function to extract the unicode of the first character of the string, then generate the hashcode.

# Slides and Code
* Hashtables_Slides.pdf:  It contains the slides we used in our presentation. We introduce the reasons that why we should use hashtables in searching.
* Hashtables_Introduction.ipynb: It presents the fundamental steps for implementing hashtables and hash search on integers and strings. We also use the lolviz package to illustrate the idea of hashtables as the following:

<img src="https://github.com/tong-sf/msds610_final/blob/main/imagesforreadme/code_image.png" width="800" height="500"/>

# Summary
Hash table is a very useful data structure for us to search information from millions of records, and hash search can help us increase the searching efficiency significantly. In the process of implementing hash search, the most important step is to construct the hashtable based on the method in which we decide to generate the hashcode.

