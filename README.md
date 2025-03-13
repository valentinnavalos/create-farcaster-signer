## Installation

**Install project dependencies**

   ```bash
   npm install
   ```

**Configure env vars**:
   - Copy the example environment file:
     ```bash
     cp .env.example .env
     ```
   - Edit `.env` to add your `NEYNAR_API_KEY` and `FARCASTER_DEVELOPER_MNEMONIC` (your warpcast recovery phrase).


## Create Farcaster Signer

**Generate a Signer** 

   ```bash
   npm get-approved-signer
   ```

**Approve the signer generated**

Needed: a browser wallet with funded roughly $2 worth of OP ETH on the Optimism mainnet.

1. Go to Farcaster optimism explorer
https://optimistic.etherscan.io/address/0x00000000fc56947c7e7183f8ca4b62398caadf0b#writeContract

2. Connect your wallet to the OP explorer.

3. Navigate to `addFor` function and add following values inside the respective placeholders. You will see values for fidOwner, keyType, key, metadataType, metadata, deadline, sig in your terminal logs.

4. Press "Write" to execute the transaction. This will create a signer for your mnemonic on the OP mainnet.
