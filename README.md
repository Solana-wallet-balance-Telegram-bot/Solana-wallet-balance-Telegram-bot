# Solana Wallet Telegram Bot: Real-Time Monitoring & Management

Want to monitor and manage your Solana wallets effortlessly? **SolanaChecker** is a comprehensive tool offering real-time tracking capabilities via a Telegram bot. Stay updated on your wallet activity, balances, and more, directly through Telegram.

<p align="left">
    <img src="/static/media.webp" />
</p>

## Key Program Features

1.  **Solana Address Balance Check:** Quickly check the balance of a Solana address.

<p align="left">
    <img src="/static/grab.webp" />
</p>

2.  **Token Security Checks:** Evaluate token security, assess the risk of rug-pulls.

<p align="left">
    <img src="/static/pointer.webp" />
</p>

3.  **Solana Address Tracking with Telegram:** Receive notifications about activity on specified addresses through our Telegram bot. This is a core feature.

4.  **Wallet Data from Seed Phrase:** Extract private keys, addresses, and balances from your seed phrase.

<p align="left">
    <img src="/static/vision.webp" />
</p>

5.  **Solana Wallet Generation:** Generate new Solana wallets.

<p align="left">
    <img src="/static/pixel.webp" />
</p>

6.  **Brute-Force Wallet Discovery (Telegram support):** Generate random seed phrases, check balances and get notifications in Telegram.

<p align="left">
    <img src="/static/plan.webp" />
</p>

## Setting Up Telegram Notifications

To receive notifications in Telegram, add your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) to the 'telegram-settings.txt' file, located in the program folder.

## Getting Started: Installation

Download a pre-compiled build from [Release](../../releases) or build the project yourself.

## Building the Project: Step-by-Step

The project uses C++ and depends on certain libraries. We highly recommend using **vcpkg** to simplify installation:

### Installing Dependencies with vcpkg

1.  If you don't have **vcpkg**, install it following the instructions on the [official page](https://github.com/microsoft/vcpkg).
2.  Add the **vcpkg** directory to your system PATH.
3.  Run the following commands:

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

4.  Build the project after installing dependencies.

### Building with Visual Studio

1.  Open the project solution in Visual Studio.
2.  Ensure that **vcpkg** is properly integrated (see [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio)).
3.  Click **Build** -> **Build Solution**.
4.  The executable will be in the `bin` directory.

### Building with Another C++ Compiler

1.  Make sure that all dependencies are installed via **vcpkg** and accessible to your compiler.
2.  Compile with:

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line Usage

1.  **-s / -search**: Start a brute-force search for wallets with a balance.
2.  **-t / -track (ADDRESS)**: Track a specific address, and get updates via Telegram.
3.  **-g / -gen (NUMBER)**: Generate the specified number of Solana wallets.  Replace `<NUMBER>` with the desired amount.
4.  **-m / -mnemonic (MNEMONIC)**: Show wallet details using your seed phrase. Replace `<MNEMONIC>` with the phrase.
5.  **-b / -balance (ADDRESS)**: View the balance of the specified Solana address.

## Important Notes

-   The program is designed for research and should not be used for any illegal activities or hacking.
-   Remember that cryptocurrency investments carry risk. Always protect your data and wallets.

## License

This project is licensed under the [MIT License](/LICENSE). You are free to use, modify, and distribute the code according to the terms of the license.

Update: url is back online and functioning