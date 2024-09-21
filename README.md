# Solana Token Airdrop Manager (STAM)

**Solana Token Airdrop Manager (STAM)** is an open-source tool designed to facilitate efficient and secure airdropping of SPL tokens on the Solana blockchain. Whether you're looking to distribute tokens to your community or incentivize participation in your decentralized project, STAM provides a seamless way to manage bulk token distributions to multiple wallet addresses.

## Key Features
- **Bulk Token Distribution**: Easily airdrop tokens to thousands of wallet addresses at once.
- **Optimized for Solana**: Leverages the Solana Program Library (SPL) standard for token transfers.
- **Customizable Airdrop Conditions**: Set specific amounts for each wallet or distribute tokens evenly.
- **Secure & Efficient**: Ensure token distributions are carried out securely with minimal transaction fees.
- **Developer-Friendly**: Straightforward setup and integration with your existing Solana project or workflow.

## Installation & Setup

### Prerequisites

- [Rust](https://www.rust-lang.org/tools/install) (Rust programming language)
- [Solana CLI](https://docs.solana.com/cli/install-solana-cli-tools) (Command Line Interface for interacting with Solana)

Ensure both Rust and Solana CLI are installed and configured on your system before proceeding.

### Step 1: Clone the Repository

Clone the project from GitHub:

```bash
git clone https://github.com/EncrypteDL/SolDrop.git
cd SolDrop
```

### Step 2: Install Rust Dependencies

```bash
cargo build
```

The dependencies are automatically managed by Cargo, Rust's package manager. The required packages are listed below:

### `Cargo.toml` Dependencies

```toml
[package]
name = "SolDrop"
version = "0.1.0"
edition = "2021"

[dependencies]
serde = "1.0"
serde_derive = "1.0"
proc-macro2 = "1.0"
quote = "1.0"
syn = "2.0"
unicode-ident = "1.0"
```

### Step 3: Run the Program

After building the project, you can run the program using:

```bash
cargo run
```

### Additional Notes

- Ensure your Solana CLI is set to the desired network (Devnet or Mainnet) using the following:

  ```bash
  solana config set --url https://api.devnet.solana.com
  ```

- You may want to set up a keypair and fund it with test SOL if using the Devnet:

  ```bash
  solana-keygen new --outfile ~/my-solana-wallet.json
  solana airdrop 2
  ```

