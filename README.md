# Advanced Financial Analytics System

Welcome to the Advanced Financial Analytics System, designed to provide deep insights into financial markets, with a particular focus on forex markets. This project leverages historical data and economic indicators to forecast movements in forex rates, especially the EURUSD pair, and integrates financial news sentiment to enhance predictions.

## Project Overview

The project aims to blend quantitative financial analysis with machine learning and data science techniques to predict forex market trends and provide actionable insights. It specifically focuses on the EURUSD currency pair, exploring correlations between macroeconomic indicators and market movements.

## Project Structure

- `/data` - Contains datasets used in the project, including historical EURUSD rates and economic indicators.
- `/docs` - Documentation and additional resources related to the project.
- `/models` - Predictive models developed for forecasting currency movements.
- `/notebooks` - Jupyter notebooks for exploratory data analysis, model development, and visualisation.
- `/scripts` - Automation scripts for data collection, preprocessing, and model evaluation.

## Key Features (Planned)

The following key features are planned for implementation in this project. They are designed to provide comprehensive insights into forex market trends, particularly focusing on the EURUSD pair:

- **Time Series Analysis**: Utilising ARIMA and LSTM models to predict future forex rates based on historical data.
- **Sentiment Analysis**: Integrating sentiment analysis techniques to assess market sentiment from global financial news and its impact on forex prices.
- **Economic Indicator Analysis**: Examining the influence of major economic announcements and indicators on forex markets.
- **Data Visualisation**: Developing interactive dashboards using Plotly/Dash for real-time data visualisation and analysis.

These features are in the planning stage and may evolve as the project progresses. Check back for updates as I advance through the development stages.

## Documentation
This project is documented thoroughly to ensure ease of use and scalability. Below are links to detailed documentation on various components of the project:

- [AWS RDS Setup Guide](docs/AWS-RDS-Setup.md): Detailed setup and configuration information for the Amazon RDS instance used in this project (transitioned to free resources (local PostgreSQL) to manage costs while maintaining full project functionality).
- [AWS S3 Setup Guide](docs/AWS-S3-Setup.md): Configuration details and security measures implemented for Amazon S3 storage used in the project.
- [AWS Lambda Automate Data Fetching Documentation](docs/AWS-Lambda-Automate-Data-Fetching.md): Detailed documentation on the setup, implementation, and challenges faced with AWS Lambda for automating data fetching.

## Getting Started

This section will guide you through the process of setting up your local environment to run the Advanced Financial Analytics System. Follow these instructions to get started.

### Prerequisites

Before you begin, ensure that you have Python installed on your system. You will also need several dependencies, which can be installed using the following command:

```bash
pip install -r requirements.txt
````
## Installation
### Clone the Repository
Start by cloning the repository to your local machine. Replace `yourusername` with your GitHub username and adjust the repository name if it's different:

```bash
git clone https://github.com/yourusername/advanced-financial-analytics-system.git
cd advanced-financial-analytics-system
```
### Set Up Python Environment
It is recommended to use a virtual environment for Python projects to manage dependencies effectively. Here's how you can set it up:

```bash
# Create a virtual environment (Unix/macOS)
python3 -m venv venv
source venv/bin/activate

# Create a virtual environment (Windows)
python -m venv venv
.\venv\Scripts\activate
```
### Install Dependencies
With your virtual environment activated, install the project dependencies by running:

```bash
pip install -r requirements.txt
```
### Environment Configuration
To fully utilise the project's capabilities, set up necessary environment variables:

1.Create a `.env` file in the project root:
```plaintext
touch .env  # Unix/macOS
type nul > .env  # Windows
```

2. Add required environment variables to the `.env` file. For example:
```plaintext
OANDA_API_KEY=your_actual_api_key_here
DB_HOST=your_db_host
DB_NAME=your_db_name
DB_USER=your_db_user
DB_PASS=your_db_password
DB_PORT=your_db_port
```
Replace your_actual_api_key_here with the API key obtained from your data provider, such as OANDA. Also, update your db connection credentials.

### Running the application
Once everything is set up, you can fetch the data by running:
```bash
python fetch_data.py
```
This will fetch the data according to the configurations specified in your environment variables and `.env` file.

## Contact
**Developer Contact**: As the sole developer and maintainer of this project, please direct any inquiries or feedback directly to me. You can reach me through my GitHub profile.

## License

This project is licensed under the MIT License. The license allows for free use, modification, and distribution of the software for any purpose, including commercial purposes, subject to the conditions listed below.

### Terms of the MIT License

Copyright (c) 2024 AyyaduraiAgalya

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

- The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

### Further Information

For more details on the MIT License, please visit [MIT License Information](https://opensource.org/licenses/MIT).

