# auction_anhcor_solana
This is the anchor implementation for solana-auction.

-> Run

# Build the solana program

npm run build

# Run validator on the localnet

npm run validator

# Get 10 SOL by airdrop and deploy program for localnet.

npm run deploy

# Run the auction. The specification is same as solana-auction

npm run test

# Tips

The solana-auction uses Pubkey::Default for highestBidderPubkey and highestBidderFtTempPubkey and highestBidderFtReturningPubkey as default.

But the anchor-auction uses exhibitor's main account and token account.
This is because the anchor checks account owner strictly.
The owner of the highestBidderPubkey and highestBidderFtTempPubkey must be TokenProgram because they are TokenAccount.


