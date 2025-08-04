# Satsuma Automated Program

This is a Python script designed to automate token swaps on the Citrea testnet. The program performs a series of transactions, specifically a multi-step swap from USDC to WCBTC and then to SUMA. It features an interactive command-line interface (CLI) to configure and manage the transaction process.

## Features

-   **Automated Multi-Step Swaps:** Executes a chained swap from USDC -> WCBTC -> SUMA.
-   **Interactive CLI:** A user-friendly menu to start transactions, set the transaction count, or perform manual swaps.
-   **Configurable Transactions:** Allows the user to set the number of swaps to perform in each cycle.
-   **Randomized Swap Amounts:** Each swap uses a random amount of USDC between 0.0001 and 0.0002.
-   **Persistent Settings:** The transaction count is saved to a local file (`satsuma_config.json`) so it doesn't need to be reset each time.
-   **Detailed Logging:** Provides clear, color-coded logs of transaction statuses, balances, and confirmations.

## Installation

1.  **Clone the repository**
    First, clone the project from GitHub and navigate into the directory.

    ```bash
    git clone https://github.com/Chimalai/STM.git
    cd STM
    ```

2.  **Create and activate Virtual Environment**
    Create a Python virtual environment and activate it to manage dependencies.

    * On Windows:
        ```bash
        python -m venv venv
        .\venv\Scripts\activate
        ```
    * On macOS and Linux:
        ```bash
        python3 -m venv venv
        source venv/bin/activate
        ```

3.  **Install Dependencies**
    Install the required Python libraries.

    ```bash
    pip install web3 python-dotenv rich
    ```

4.  **Configure Environment Variables**
    Create a `.env` file in the project's root directory and add your private key. The script currently supports one private key.

    ```
    PRIVATE_KEY_1="your_private_key_here"
    ```

## Usage

To start the program, run the following command in your terminal:

```bash
python main.py
```

The program will display an interactive menu, allowing you to choose one of the following options:
 * Start Transactions: Runs the automated swap process based on the configured transaction count.
 * Set Transaction Count: Prompts you to set the number of transactions per cycle.
 * Manual Swap: Allows you to run a one-time swap with a specified number of transactions.
 * Exit: Closes the program.
Satsuma Automated Program
by @PetrukStar

