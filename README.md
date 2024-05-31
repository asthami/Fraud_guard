Fraud_Guard - Real-Time Payment Fraud Detection API on Google Cloud

Here’s a brief overview of our deployed API, demonstrating how it assesses fraud probabilities for a given User-ID using three Deep Learning Models. These models were fine-tuned for recall, precision, and accuracy to address various use cases.

Demonstration Video: Demonstration_of_The_Three_models.mp4

BASIC FLOW:

Input the User-ID of an existing user from our graph database.
The API connects to the Neo4j Graph Database to retrieve user features.
The three models then provide the probability of the User being fraudulent based on these graphical features. (For more details, refer to the report.)
USE CASES:

Our system employs three distinct models tailored to different types of payment transactions:

General Transactional Model :

Suitable for payment gateways handling a wide range of transaction types, from large money transfers to small daily purchases.
Balances accuracy and coverage, ensuring reliable performance across various transaction sizes.
Large Transaction Fraud Detection Model :

Designed for gateways dealing with large transactions.
Focuses on catching potential fraud while minimizing false alarms.
Employs an optimized setup to reduce missed fraud cases and includes tools for quick problem resolution.
Precision-focused Model for Small Transactions :

Tailored for gateways processing numerous small transactions.
Prioritizes accuracy to avoid unnecessary flags, crucial for maintaining customer trust and operational efficiency given the high transaction volume.
These models can be used individually or in combination, depending on business needs. By offering tailored solutions, our system ensures secure transactions while maintaining customer satisfaction.

Deployment:

The API was deployed on Google Cloud using Docker and ML Cloud Run.
Deployment has been paused to avoid continuous billing charges.
For further details on model summaries, performance, and dataset exploration using the Neo4j Graph Database and Python libraries, please refer to the project report:

Project Report