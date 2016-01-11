###Lesson 18: Big Data

####Slides
- [ Lesson 18 Slides ](lec18.pdf)

####Handouts
- [PySpark](https://github.com/pburkard88/DS_BOS_07/blob/master/Notebooks/18_PySpark.ipynb)

####Spark Installation:
If you'd like to follow along with the Spark notebook you can attempt to install Spark locally so that you can run the PySpark manipulations (these instructions are for a Mac only, Windows could be tricky...).

1. Install Spark on your Mac by running the following: `brew install apache-spark`
2. Install findspark: `pip install -e .` after cloning it from [here](https://github.com/minrk/findspark), and `cd findspark`)
3. Install the Java JDK from [here](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html)
4. Now when you start an IPython NB, you should have all the tools you need to go find your local Spark installation and interact with it via PySpark.  To create a SparkContext within your notebook, you'll have to run something like the following within the notebook:
<pre><code>import findspark
import os
findspark.init()
import pyspark
sc = pyspark.SparkContext()</code></pre>