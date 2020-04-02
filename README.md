# spark
Jupyter notebooks for Apache Spark

## Installing Apache Spark
1) Check that Java SDK is installed typing `java -version`in a terminal, which should return something like `openjdk version "1.8.0_242"`
2) Download Spark from https://spark.apache.org/downloads.html, selecting pre-built for Hadoop.
3) Unzip the .tgz archive, rename the folder 'spark' and move it to the user's home (so, the full path is `~/spark`)
4) Add the to the environmental variables:
	* Execute `nano ~/.bashrc` 
	* Add the following lines at the end:
		SPARK_HOME=~/spark
		export PATH=$SPARK_HOME/bin:$PATH
		export PYSPARK_DRIVER_PYTHON=jupyter
		export PYSPARK_DRIVER_PYTHON_OPTS='notebook'
	* Execute `source ~/.bashrc`
	* Restart computer to ensure effectiveness of changes
5) Execute `pyspark` in any terminal window
