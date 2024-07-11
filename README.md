# starknet-etl

An ETL tool to Extract, Transform, Load starknet data

## Architecture

[docs/arch.jpg](docs/arch.jpg)

The architecture depicted in the image illustrates a data pipeline that transforms raw blockchain data into actionable insights through the following stages:

### 0. ETL (Extract, Transform, Load):

- **Full-Archive Node**: The process starts with data extraction from full-archive nodes of various blockchain networks (such as Ethereum, Binance Smart Chain, and Bitcoin).
- **RPC (Remote Procedure Call)**: The extracted data is communicated via RPC to be processed.
- **CSV & Python**: The raw data is then transformed into CSV format using Python scripts. This transformation step prepares the data for further storage and analysis.

### Data Warehouse:

- **Storage Solutions**: The processed data is stored in a data warehouse, which includes databases, file systems, and other storage solutions. The data warehouse acts as a central repository for all the transformed data.
- **Data Aggregation**: The data warehouse aggregates data from various sources, ensuring it is organized and accessible for analysis.

### Insight:

- **Visualization and Dashboarding**: The final stage involves generating insights from the stored data. This is achieved through visualization tools and dashboards that allow users to monitor and analyze the data.
- **Analysis**: The insights generated can be used to make informed decisions, identify trends, and optimize operations based on the analyzed data.

### Automation:

- **Manual & Bots**: The architecture also incorporates both manual inputs and automated bots to interact with the data at various stages. Bots can handle repetitive tasks, while manual processes ensure data quality and address exceptions.
