# TON CLI

[![Version npm](https://img.shields.io/npm/v/ton-cli.svg?logo=npm)](https://www.npmjs.com/package/ton-cli)

CLI client for TON.

## Features
- 🚀 Works anywhere and does not require to install local TON node
- 🔐 Encrypted storage of wallets
- 💸 Multiple wallets (even thousands of them if you wish)
- 🍰 Get balance
- ✈️ Transfers
- 💾 Unecnrypted backups that could be also used to import to other keystores if needed

## Install

```bash
npm install -g ton-cli
```

## How to use
Invoke `ton-cli` and follow wizard.
You can use flag --test to run client on test net instead of production.

```
# ton-cli
? Pick command
❯ Open keystore
  Create keystore
  Restore keystore
```

## Offline mode

`ton-cli` supports offline mode that could be enabled via:
* `--offline` argument
* `TON_CLI_OFFLINE=true` environment variable

## Performing transfers
When you have working keystore you have to write out contacts.json file in the same directory to be able to perform transfers in the form:

```
[
    {
        "name": "validator_0001",
        "address": "Ef9I0khL_IoN4UrmMFqNKhMZCTyKxroNCE_ajIesviF_S2bC"
    }
]
```

## Testing

Repository is bundled with test keystore and a wallet with a test coins for test (please, do not wipe it's balance).
Checkout current project and run `yarn cli` to start test client.

Test keystore password: 
```
sleep fan egg excess risk friend column remain seven bread disagree culture quick pride crush they ancient access flock settle prison kick tube word
```

# License

MIT
