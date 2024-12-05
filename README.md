# Solana Distributor

[Solana Distributor](https://scripts.bebralabs.com/solana-distributor) is a powerful tool for distributing SOL to multiple addresses efficiently. Ideal for handling SOL airdrops and distributions to thousands of addresses quickly and with ease.

### Additional Links:
+ [Full documentation & video guide](https://splashy-celery-733.notion.site/Solana-Distributor-12a512669e1a80bb876bd355b6407c40?pvs=4)
+ [Buy with crypto](https://app.hel.io/pay/6751734ceb1b3674fc87c511)
+ [Buy with card](https://t.me/bebra_scripts/7)

## How to Use:

### 1. Install Solana CLI
Ensure that you have the Solana CLI installed on your system. Refer to the official guide for installation: [Solana CLI Installation](https://docs.solana.com/cli/install-solana-cli-tools).

### 2. Install Python
Download and install Python from the official website: [Python.org](https://www.python.org/). Make sure to add Python to the "PATH" during installation.

### 3. Install Dependencies
Open a terminal and run:
```bash
pip3 install base58
```

### 4. Connect Your Wallet to Solana CLI
There are a few ways to connect your wallet:
- Place your Solana wallet private key in the same folder as the script, saved as `key.json`. Then run:
  ```bash
  solana config set -k key.json
  ```
- If you don't have a `.json` keypair, run the connector script with:
  ```bash
  python3 connector.py <private_key>
  ```
  This script will generate a `key.json` file and automatically link it to the CLI.

### 5. Prepare the Recipient List
Create a CSV file named `send.csv` with the following format:
```csv
address,amount
EgKPanaYKEyFs1c91aNfqdXQeFJoAFKe2VVBHxSGSEV6,0.1
ACLwGYEoKZQej6aUJ8eM811YkjRwfvY4AiEsMTqKGNuh,1.5
```

### 6. Run the Script
Execute the script using the following command:
```bash
python3 send.py
```

### 7. Monitor Progress
The script will display real-time updates in the terminal, showing the status of each transfer. It also generates a file named `result.csv`, which logs the outcome of each transaction with the following fields:
- `address`
- `amount`
- `status` (`Success` or `Failed`)

---

**Tips for Use**:
- 💡 Always double-check the recipient addresses in the `send.csv` file to ensure accuracy.
- 🔒 Keep your wallet keys secure and never share them publicly.

---

Thank you for using Bebra Scripts. For support, contact us: [https://t.me/bebralabs_bot](https://t.me/bebralabs_bot)

**Web3 Development Services** – [https://t.me/bebralabs_bot](https://t.me/bebralabs_bot)

Created with ❤️ by **Bebra Labs**  
[https://bebralabs.com](https://bebralabs.com)

