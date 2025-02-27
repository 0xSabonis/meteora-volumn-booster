# Solana Volume Bot on Raydium 

The **Solana Volume Bot** is designed to automate the distribution of SOL to multiple wallets and execute continuous buy and sell swap transactions on the **Raydium** platform. It utilizes Solana’s blockchain to perform these operations in a highly efficient and scalable manner.

## Features

- **Automated SOL Distribution**: Distribute SOL to new wallets automatically for seamless trading.
- **Continuous Buy and Sell Swaps**: The bot executes simultaneous buy and sell transactions without interruption.
- **Customizable Parameters**: Set buy amounts, intervals, wallet distribution, and other parameters to fit your needs.
- **Massive Buy Mode**: Execute large-scale buy operations across multiple wallets.
- **Sell Mode**: Gradually sell tokens in sub-wallets through controlled small transactions.
- **Token Pair Settings**: Configure token mint addresses and pool IDs for swap operations.
- **Logging**: Adjustable logging levels to help with monitoring and debugging the bot’s actions.

## Environment Variables

To configure the bot, define the following environment variables in a `.env` file:

```env
PRIVATE_KEY=                 # Private key for the main wallet
RPC_ENDPOINT=                # RPC endpoint for Solana
RPC_WEBSOCKET_ENDPOINT=      # RPC WebSocket endpoint for Solana

####### BUY SETTINGS #######
IS_RANDOM=true               # Enable random buy amounts
DISTRIBUTION_AMOUNT=0.01     # Amount of SOL to distribute to each wallet
BUY_AMOUNT=0.01              # Fixed buy amount for each transaction
BUY_UPPER_AMOUNT=0.002       # Upper limit for random buy amount
BUY_LOWER_AMOUNT=0.001       # Lower limit for random buy amount

BUY_INTERVAL_MAX=2000        # Maximum interval between buys in milliseconds
BUY_INTERVAL_MIN=4000        # Minimum interval between buys in milliseconds

CHECK_BAL_INTERVAL=3000      # Interval to check wallet balances in milliseconds
DISTRIBUTE_WALLET_NUM=8      # Number of wallets to distribute SOL to

SWAP_ROUTING=true            # Enable swap routing for token swaps

###### FOR MASSIVE BUY ######
WALLET_NUM=8                 # Number of wallets for massive buy operations

########## FOR SELL MODE ##########
SELL_ALL_BY_TIMES=20         # Number of times to sell tokens in sub-wallets gradually
SELL_PERCENT=100             # Percentage of tokens to sell from the main wallet

#### TOKEN PAIR SETTINGS ####
TOKEN_MINT=6VbEGuqwhjdgV9NxhMhvRkrFqXVNk53CvD7hK3C3yQS9  # Token mint address
POOL_ID=null                  # Pool ID for the token pair

TX_FEE=10                    # Transaction fee (in SOL)
ADDITIONAL_FEE=0.006         # Additional fee (greater than 0.006 SOL)
JITO_KEY=                    # Jito key (for transaction optimization)
JITO_FEE=120000              # Jito fee
BLOCKENGINE_URL=ny.mainnet.block-engine.jito.wtf  # Block engine URL

###### GENERAL SETTINGS ######
LOG_LEVEL=info               # Logging level (info, debug, error)
```


## 👤 Contact
- Telegram: Rizz Muffin[https://t.me/dogewhiz]
- GitHub: https://github.com/0xSabonis

