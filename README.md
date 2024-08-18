<img width="900" alt="30 Jul - Navigating the DeFi Ecosystem" src="https://github.com/user-attachments/assets/f4166974-50f5-400f-b084-5b95428f48ed">

# Quest 3 - Execute a Token Swap 🦄

Welcome to Quest 3 of the **Navigating the DeFi Ecosystem** campaign, where we will execute a token swap on Uniswap!

## Pre-requisites

Before you begin, do ensure you have the following installed on your system:

- Git
- Node.js

## Project Setup ⚙️

1. Clone the repository

```bash
git clone https://github.com/clement-stackup/token_swap.git
```

2. Navigate to the project directory:

```bash
cd token_swap
```

3. Install the necessary dependencies & libraries

```bash
npm install --save
```

<!-- ADDED BY CRENSHAW - UPDATE TO TOKEN SWWAP (UNISWAP AND AAVE) -->>

This README section accurately describes the functions and steps for interacting with the Aave protocol as outlined in the provided code snippets.

The provided functions demonstrate exactly how to expand the utility of the swapped LINK tokens by opening a supply position on Aave to earn interest. This process showcases the integration and composability of different DeFi protocols.

The workflow is as follows:

First, we use the getLendingPool function to retrieve the current Aave lending pool address.

Then, we call the approveAave function to grant permission for the Aave protocol to spend the LINK tokens we obtained from the Uniswap swap.

Finally, we use the depositToAave function to actually supply the LINK tokens to the Aave protocol, opening a supply position that will start earning interest.

## PART F - Get Aave Lending Pool

In this step, we retrieve the address of the Aave lending pool:

1. Locate the `getLendingPool` function in `index.js`.
2. This function uses the LendingPoolAddressesProvider contract to get the current lending pool address.
3. It returns the address of the active Aave lending pool.

## PART G - Approve Aave to Spend LINK

Here we approve the Aave protocol to spend LINK tokens:

1. Find the `approveAave` function in `index.js`.
2. This function approves the Aave lending pool to spend a specified amount of LINK tokens.
3. It creates an approval transaction and sends it using the provided wallet.
4. The function logs the transaction details and confirmation.

## PART H - Deposit LINK into Aave

Finally, we deposit LINK tokens into the Aave protocol:

1. Locate the `depositToAave` function in `index.js`.
2. This function interacts with the Aave lending pool contract to supply LINK tokens.
3. It creates a deposit transaction with the specified amount of LINK.
4. The function sends the transaction and logs the details and confirmation.

To execute these steps:

1. Ensure your `.env` file is set up with the necessary private key and RPC URL.
2. Open a terminal in the project directory.
3. Run the script using: `node index.js`.
4. The script will perform the Aave-related operations and display transaction details.
5. Verify the deposits by checking the provided Etherscan links or your Aave dashboard.

Troubleshooting:

- If you encounter errors, verify that you have sufficient LINK tokens and ETH for gas fees.
- Ensure all contract addresses and ABIs are correct and up-to-date.
- Check that you have the necessary permissions to interact with the Aave protocol on the Sepolia network.

Now that you're set up, you're ready to start the quest! 🏁 Follow the steps as outlined in the campaign. Each step contains detailed instructions to guide you through the process. 📜

Happy questing~ 🎉
