# NoSQL-Project
# Twitter Data Streaming and Real-time Analysis

This project aims to build a data pipeline that streams live Twitter data, processes it using Apache Spark, stores it in MongoDB for persistence, and visualizes trending topics in real time. 

## Getting Started

Follow these steps to get the project up and running on your local machine.

### Prerequisites

Ensure you have the following installed on your local system:

- Jupyter Notebook
- Apache Spark
- MongoDB
- Python 3.x
- Required Python libraries: `pandas`, `pyspark`, `tweepy`, and `matplotlib`

Also, please make sure to set up Twitter API credentials by creating a Twitter application.

### Running the Project

1. **Start the server socket:** Run the `tweetRead.ipynb` notebook. This will start a server socket that listens for incoming tweets.

2. **Spark Streaming and MongoDB storing:** Run the `sparkStreamingMongodb.ipynb` notebook. This will start processing the incoming tweets using Spark Streaming and store them in MongoDB. Alternatively, you can run `spark.ipynb` to process the incoming tweets using Spark only.

3. **Batch Processing:** Run the `batchProcessing.ipynb` notebook to visualize the data stored in MongoDB.

4. **Spark-submit:** Run the `sparkMongo.py` script using the following command:

```bash
spark-submit --jars org.mongodb.spark_mongo-spark-connector_2.11-2.4.0.jar,mongo-java-driver-3.9.0.jar sparkMongo.py
```

## Authors

1. Anand Prakash (IMT2020040)
2. Ayushmaan Singh (IMT2020126)
3. Vanshvardhan Singh (IMT2020010)

## Acknowledgments

- Thanks to the creators of Tweepy, Apache Spark, MongoDB, and Python for their tools.
