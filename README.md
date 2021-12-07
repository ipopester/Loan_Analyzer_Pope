# Loan Qualifier Application

This is an application designed to facilitate the loan selection process, which based on the user's core financial information, such as debt, home value, and credit score. Applicants often want to know whether their criteria meet those of  potential lenders. This application produces a list of qualifying lenders with the option to save the result as a csv file.

## Technologies

This application was written using python 3.7 and is designed to be executed through a CLI (command line interface), such as Terminal (MacOS) or GitBash (Windows). Below are the critical dependencies used and associated documentation:

* [python](https://www.python.org/downloads/) 3.7.11 

* [questionary](https://www.python.org/downloads/) 1.10.0

* [fire](https://google.github.io/python-fire/guide/) 0.4.0
___

## Installation Guide

Before running the application, make sure that a python development environment has been activated in the CLI. 

Install the following dependencies:

```python
    pip install fire
    pip install questionary
```

The primary python file in this application is app.py
___

## Usage

To use the loan qualifier application, clone the repo using the link on GitHub. Then run  `app.py` in the CLI using the following command:

```python
    python app.py
```

Upon running this code the user will be asked to enter the file path to the rate-sheet containing the list of banks and loan qualifications:

![Initial prompt from the application](https://raw.githubusercontent.com/ipopester/Loan_Analyzer_Pope/main/images/Initial_CLI_Prompt_Loan_Qualifier.png)

After entering in a file path, the user will be asked to provide the financial information for the applicant:

![Prompt for applicant's financial data](https://raw.githubusercontent.com/ipopester/Loan_Analyzer_Pope/main/images/Prompt_Applicant_Data_Loan_Qualifier.png)

The application runs a series of filters to determine which banks would be willing to offer a loan based on the applicant's financial information. Based on the results, there are two outcomes:

1. If no qualifying loans exist, the program closes.
2. If there are qualifying loans, the user is given the option whether to save the file as a csv.

To save the result in the data folder:

```python
    ./results/
```
A message confirming that the results have been saved will appear in the CLI:

```python
    A csv file of qualifying loans has been created.
```

## Contributors

Ian Pope: iancpope@uw.edu

## License

Copyright (c) (2021) (Ian Pope)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
