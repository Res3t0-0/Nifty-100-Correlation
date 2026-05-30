# A Mini Project To Find Top 10 Most Correlated stocks in Nifty 100 Index
Here I used the help of yfinance, pandas and matplotlib to help me find the top 10 pairs of stocks. I also compared the performance Difference in pandas and numpy while calculating the volatility matrix. In pandas i used the help of .rolling().std() whereas in numpy i used the help of broadcasting.

### Why Broadcasting in NumPy?
* Its a concept i recently learned and i was curious to know if it would be faster than pandas despite it taking more memory.

# Correlation Matrix

<img width="835" height="846" alt="image" src="https://github.com/user-attachments/assets/cead0371-762d-4af8-ade1-afd8ef1f858d" />
<br><br>

Here are the top 10 pairs of stocks with their correlation values

| Ticker 1 | Ticker 2 | Correlation |
|:---|:---|---:|
| PFC.NS | RECLTD.NS | 0.955919 |
| ADANIPORTS.NS | AMBUJACEM.NS | 0.883742 |
| JINDALSTEL.NS | TATASTEEL.NS | 0.868333 |
| BPCL.NS | IOC.NS | 0.867992 |
| BANKBARODA.NS | CANBK.NS | 0.867185 |
| ADANIENT.NS | ADANIPORTS.NS | 0.856324 |
| JSWSTEEL.NS | TATASTEEL.NS | 0.855271 |
| BANKBARODA.NS | SBIN.NS | 0.852140 |
| JINDALSTEL.NS | JSWSTEEL.NS | 0.849071 |
| GAIL.NS | NTPC.NS | 0.846679 |

### Proofs of Correlation:

<img width="786" height="784" alt="image" src="https://github.com/user-attachments/assets/0b3d9267-3f1d-4550-b4ea-651b24ce193c" />

<img width="786" height="784" alt="image" src="https://github.com/user-attachments/assets/536b6b98-4347-47de-a981-4f4915e08745" />

# Performance Analysis

<img width="531" height="72" alt="Screenshot From 2026-05-30 18-22-45" src="https://github.com/user-attachments/assets/d2eb356d-4c0f-4400-aa19-a0e9c084d808" />

We can understand from the above image that Using Pandas was faster than NumPy Broadcasting method. This is due to the fact that pandas uses Cpython optimized c code in the background and also since the broadcasting method creates a huge 3D array to calculate the matrix.

### Note:
* There maybe faster methods in numpy to calculate the volatility matrix. But this Project is based on my curiosity.
