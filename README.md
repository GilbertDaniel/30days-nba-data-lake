# NBA Data Lake on AWS

This project is part of the DevOps Challenge and focuses on creating an NBA Data Lake for analytics. It uses AWS services to build an efficient workflow for storing, processing, and querying NBA player data.

## Features

- **Data Storage**: Stores raw NBA player data in JSON format in Amazon S3.
- **Data Cataloging**: AWS Glue is used to define the schema and catalog the data.
- **Data Querying**: Amazon Athena enables querying data directly from the S3 bucket.
- **Serverless Architecture**: The project leverages AWS cloud-native services to minimize infrastructure overhead.

## Technologies Used

- **Amazon S3**: Secure and scalable storage for raw data.
- **AWS Glue**: Simplifies data preparation with schema definition and data cataloging.
- **Amazon Athena**: Provides a serverless way to query the data.
- **Python**: Automates the setup and processing of AWS services.
- **python-dotenv**: Manages environment variables securely.

## Installation and Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/GilbertDaniel/30days-nba-data-lake.git
   cd 30days-nba-data-lake
   ```

2. **Set Up Environment Variables**:
   - Create a `.env` file in the project directory.
   - Add the following variables:
     ```env
     SPORTS_DATA_API_KEY=your-api-keys
     NBA_ENDPOINT=https://api.sportsdata.io/v3/nba/scores/json/Players
     ```

3. **Query Data Using Athena**:
   - Open the AWS Management Console and navigate to Amazon Athena.
   - Use the Glue table to run SQL queries on the NBA data.

## Key Takeaways

- **Data Lake Architecture**: Combines S3, Glue, and Athena for efficient analytics workflows.
- **Automation**: Python scripts streamline the setup and management of AWS resources.
- **Security**: Environment variables and IAM policies ensure secure and efficient operations.
- **Serverless Analytics**: Leverages Glue and Athena for scalable and cost-effective data querying.

## Future Enhancements

- Automate data ingestion with AWS Lambda and EventBridge.
- Visualize the data with Amazon QuickSight.
- Add support for multiple data formats (e.g., CSV, Parquet).

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

Feel free to contribute by opening issues or submitting pull requests to enhance the project!
