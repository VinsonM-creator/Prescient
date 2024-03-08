# Prescient
Prescient Securities .NET Developer Assessment
# Overview
The ExcelToDatabase application is a .NET C# console application designed to download Excel files from a specified URL, process each file, read its contents, and save contract details to a SQL database. It utilizes the Microsoft.Interop.Excel library to handle Excel file operations and interacts with a SQL database to store contract details.
# Features
Download Excel files from a specified URL.
Read Excel file contents and extract contract details.
Save contract details to a SQL database.
Prevent duplicate entries in the database by tracking processed files.
Generate a report of total contracts traded within a specified date range.
# Prerequisites
Microsoft .NET Core Runtime or SDK
Microsoft Office installed (for Microsoft.Interop.Excel)
SQL Server Management Studio or any SQL client
# Installation
Clone or download the repository to your local machine.
Open the solution in Visual Studio or any compatible IDE.
Build the solution to restore dependencies and compile the application.
# Usage
1. Downloading Excel Files
- Run the application executable or execute the console application.
- The application will automatically download Excel files from the specified URL to the local folder.
2. Processing Excel Files
- After downloading the Excel files, the application will process each file.
- It reads the contents of each Excel file and saves contract details to the SQL database.
3. Generating Report
- Execute the stored procedure [dbo].[SP_Total_Contracts_Traded_Report] in your SQL Server Management Studio or SQL client.
= Provide the @DateFrom and @DateTo parameters to specify the date range.
= The stored procedure will return a table with columns [File Date], [Contract], [Contracts Traded], and % Of Total Contracts Traded.
# Configuration
Update the connection string in the application configuration file (app.config) to point to your SQL database.
Customize the URL for downloading Excel files and adjust file processing logic as needed.
# Contributing
Contributions are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request.

# License
This project is licensed under the MIT License.

# Acknowledgments
This application was developed as a solution to a programming task.
