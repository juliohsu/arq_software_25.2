# How to run sales_generator.py (locust script)

![Apache Flink E-Commerce Analytics with Elasticsearch and Postgres](architecture_img.png)

Install Locust: pip install locust.

Run it with: locust -f sales_generator.py --host=http://your-kafka-endpoint.

Adjust the --users and --spawn-rate parameters (e.g., --users 100 --spawn-rate 50 to start with 50 users/sec, scaling up to 100) to control the event rate.

Ensure your endpoint (e.g., a Kafka producer API) accepts POST requests with JSON data.