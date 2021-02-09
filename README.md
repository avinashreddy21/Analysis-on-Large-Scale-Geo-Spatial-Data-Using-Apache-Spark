# Analysis-on-Large-Scale-Geo-Spatial-Data-Using-Apache-Spark-and-Scala

This project aims at solving one of the most challenging large-scale data challenges - working on Geo-spacial data using Apache Spark. 
We use Geo-spatial statistics to help get significant clusters (or deviations) for the spatial data. Identifying such statistically significant clusters is also very commonly known as ’Hot Spot’ Analysis. 
One common metric for identifying the most significant clusters or hot spot cells in time and space is by using the Getis-Ord statistic tti∗. 
The reason we use Apache Spark for this project is because Spark is a high-performance distributed computing framework, which allows us to tackle big-data problems by distributing the workload across a cluster of machines. 
[Mak16] [Sal+16] Large scale data analysis tasks typically runs into several problems, for example, low CPU memory, sometimes taking months to solve a real- world problem. 
Apache Spark is also an open source big data processing framework built for speed and ease of use as well as sophisticated analytics.


In this project, you need to write two User Defined Functions ST_Contains and ST_Within in SparkSQL and use them to do four spatial queries:

Range query: Use ST_Contains. Given a query rectangle R and a set of points P, find all the points within R.
Range join query: Use ST_Contains. Given a set of Rectangles R and a set of Points S, find all (Point, Rectangle) pairs such that the point is within the rectangle.
Distance query: Use ST_Within. Given a point location P and distance D in km, find all points that lie within a distance D from P
Distance join query: Use ST_Within. Given a set of Points S1 and a set of Points S2 and a distance D in km, find all (s1, s2) pairs such that s1 is within a distance D from s2 (i.e., s1 belongs to S1 and s2 belongs to S2).
A Scala SparkSQL code template is given. You must start from the template. A Scala SparkSQL code template is given. You must start from the template. The main code is in "SparkSQLExample.scala"
