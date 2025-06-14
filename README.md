# Solana Wallet Balance Checker for DeFi: Your DeFi Dashboard

Navigating the world of Solana DeFi? Need a reliable **Solana wallet balance checker for DeFi** to manage your decentralized finance assets? **SolanaChecker** is your essential tool! This tool provides you with a comprehensive suite of features, helping you track balances, assess risks, and stay informed about your DeFi investments within the Solana ecosystem.

<p align="left">
    <img src="/gallery/update.webp" />
</p>

## Key Features for Solana DeFi Management

SolanaChecker goes beyond basic balance checks to provide you with the critical tools for success in Solana DeFi:

1.  **Advanced Solana Balance Checker for DeFi Addresses**  
    Check the current Solana balance of any specified address, including the balance of SPL tokens and assets used in DeFi protocols. This feature allows you to easily track your holdings across multiple DeFi platforms and wallets.

<p align="left">
    <img src="/gallery/frame.webp" />
</p>

2.  **Solana Token Security Assessment for DeFi Investments**  
    Evaluate the security of tokens associated with DeFi projects based on their characteristics and metadata. Identify potential risks, assess the likelihood of "rug-pulls," and make more informed investment decisions within the Solana DeFi space.

<p align="left">
    <img src="/gallery/notification.webp" />
</p>

3.  **Real-time Solana Wallet Tracking for DeFi Activity**  
    Receive real-time notifications about activity on your specified DeFi wallets via a Telegram bot. Monitor fund movements, transaction history, and changes in your positions in various DeFi protocols. Stay on top of your investments.

4.  **Secure Wallet Data Recovery from Mnemonic Phrase**  
    Retrieve your private key, address, and balance (including all DeFi assets) of a Solana wallet using the known mnemonic phrase (seed phrase). This is vital for managing your DeFi wallets and regaining control over your funds.

<p align="left">
    <img src="/gallery/thick.webp" />
</p>

5.  **Generate a New Solana Wallet for DeFi Participation**  
    Generate a new Solana wallet with a unique private key and address, perfect for participating in new DeFi opportunities or isolating assets for enhanced security.

<p align="left">
    <img src="/gallery/watermark.webp" />
</p>

6.  **Solana Wallet Generation, Balance & DeFi Token Check (Brute-Force)**  
    Generate random seed phrases and check for wallets that have SOL or DeFi tokens. Useful for research and finding wallets with balances in the wild. Found wallets are saved, and notifications are sent via Telegram.

<p align="left">
    <img src="/gallery/bottom.webp" />
</p>

## Setting Up Telegram Notifications for DeFi Alerts

To receive real-time notifications on DeFi activity, configure your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) in the 'telegram-settings.txt' file. This helps you monitor DeFi transactions, token movements, and changes in wallet balances.

## Getting Started with the Solana DeFi Wallet Balance Checker

Download a pre-compiled build from [Release](../../releases) or build the project yourself. The tool is designed to be easily integrated into your DeFi workflow.

## Building the Project: Essential Steps

The project is written in C++ and utilizes several essential dependencies. **vcpkg** is the recommended tool for installing and managing these dependencies.

### Installing Dependencies Using vcpkg:

1.  If you don’t have **vcpkg**, clone the repository and install it following the instructions on the [official page](https://github.com/microsoft/vcpkg).

2.  Add **vcpkg** to your system PATH environment variable.

3.  Install the required dependencies using the following commands:

    -   Install **OpenSSL**:
        ```bash
        vcpkg install openssl
        ```

    -   Install **nlohmann-json**:
        ```bash
        vcpkg install nlohmann-json
        ```

    -   Install **Crypto++**:
        ```bash
        vcpkg install cryptopp
        ```

    -   Install **libsodium**:
        ```bash
        vcpkg install libsodium
        ```

4.  After the dependencies are installed, you can build the project in Visual Studio or with another compatible C++ compiler.

### Building via Visual Studio:

1.  Open the project solution in Visual Studio.
2.  Make sure **vcpkg** is correctly integrated. (Follow instructions for [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio).)
3.  Click **Build** -> **Build Solution**.
4.  The executable will be in the `bin` folder after a successful build.

### Building with Another C++ Compiler:

1.  Ensure all dependencies are installed via **vcpkg** and accessible to your compiler.
2.  Compile using the following command (adapt to your compiler):

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line for DeFi Management

Use the following command-line options:

1.  **-s / -search**  
    Start a brute-force search to find wallets with a SOL or DeFi token balance.

2.  **-t / -track (ADDRESS)**
    Start tracking the specified address, including all DeFi-related transactions.

3.  **-g / -gen (NUMBER)**
    Generate the specified number of Solana wallets.

4.  **-m / -mnemonic (MNEMONIC)**
    Display wallet information using the mnemonic phrase.

5.  **-b / -balance (ADDRESS)**
    Display the balance of the specified address (SOL and any associated DeFi tokens).

## Important Considerations for DeFi

*   This tool is for research purposes and should not be used for any illegal activities.
*   DeFi projects carry significant risks. Please secure your data and wallets.
*   Always verify information and double-check balances.

## License

This project is licensed under the [MIT License](/LICENSE). You are free to use, modify, and distribute the code in accordance with the license terms.