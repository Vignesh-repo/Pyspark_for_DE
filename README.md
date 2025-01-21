# Pyspark_for_DE
It's simple code example to demonstrate the basics of PySpark.
Data engineering plays a crucial role in processing and transforming large volumes of data. Apache Spark, an open-source big data processing framework, provides a powerful tool called PySpark that allows data engineers to work with big data using Python. PySpark combines the simplicity of Python with the scalability and speed of Spark, making it an excellent choice for data engineering tasks. In this guide, we will explore PySpark for data engineering beginners, requirements, and providing code examples to help you get started.
from pyspark.sql import SparkSession

We are going to do the 3 actions
Create a SparkSession, Create a DataFrame and Print the DataFrame


from pyspark.sql import SparkSession

 # Create a SparkSession
 spark = SparkSession.builder.appName("PySparkApp").getOrCreate()

 # Create a DataFrame
 data = [("Mustang","GT350",1997, 100000), ("BMW","X4",2010, 250000), ("Porsche","C911",1990, 180000)]

 df = spark.createDataFrame(data, ["Brand", "Model", "Year", "Price"])

 # Print the DataFrame
 df.show() 
  


 
 
