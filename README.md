0# Data Analyst Challenge

We're providing you with a simplified csv file of transactions that merchants have made with REPAY 
over a certain period of time. 

| date       | merchant| return_code  |
|------------|---------|----|
| 2019-01-01 | 3899978 | 1  |
| 2019-01-01 | 1005527 | 0  |
| 2019-01-01 | 3899978 | 0  |
| 2019-01-01 | 1005527 | 0  |
| 2019-01-01 | 1002349 | 1  |
| 2019-01-01 | 1005527 | 40 |
| 2019-01-01 | 1005527 | 0  |

Possible transaction return codes are as follows:
- 0,  transaction approved
- 1,  transaction declined, insufficient funds
- 21, transaction declined, card reported stolen
- 36, transaction declined, improper format
- 40, transaction declined, unknown reason

There is a profit margin associated with each return code:
- 0, 10 cents
- 1, -5 cents
- 21, 0 cents
- 36, -7 cents
- 40, -2 cents

Please demonstrate SQL queries to generate tables that show the following :

- Number of transactions, approvals, and total declines for each day
- Number of approval codes for each merchant for each day
- Total profit for each merchant for each day

As a final exercise in story telling:

One of our merchants (1005527), has contacted us with concerns that their most recent sets of transactions 
have been off. Using the provided data, help us investigate if this is the case. Feel free to use any tools 
or skills at your disposal to make a simple report on whether their perception might be real. 

