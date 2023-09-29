FAST Faculty Data Extraction & Analysis

This project involves web scraping data from the websites of three campuses of FAST University (Lahore, Islamabad, and Karachi) to collect information about the faculty members. The collected data is then transformed into structured data frames, concatenated into a single data frame, and analyzed. The primary objectives are to extract faculty details, create a comprehensive dataset, and generate a random sample for analysis.

Step 1: Web Scraping
In the first step, we analyze the structure of faculty pages for each campus to collect the following details for each faculty member:

ID: An identifier for each faculty member.
Name: Full name of the faculty member.
Designation: The position or job title of the faculty member.
HEC Approved: A Boolean indicating if the faculty member is HEC approved.
Highest Education: The highest educational qualification of the faculty member.
Email: The email address of the faculty member.
Department: The department to which the faculty member belongs.
Extension: The contact extension or phone number of the faculty member.
Image URL: The URL of the faculty member's image.
PHD Supervisor: A string indicating if the faculty member is a PHD supervisor.
This data is collected for all faculty members in the Lahore, Islamabad, and Karachi campuses and is stored in separate CSV files: lhr.csv, isb.csv, and khi.csv.

Step 2: Data Concatenation
In the second step, we concatenate the data frames from the three campuses into a single data frame named "fast_faculty.csv." This consolidated dataset contains information about all faculty members across the three campuses.

Step 3: Data Sampling
In the final step, we load the "fast_faculty.csv" data frame into a variable named "faculty." We then apply a sampling method to create a random sample of the faculty dataset. The sampling fraction is determined by dividing the last digit of the student's ID by 10. If the last digit is 0, the sampling fraction remains as is (0.1).

The resulting sample data frame is named "sample_" and is saved as a CSV file named "sample.csv" for further analysis.
