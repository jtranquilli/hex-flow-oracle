Keys are omitted from this repository, as are spot trading API interactions but the code is fairly redundant anyway.
1. Use websockets to livestream data through QuickNode from the Uniswap V2 factory contract
2. Set up event notifications for the hashcode of PairCreated() events
3. When a new PairCreated() event is detected pull the hash values of each token
4. Most likely one token will not be considered trust worthy and will need to be investigated.
5. Ensure liquidity is locked for the less trustworthy token
6. Investigate risk factors to reduce likelihood of honeypot/rug-pull
7. In the event that the new token is considered "trustworthy" execute the trade according to risk tolerance

