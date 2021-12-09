# Loan Qualifier Application

This repository contains the code for a CLI application to match applicants with qualifying loans. The application analyzes loan data and evaluate user's profile based on their credit score debt, income, amount of loan requested, and property value.

## Technologies
The application is written in Python 3.9.7 and uses the following libraries:
-fire-0.4.0
-questionary-1.10.0

The application runs from the command line on Windows, Linux or Mac OS systems.


## Installation Guide

Download the repository code through GitHub and unpack the archive. Run the following commands to unstall all the dependencies:
```
pip install -r requirements.txt
```
## Usage
In the command line go to the folder containing the file 'app/py'.
For example:
```
cd/home/user/loan_qualifier_app
```

Run the CLI application by using the following command:
```
$ python app.py
```
Depending on your local Python interpreter, change 'python' to 'python3', if needed.

The first promt requests user to enter the path to a data file. Use the provided file 'data/daily_rate_sheet.csv' (Mac or Linus) and 'data\daily_rate_sheet.csv' (for Windows).

Answer the promt about the user's credit score, debt, income, loan amount, and home value. Once you enter user data, the application will filter and show you the available loans and display your monthly debt to income raio and loan to value ratios. If thereare available loans, the application will offer you an option to save the intformation to a file. If you want to save the informatio, press 'Y' or type 'yes' and the enter the file name. For example 'info' or 'available loans'.
The program will save loan details info a CSV file with the given name in the same folder.

```
$python app.py
? Enter a file path to a rate-sheet (.csv): data/daily_rate_sheet.csv
? What's your credit score? 700
? What's your current amount of monthly debt? 300
? What's your total monthly income? 2000
? What's your desired loan amount? 1000
? What's your home value? 35000
The monthly debt to income ratio is 0.15
The loan to value ratio is 0.03.
Found 11 qualifying loans
? Do you want to save the information about the qualifying loans? Yes
? Enter a file path to save the information: info
The information is saved into the info.csv file.
```
## Contributors
Project author : A.Rubkevich

Contact information : anastasiyarubkevich@github.com

## License
MIT License

Copyright (c) 2021