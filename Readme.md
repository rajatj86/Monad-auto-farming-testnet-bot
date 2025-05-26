Monad Testnet Automation Bot
A user-friendly GUI-based bot for automating interactions on the Monad Testnet, including contract deployment, staking/unstaking, token swapping, voting, and wallet generation.
Prerequisites

Python 3.8+
Node.js (for PM2, optional)
Monad Testnet wallet with MON tokens

Setup

Navigate to the project directory:
cd monad-bot


Install dependencies:



Running the Bot

First Run (Foreground):
python main.py

 This opens the GUI. Enter your private key (kept in memory, not saved) and contract addresses as needed. Click buttons to perform actions.

Usage

Load Wallet: Enter your private key in the GUI and click "Load Wallet".
Enter Contract Address: For staking, swapping, or voting, input the target contract address.
Perform Actions: Click buttons to deploy contracts, stake/unstake MON, swap tokens, vote, or generate new wallets. Confirm each transaction in the pop-up.
View Logs: The output log displays transaction details and errors.

Security Notes

Private keys are not stored on disk.
Transactions require user confirmation.
Balance checks prevent wallet draining.
Always verify contract addresses before interacting.

Troubleshooting

RPC Connection Issues: Ensure internet connectivity and try again.
Insufficient Balance: Fund your wallet with MON tokens.
Invalid Contract Address: Verify the contract address on the Monad Testnet explorer.

Credits

Developed by [Rajat]

