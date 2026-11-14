
# Project Background

We have a requirement where we need update the latest USD exchange rates every day and log them into Google Sheets. This sheet will be then be used in Power BI dashboard to dynamically convert values using up to date rates. Hence eliminating the dependency on static numbers.

# Assumptions and Caveats

- Exchange rates are updated to google sheets only.
- Make.com application is used as low code bridge linking the exchange rate website and google sheets.

# Thought process

- We start by thinking how would do this manually - open a browser, search for exchange rate webiste and then copy paste them on to the google sheets.
- We will make sure the data collected is clean, timestamped and formatted.
- We will let flow run once in the background without needing to be attended.

# Solution Design

- A trigger that starts the flow automatically everyday.
- Process to fetch the exchange rates from the website.
- Final step to add the rates to google sheets in a clean format.

# Outcome

- Every day, the scenario runs and logs the latest exchange rate to your sheet.  
- Power BI always uses the most recent value, no more hardcoded conversions. 
- About 30 minutes of time is saved, errors avoided, and stays up to date automatically.

![Outcome](Images/Screenshot%202026-11-12%20011849.png)
![Outcome](Images/Screenshot%202026-11-12%20011953.png)
