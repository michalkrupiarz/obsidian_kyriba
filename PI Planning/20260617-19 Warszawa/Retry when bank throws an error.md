Prerequisite [[message splitting]]

Scenario
1. There is a request for bank data
2. Something is wrong
3. We try to make a retry

Issues
1. When to retry
2. How to retry 
3. What to retry
4. What to present to user with [[error handling]]

Solutions
1. We will retry only based on set of http codes (it will be configurable so we can exclude or include set of http codes), and according to them. For Banks that return 200 with error code, we do not retry in MVP. For [[SPI]] we need to add additional things (to be confirmed).
2. Retry will happen as a strategy [[retry strategy]] for different http codes. By default it will be: retry after 1 min, 5 min, 15 min. It can be configured per bank or even per flow 
3. First step here is to have a [[message splitting]] so we have single account per response (to be confirmed). Then we can separate acounts that worked from ones that failed, and retry only those that failed

Needed solutions
1. When communication is triggered we have only one line to present outcome. 
2. What to present in monitor traces and how this communication will be shown there? 
3. Consider scenario when few accounts fail and we need to retry, how integration will work? I belive it is based on files created and put somwhere in kapp so it can be picked up by automatic job.