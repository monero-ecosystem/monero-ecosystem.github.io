---
layout: post
title: "Vanity Monero"
repo_name: 'vanity-monero'
description: 'Generate vanity address for CryptoNote currency'
introduction: 'Generate vanity address for CryptoNote currency'
date: 2019-07-03 00:00:00
maintainer: 'Equim-chan'
maintainer_uid: '17795845'
main-class: 'utility'
tags:
- Equim-chan
- vanity
---

vanity-monero is a tiny CLI tool that generates vanity address for CryptoNote currencies. Currently only Monero main net and test net are supported.

== Features
* Prefix matching from 1st or 3rd index of address string.
* Regex matching at any position.
* Multi-language mnemonic seeds generation.
* Faster generation when there is only spend key that is needed in a specific pattern.
* Support https://en.bitcoin.it/wiki/Split-key_vanity_address[split-key vanity address] generation, which makes scaled vanity mining potential.
