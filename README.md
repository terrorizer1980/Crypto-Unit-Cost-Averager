# Crypto-Unit-Cost-Averager

Automatically buy an amount of cryptocurreny (currently only Etherum) at regular intervals, to support [unit cost averaging](https://en.wikipedia.org/wiki/Dollar_cost_averaging) investment stratergy.


Written to run on Node.

`npm run start`

Create a gdaxrc. in this shape:
~~~json
{
    "url" : "https://api.gdax.com",
    "key" : "",
    "secret" : "",
    "passphrase" : "",
    "product" : "ETH-EUR", 
    "amount" : "10",
    "interval" : "1" 
}
~~~
You can generate an api key,secret and passphrase under your gdax [account](https://www.gdax.com/settings/api).
amount => is the amount you want to spend.
interval => is the intervals in hours you want to buy.


---

#####Future functionality backlog
- Buy more if the price is dropping
- Be able to buy Litecoin and Bitcoin
- Clear unfilled orders
- Add a UI - considering Vue.js
- Investigate sockets to buy on price drops without polling
- Phone notification when a purchase is made
- Withdraw money from exchange to wallet automically

