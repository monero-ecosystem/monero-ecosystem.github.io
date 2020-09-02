---
layout: post
title: 'Monero C++ Library'
repo_name: 'monero-cpp'
description: 'A C++ library for using Monero '
introduction: 'A C++ library for creating Monero applications using native bindings'
date: 2020-09-01 00:00:00
maintainer: 'woodser'
maintainer_uid: '13068859'
main-class: 'utility'
tags:
- woodser
- C++
- library
image: 
color: '#B31917'
---
A C++ library for creating Monero applications using native bindings to Monero.

- Supports fully client-side wallets by wrapping wallet2.h.
- Supports multisig, view-only, and offline wallets.
- Uses a clearly defined data model and API specification intended to be intuitive and robust.
- Query wallet transactions, transfers, and outputs by their properties.
- Receive notifications when wallets sync, send, or receive.
- Tested by over 100 tests in monero-java and monero-javascript using JNI and WebAssembly bindings.