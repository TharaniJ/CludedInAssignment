1. Load raw data from company.csv file.
   
3. Create profile report for the raw data.
   libraries used : ydata-profiling(main library) and pandas
   
5. Complete the data Cleansing for the Company.csv file.
   3.1 Findout the total duplicate rows in the docuemnt.
   3.2 Strip whitespace from column names and listdown the company names.
   3.3 Standardize country names to Title Case.
   3.4 Remove invalid values from 'RegAddress.Country' column.
   3.5 Remove invalid values from 'CountryOfOrigin' column.
   3.6 Replace common invalid/missing entries with real NaN.
   3.7 Convert date columns to datetime format.
   3.8 Fill missing values in Country column.
   libraries used : pycountry, pandas, numpy

7. Complete the Deduplication for the Company.csv file
   Remove duplicate records based on Company Name and PostCode

8. Generate the report by Calculateing the total missing values and percentage.

9. Removing Duplicate Rows using Deduplication function
    
11. Validate each record against Companies House database using REST API
    11.1 Navigate to the "Companies House Rest API" page
    11.2 Register with email and create a login for the page
    11.3 Go to create application and create an application in 'Live' environment.
    11.4 get the "API key" and use it to accesss the data from the page.
    11.5 Function to validate each company number
    11.6 Add a flag if its a valid companies and available in the page.
    11.7 Display the result in a data frame.
    libraries used : requests, pandas, requests.auth.HTTPBasicAuth

13. validate data using API and Company.csv, make a flag if the validation is correct, Entrich the usefu information from API.
    libraries used : requests.auth.HTTPBasicAuth, requests, numpy, time
    
15. Generate reports using charts and diagrams for the visualization
    15.1 Get the Total, valid and invalid company numbers.
    15.1 Generate Pie Chart for the Valid vs Invalid companies.
    15.3 Generate Bar Chart for the Company Status (active, dissolved etc.)
    15.4 Generate Year-wise Incorporation (When companies were created)
    libraries used : matplotlib.pyplot and seaborn

17. Export the final enriched and validated dataframe into a CSV file

18. Sending a Final report to a email.
    18.1 Visit 'myaccount.google.com' and create app password
    18.2 Email server details
    18.3 Create the email message
    18.4 Specify the path to the CSV file
    18.5 Attach the CSV file to the email
    18.6 Set up the SMTP server and send the email
    libraries used :smtplib, email.mime.multipart.MIMEMultipart, email.mime.base.MIMEBase, email.mime.text.MIMEText, email.encoders,os
