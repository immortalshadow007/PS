<h1 align="center">
  PolygonScan Scraper Discord bot
  <br>
</h1>

<h4 align="center">Crypto signals, transactions monitoring, price alerts, scrape data from blockchain</h4>

<p align="center">
  <a href="#overview">Overview</a>
  •
  <a href="#setup">Setup</a>
  •  
  <a href="#commands">Commands</a>
  •
  <a href="#license">License</a>
</p>

# Overview

A Discord bot that uses the [Polygonscan API](https://polygonscan.com/apis), [Disnake](https://docs.disnake.dev/en/stable/) library to provide access to various blockchain data and functionality, such as querying the state of a contract, retrieving transaction history, or submitting transactions. 

PolygonScan Scraper Discord does not require any administrative privileges nor store any data.

### Scopes
- Bot.
- Application dependent on user commands.

### Required bot permissions by admins
- Send Messages
- Embed Links
- Attach Files

# Setup
The bot has additional features such as monitoring crypto wallets for incoming transactions and price change alerts. To properly setup run the next commands:

- ``` ps-set_wallet_address <wallet>``` Set set crypto wallet to monitor for new changes
- ``` ps-set_transaction_channel <your_transaction_channel_id``` Set channel to get incoming transaction as a message.
- ``` ps-set_price_alert_channel <your_price_alert_channel_id``` Set channel to get alerts for new price changes.
- ``` ps-set_signal_pair ``` Set crypto pair with USDT to fetch data from Binance and generate the crypto signal

Full access to the bot can be unlocked by one-time payment through the PayPal payment gateway. Upgradable functionalities, such as returning CSV files, scrapping up to 1000 transactions, and much more.

# Commands

Prefix command: ```ps-```

- ```ps-ping```  Return bot latency. 
- ```ps-help``` List all commands.
- ```ps-help <command>``` More info on a command
- ```ps-donate``` Display how to donate information
- ```ps-creator``` Returns a contract's deployer address and transaction hash it was created, up to >= 5 at a time
- ```ps-gas``` Returns the current Safe, Proposed, and Fast gas prices
- ```ps-abi``` Returns the contract Application Binary Interface ( ABI ) of a verified smart contract.
- ```ps-getTrxHash <transaction hash>``` Return a link for specific transaction hash. 
- ```ps-getTrx <wallet address> <offset>``` Return a list of normal transactions of a specific address.
- ```ps-getTokenHolder <token_smart_contract>``` Return 1000 holders of specific ERC20 token.
- ```ps-getBalance <wallet address>``` Get amount in MATIC for single address. 
- ```ps-getErc20 <wallet address> <contract address> <offset>``` Return list of ERC-20 transactions, can be filtered by specific smart contract address. 
- ```ps-getErc721 <wallet address> <contract address> <offset>``` Return list of ERC-721 (NFT) transactions, can be filtered by specific smart contract address. 
- ```ps-getErc1115 <wallet address> <contract address> <offset>``` Return list of ERC-721 (NFT) transactions, can be filtered by specific smart contract address

# License

Released under the [GNU GPL v3](https://www.gnu.org/licenses/gpl-3.0.en.html) license.
