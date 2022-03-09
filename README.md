# Hiking-Route-in-Hong-Kong-
The problem I define is https://www.hiking.gov.hk/trail, a government official website, sharing the hiking routes and information about hiking in Hong Kong.  In the code, I scrape the webpage in English, finding titles and useful elements. I scrape all the information about hiking routes. It includes the hiking trail names, districts, difficulties, rating, and descriptions.

In the code, I scrape the webpage in English, finding titles and useful elements. I scrape all the
information about hiking routes. It includes the hiking trail names, districts, difficulties, rating, and
descriptions.

However, the difficulties and rating of trails are in the same class on the webpage. I use the for loop
and conditional statements to separate the elements by identifying the word “stars” as difficulties.
Meanwhile, there are “\n” and several spaces at the beginning of the descriptions. I use for loop
again to beautify the trail descriptions.

I create a data frame that shares the information of the hiking trails with the output as a CSV file.
There are 5 columns (without index) and 129 rows, meaning that there are 129 trails in total. Each
column represents trails’ name, district, difficulties (with five as full marks), ratings (with five as full
marks), and descriptions. Each row means each trail. It is sorted by the trail names in alphabetical
order, the same as the webpage.

Despite that, there are still some bugs in the data frame. First, the number of symbols of hearts or
stars might be different from that in text. For example, there are only three hearts in ratings of
Aberdeen Tree Walk, but it has written “Rating 4-Heart”, reducing the accuracy of the data. Also, the
descriptions of the trails end with “...”, which has not shown the complete description but only a
summary.
