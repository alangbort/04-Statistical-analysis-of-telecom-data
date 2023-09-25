# Statistical analysis of telecom data

## Objective
Clients were offered two tariff plans: "Smart" and "Ultra". In order to adjust the advertising budget, the commercial department wanted to understand which tariff brings in more money

## Description
The data of 500 users of the Company was available: who they were, where they came from, what tariff they used, how many calls and messages each of them sent in 2018. We needed to analyze customer behavior and concluded which tariff was better

## Data
The following data on **users, calls, messages, internet sessions and tariffs** were available:
- Table **Users** - information about users:
  - **user_id** - unique user identifier
  - **first_name** - user's first name
  - **last_name** - user's last name
  - **age** - user's age (years)
  - **reg_date** - date of tariff activation (day, month, year)
  - **churn_date** - date of tariff termination (if the value is missing, it means that the tariff was still in effect at the moment of data upload)
  - **city** - city of user's residence
  - **tarif** - tariff plan name
 
- Table **Calls** - information about calls:
  - **id** - unique number of the call
  - **call_date** - date of call
  - **duration** - duration of the call in minutes
  - **user_id** - identifier of the user who made the call

- Table **Messages** - information about messages:
  - **id** - unique call number
  - **message_date** - date of the message
  - **user_id** - identifier of the user who sent the message

- Table **Internet** - information about internet sessions:
  - **id** - unique session number
  - **mb_used** - amount of Internet traffic spent during the session (in megabytes)
  - **session_date** - date of internet session
  - **user_id** - user identifier

- Table **Tariffs** - information about tariffs:
  - **tariff_name** - tariff name
  - **rub_monthly_fee** - monthly subscription fee in rubles
  - **minutes_included** - number of minutes per month included in the subscription fee
  - **messages_included** - number of messages per month included in the subscription fee
  - **mb_per_month_included** - amount of Internet traffic included in the subscription fee (in megabytes)
  - **rub_per_minute** - cost of a minute of talk time in excess of the tariff package (for example, if the tariff includes 100 minutes of talk time per month, then 101 minutes will be charged)
  - **rub_per_message** - cost of sending a message in excess of the tariff package
  - **rub_per_gb** - cost of additional gigabyte of Internet traffic over the tariff package (1 gigabyte = 1024 megabytes).

## Technology Stack
Python, Pandas, Matplotlib, Seaborn, Scipy
