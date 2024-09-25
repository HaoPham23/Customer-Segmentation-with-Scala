Model to Segment customers based on their previous purchase history. We use the RFM Analysis and K-means clustering techniques to cluster similar customers and use Apache Spark to code our model.The dataset used here is the Ecommerce data provided in kaggle: https://www.kaggle.com/carrie1/ecommerce-data/ . One issue i faced with the dataset is that the date format provided for the InvoiceDate column could not be processed in spark, i was not sure it was due my environment issue so i used a python script(provided in this repo) to reformat the InvoiceDate.

# Prerequisites
- [Scala](https://www.scala-lang.org/download/)
- [Apache Spark](https://www.apache.org/dyn/closer.lua/spark/spark-3.5.3/spark-3.5.3-bin-hadoop3.tgz)

# Steps to run

1. Clone the repository
2. Change the value `retailDataHomeDir` in `src/main/scala/Segmentation.scala` to the path of repo
2. Run `sbt` in the root directory of the project
3. Run `run` in the sbt shell