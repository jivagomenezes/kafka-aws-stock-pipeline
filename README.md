
This project demonstrates a **real-time data ingestion pipeline** leveraging **Kafka** and **AWS services**. It fetches weather data from Lisbon using a weather API, buffers the data with Kafka, and processes it seamlessly into AWS for further analysis and storage.

---

## Key Features 🚀

- **Weather Data Fetching**: Retrieves real-time weather data from Lisbon via a public API.
- **Kafka Buffering**: Utilizes Kafka to handle and buffer the real-time data stream.
- **AWS Integration**:
    - Sends weather data to an **S3 bucket** for storage.
    - Enables SQL-like querying using **AWS Athena**.
    - Implements **IAM roles** for secure access to AWS resources.

---

## Pipeline Overview 🛠️

1. **Data Ingestion**: Fetch weather data via API.
2. **Buffering**: Stream the data through Kafka for processing.
3. **AWS S3**: Store the processed data in an S3 bucket.
4. **Query Execution**: Use AWS Athena to analyze the stored weather data.
5. **Secure Access**: Employ AWS IAM for secure and managed access to resources.

---

## Diagram 📊

![Kafka AWS Weather Pipeline](images/Kafka%20project.png)

---

## How to Use 💻

1. Clone the repository:
    
````bash
git clone https://github.com/yourusername/kafka-aws-weather-pipeline.git
````

1. Install dependencies:
    
````bash
    pip install -r requirements.txt
````
    
3. Run the producer to fetch and stream weather data:
````bash
  python producer.py
````
    
4. Start the Kafka consumer to process and store data in S3:
    
````bash
python consumer.py
````

---

## Prerequisites 📋

- **Kafka** installed and running (e.g., via Docker or a local setup).
- **AWS S3 Bucket** for data storage.
- **AWS Athena** for querying.
- Configured **IAM credentials** with permissions for S3 and Athena access.

---

## Why This Pipeline? 🌟

This project showcases the integration of real-time data processing tools (Kafka) with cloud-based analytics and storage solutions (AWS). It is a great starting point for:

- **Learning Kafka pipelines**.
- **Exploring AWS services like S3 and Athena**.
- Building scalable, real-time ingestion solutions.
