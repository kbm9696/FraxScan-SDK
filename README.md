
# Fraxtal Python SDK

Welcome to the Fraxtal Python SDK! This library provides a simple interface for interacting with the Fraxtal blockchain, making it easy to build blockchain-based applications in Python. The SDK is available as a PIP package for easy installation and usage.

## Installation

You can install the Fraxtal Python SDK using pip:

```bash
pip install FraxScanSDK
Package Url: https://pypi.org/project/FraxScanSDK/1.0.1/
```
## Access APIS
```bash
from FraxScanSDK import FraxScanApis
accounts = FraxScanApis.AccountsApi()
accounts.set_api_key_token(api_key='YSHJE758IWYISKUY3JRB4EVQEDE2BBVZJC')
response = accounts.get_frxETH_balance(address='0xe7c147cd1a7c05a6e73217645547582024e87a9b')
print(response)
```

## Features

The SDK provides the following functionalities:

### Accounts

This module allows you to manage blockchain accounts. You can create new accounts, retrieve account details, and manage private keys securely. It provides an easy way to handle account-related operations, such as checking balances and generating new addresses.

### Transactions

With the Transactions module, you can create, sign, and send transactions on the Fraxtal blockchain. It supports constructing transactions with various parameters, ensuring they are properly formatted and broadcasted to the network. This module simplifies the process of transferring assets and interacting with contracts through transactions.

### Blocks

The Blocks module allows you to retrieve information about blocks on the Fraxtal blockchain. You can get details of a specific block by its number or hash, and subscribe to new block events. This is useful for applications that need to monitor blockchain activity or validate transaction confirmations.

### Geth Proxy

The Geth Proxy module allows you to interact with a Geth (Go Ethereum) node via JSON-RPC. It provides lower-level access to the Fraxtal blockchain, enabling you to perform various network and node operations that are not covered by the higher-level modules. This is useful for advanced users who need direct interaction with the node.

### Tokens

The Tokens module simplifies the management and interaction with tokens on the Fraxtal blockchain. It supports standard token types like ERC-20 and ERC-721, allowing you to perform operations such as token transfers, balance checks, and token creation. This module abstracts the complexities involved in token operations.

### Stats

The Stats module provides various statistics and metrics about the Fraxtal blockchain. You can retrieve information about the network status, transaction counts, block times, and other relevant data. This is useful for monitoring the health and performance of the blockchain network.

## Contributing

We welcome contributions to the Fraxtal Python SDK! Please open issues or pull requests on the [GitHub repository](https://github.com/yourusername/fraxtal-sdk).

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

