Roughly speaking the process of the bot is as follows
1. Use websockets to livestream data from the Uniswap V2 factory contract
2. Set up notifications for the hash of PairCreated() events
3. When a new PairCreated() event is detected pull the hash values of each token
4. Most likely one token will not be considered trust worthy and will need to be investigated.
5. Investigate risk factors such as liquidity locking and the creator of the new token
6. In the event that the new token is considered trust worthy, execute the trade

Code available upon request
