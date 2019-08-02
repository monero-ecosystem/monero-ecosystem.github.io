---
layout: post
title: 'MoneroTipsBot'
repo_name: 'MoneroTipper'
description: 'An on-chain, non-custodial, Reddit Monero tip bot written in Python.'
introduction: 'An on-chain, non-custodial, Reddit Monero tip bot written in Python.'
date: 2019-08-02 00:00:00
maintainer: 'dginovker'
maintainer_uid: '32943174'
main-class: 'utility'
tags:
- dginovker
- monero-python
image: 
---

An open-source, non-custodial, on-chain tipping service.
====================

Brought to you by the /r/Monero community.

See tips in action [here](https://www.reddit.com/user/Monerotipsbot).

*****

## How to use

\>\>\> **DO NOT** store more Monero than you're willing to lose <<<

*****

### Creating a Wallet, Checking your Balance & Public Address

[(Click here!)](https://www.reddit.com/message/compose/?to=MoneroTipsBot&subject=My%20info&message=Hit%20%27send%27%20and%20the%20bot%20will%20tell%20you%20your%20balance%20:\))


### Tipping

`/u/MoneroTipsBot <amount> XMR` will tip whoever you replied to the amount! For example, commenting `/u/MoneroTipsBot 0.25 XMR. Thanks for the tutorial!!` will send whoever you've just replied to 0.25 XMR from your wallet.

### Withdrawing

[(Click here!)](https://www.reddit.com/message/compose/?to=MoneroTipsBot&subject=Withdraw%200%20XMR&message=Replace%20this%20line%20with%20your%20public%20address!)

To withdraw any part of your balance, PM /u/MoneroTipsBot with the subject as `Withdraw <amount> XMR` and the message as just your address. For example, messaging /u/MoneroTipsBot `Withdraw 0.75 XMR` with the message content `44AFFq5kSiGBoZ4NMDwYtN18obc8AemS33DBLWs3H7otXft3XjrpDtQGv7SqSsaBYBb98uNbr2VBBEt7f2wfn3RVGQBEP3A` will withdraw 0.75 Monero to that address.

*(Warning: withdrawals cannot be reversed once they are done!)*

### Anonymous tips

[(Click here!)](https://www.reddit.com/message/compose/?to=MoneroTipsBot&subject=Anonymous%20tip%20MoneroTipsBot%200%20XMR&message=Replace%20this%20line%20with%20your%20message%20!)

To make an anonymous tip to any Reddit use, PM /u/MoneroTipsBot with the subject as `Anonymous tip USER <amount> XMR`, with any message you want to deliver alongside. For example, messaging /u/MoneroTipsBot `Anonymous tip fluffyponyza 5 XMR` with an empty body will tip /u/fluffyponyza 5 Monero, without any hint of who sent it!

### Extracting your private key

**Warning: If you share your private key with anyone, you may lose your funds.**

[(Click here!)](https://www.reddit.com/message/compose/?to=MoneroTipsBot&subject=My%20private%20info&message=I%20understand%20this%20will%20give%20me%20my%20PRIVATE%20key%20that%20can%20be%20used%20to%20access%20my%20funds.)

If you're sure you understand what your private key can do, and how to use it, PM /u/MoneroTipsBot with the subject `My private info`. The bot will reply displaying your public address, total balance, and your private key (mnemonic) which you can use to export funds/import into another wallet.


### Donating to the CCS

*https://ccs.getmonero.org*

Monero uses community crowdfunding to fundraise developers. You can donate directly to it from here!

**Donation:**

Percent of your balance | [100%](https://www.reddit.com/message/compose/?to=MoneroTipsBot&subject=Donate%20100%%20of%20my%20balance&message=Hit%20%27send%27%20to%20donate%20100%%20of%20your%20balance%20to%20the%20CCS.) | [75%](https://www.reddit.com/message/compose/?to=MoneroTipsBot&subject=Donate%2075%%20of%20my%20balance&message=Hit%20%27send%27%20to%20donate%2075%%20of%20your%20balance%20to%20the%20CCS.) | [50%](https://www.reddit.com/message/compose/?to=MoneroTipsBot&subject=Donate%2050%%20of%20my%20balance&message=Hit%20%27send%27%20to%20donate%2050%%20of%20your%20balance%20to%20the%20CCS.) | [25%](https://www.reddit.com/message/compose/?to=MoneroTipsBot&subject=Donate%2025%%20of%20my%20balance&message=Hit%20%27send%27%20to%20donate%2025%%20of%20your%20balance%20to%20the%20CCS.)
:--|:--|:--|:--|:--
[Custom amount of XMR](https://www.reddit.com/message/compose/?to=MoneroTipsBot&subject=Donate%200%20XMR&message=Hit%20%27send%27%20to%20donate%20the%20amount%20of%20Monero%20in%20the%20subject%20line%20to%20the%20general%20dev%20fund) | | | |

[Make an anonymous donation](https://www.reddit.com/message/compose/?to=MoneroTipsBot&subject=Withdraw%200%20XMR&message=46zarwyDHd8F2GXxVuETVz3wKvEnWic634eYykBS9Q6UbmQfm2y7XRt45KzF6rGT1Pj9YTp55iHRKXZsR7AaxDZM7XqtYRK)

**Top Donators**

Username | Amount
:--|:--
/u/outerspacerace | 0.100000 XMR
/u/OsrsNeedsF2P | 0.089653 XMR
Anonymous | 0.0684099 XMR


*****

## F.A.Q.

*****

### Is this real Monero!?!?!?

Yup! Don't lose it!

### Someone sent me a tip! How can I withdraw it for money?

This depends on few factors, such as what country you're from and how much you've received. For large amounts, you can use any [Exchange](https://www.getmonero.org/community/merchants) that supports Monero, or for smaller amounts, it may be easier to spend at [Merchants & Services](https://www.getmonero.org/community/merchants) that accept Monero instead.

### Why is all my Monero unconfirmed? I want to send more tips!

Monero works by sending your Monero to a destination, then all the return "change" back to yourself. This means if you only ever received Monero from 1 source, you can only make 1 transaction at a time.

The easiest and quickest way to fix this problem is to wait a bit, then *tip yourself* your full balance. This will split your balance into 6 inputs, which should be enough to get going again!

### How much Monero is too much?

Consider any Monero you put on the tipper service spent. While you can always retrieve it (if you wrote down your private key), the purpose of the service is to tip others; so you should not put anything on it that you are not comfortable with completely losing.

### Do you own a copy of my private key?

Yes!! So don't store too much. While it is stored encrypted on the service, until someone can figure out how I can circumvent this I'll have access to your keys and funds. So don't store more than you're willing to lose, and back up your private key in case the service ever goes down!

### Is it open source?

Absolutely! The code is free to learn from, copy or redistribute and is available on Github [here](https://github.com/dginovker/MoneroTipper).

### How can I verify transactions are occurring on-chain?

After a successful tip, you can take the tx key and input it to a Monero block explorer, such as [MoneroBlocks](https://moneroblocks.info/). Since Monero is private, the amount and addresses are hidden, but you can still verify the transaction took place, and verify further details by exporting your private key and looking it up in a local wallet.

*****

## Version history:

- 0.1: Initial release, testnet only
- 0.2: Security and bugfixes
- 0.3: Output splitting enhancements
- 0.4: Logging and CCS donations
- 0.5: Better RPC handling
- 0.6: Mainnet release
- 0.7: Lock handle and background sync
- 0.8: Anonymous tips and UX

### Special thanks to
- [moneromoo](https://github.com/moneromooo-monero)
- [hyc](https://github.com/hyc)
- [jtgrassie](https://github.com/jtgrassie)

*For all your help answering my questions <3*

## Report a bug

#### Known issues

- If you're on the redesigned Reddit, copying a previous post's tip and pasting it as your own will actually paste `[/u/Monerotipsbot](https://www.reddit.com/user/monerotipsbot)`, rather than `/u/Monerotipsbot`, causing it not to be summoned

If you found a bug not on this list, either message me [here](https://www.reddit.com/message/compose/?to=OsrsNeedsF2P&subject=A%20%20bug!!%20/u/MoneroTipsBot&message=Please%20be%20as%20detailed%20as%20possible.%20What%20happened?%20What%20should%20have%20happened?%20Thank%20you!) or sent me an email at cryptonotev7@protonmail.com!

*****

## Terms of use

*****

1) Don't break real world laws

2) Back up your private seed

3) Don't store more than you're willing to lose

By using the tipping service you agree to not break sitewide rules or break real world laws. You are responsible for ensuring the safety and retrieval of your own funds. The service may always go down, so you are likewise responsible for backing up your private seed and I am not responsible for lost funds because of failure to do so. By having Monero on this service, you agree to not hunt me down for it. It's yours, you're responsible for it. The source code is published on Github [here](https://github.com/dginovker/MoneroTipper), so if you spot a potential security flaw please let me know ASAP either through a Reddit PM to /u/OsrsNeedsF2P, or an email to cryptonotev7@protonmail.com.

Stay safe and happy tipping!
