# HIPIN-BOT

An automated bot for managing PinAI accounts, handling daily tasks, and automatic model upgrades.

## Features

- Automatic token management and renewal
- Daily check-in automation
- Automatic coin collection
- Automatic model upgrades when sufficient points are available
- Multi-account support
- Token expiration monitoring
- Detailed logging system
- Multi-Account Proxy

## Prerequisites

- Node.js (v14 or higher)
- npm (Node Package Manager)
- A Telegram account

## Installation

1. Clone this repository:

```bash
git clone https://github.com/ByteBeggar/HIPIN-BOT.git
cd HIPIN-BOT
```

2. Install dependencies:

```bash
npm install
```

## Configuration

### 1. Register on PinAI:

- Visit this link to register: [PinAI Registration](https://t.me/hi_PIN_bot/app?startapp=p5vLl1t)
- After registration, copy the initialization data

### 2. Set Up data.txt:

- Edit `data.txt` file in the project root
- Add your initialization data (one account per line)

Example `data.txt` format:

```
user=
query_id=
```

## Usage

Run the bot:

```bash
node nidex.js
```
## No Proxy
Run the bot:

```bash
node index-proxy.js
```

The bot will automatically:

- Check and renew tokens if needed
- Perform daily check-ins
- Collect available coins
- Upgrade models when possible
- Run tasks every 24 hours

## Logging

The application uses Winston for logging with the following levels:

- ERROR: For error messages
- WARN: For warnings
- INFO: For general information

Logs include timestamps and are displayed in the console.

## Token Management

Tokens are automatically managed and stored in `token.json`. The bot will:

- Check token validity
- Refresh expired tokens
- Store tokens securely

