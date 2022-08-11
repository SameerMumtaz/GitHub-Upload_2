# GitHub-Upload_2

---

# Project Title

This is a python command-line interface application that allows users to see qualifying loans from lenders quickly and easily. The application works by taking in a `daily_rate_sheet` of loan criteria from various loan providers, asking the user a number of questions to evaluate their loan eligibility, and then returning to them a list of qualifying loans.

---

## Technologies

This program was wrtten using Python 3.9.12, along with the Python modules/libraries: questionary, fire, and pandas. 

The Fire library is used to allow the user to dynamically input values. 
(https://github.com/google/python-fire)

The Questionary module is used to enable the user to interact with various functions, using the CLI.
(https://github.com/tmbo/questionary)

---

## Installation Guide

Prior to running the provided code, the user MUST install the Fire and Questionary modules by running:

pip install fire

pip install questionary

---

## Usage

The code is relatively straightforward, to access this program/application, simply input: python app.py into your GitBash or Terminal
You will then be prompted by five questionaries, which the user must provide answers to. Here are the questionaries:
    
    credit_score = questionary.text("What's your credit score?").ask()
    debt = questionary.text("What's your current amount of monthly debt?").ask()
    income = questionary.text("What's your total monthly income?").ask()
    loan_amount = questionary.text("What's your desired loan amount?").ask()
    home_value = questionary.text("What's your home value?").ask()
You, as the user, must simply input the values of each which pertains to you, then enable the application to begin filtering out loans from a csv file provided, according to what you do and don't qualify for, based on the values you previously entered.
![Loan Qualifier Prompts](Images/loan_qalifier.png)

---

## Contributors

Sameer Mumtaz
sm@ampexbrands.com

---

## License

MIT
