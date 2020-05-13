---
layout: post
title: 'PiNode-XMR'
repo_name: 'PiNode-XMR'
description: 'Monero node for single board computers with web interface and pre-configured tools.'
introduction: 'Monero Node for Single Board Computers'
date: 2020-05-13 00:00:00
maintainer: 'shermand100'
maintainer_uid: '20049380'
main-class: 'utility'
tags:
- shermand100
- Raspberry Pi
- Single-Board-Computer
image: 
color: '#B31917'
---

![PiNode-XMR logo](https://github.com/monero-ecosystem/PiNode-XMR/blob/master/Screenshots/PiNode-XMR%20logo.jpg)
# User Manual v3.20.04-Open-Build		
#### Self Install Open Source Build for Raspbian (Raspberry Pi) & Armbian Debian Buster (For all other devices)
or
#### Pre assembled disk images available for download (Raspberry Pi 3b+ & 4)

## Support at
* [Redit.com/r/PiNode](https://www.reddit.com/r/pinode/)
* Telegram group PiNode-XMR [t.me/PiNodeXMR](https://t.me/PiNodeXMR)

*Hosting large image files such as the pre-sync'd version does come with it's costs. If you like the project or found the images helpful any contribution would be gratefully received:*

43HoAhqx9q3MR1crAjpQtYVhvzQhZgqPwSWVQMmPvYmr18qVUEjCHcsEasuCxS486rWSSg1gbGqanet67NWRsh1bQL9KkB9

## Intro

Let me start by saying I'm glad the internet has bought you to here. It's taken several years to get to this point of the project, which in itself has been part of a multi year hobby creating nodes for cryptocurrencies and producing guides for beginners to follow along the way. The project is in a changing state at the moment with a shift from pre-built disk images, to you the user running a single command to initiate the install from this github repository. The reason for this change is to present the project as open source, increase transparency and trust. It also gives the added benefit of no longer being tied to the hardware of the device I was building the disk images on. This gives you the user much greater freedom to install your node on any Armbian device of your choice. Whilst this transition to open source finalises I will continue to provide the pre-made and pre-syncd disk images for the Raspberry Pi, but will phase this out over the year.
Also throughout the years I've had many requests from users if they could purchase pre-made nodes and although this is not something my lifestyle can accommodate, it does signal that users too have busy lifestyles, they want a node fast and I hope this project is a reasonable solution to that request.

To that end I hope you find this latest project invaluable to running your own Monero node, fast. The initial sync will take some time, and for that reason I also supply this node pre-sync'd as an image. Security for the device has been configured but every copy of this device currently has the same password as I set it. It is important you change it to something unique, this is detailed later on in this document.

Dan

*This Manual is still aimed at a low beginner level user including SD formatting and image writing. After these chapters and node usage you'll find detailed breakdowns of how this node works for those that are interested in contributing. Finally all suggested software used in the setup stages are downloadable for free*

## Contents:

* [Intro](https://github.com/monero-ecosystem/PiNode-XMR#intro)
   * [Features List](https://github.com/monero-ecosystem/PiNode-XMR#features)
   * [Hardware Requirements](https://github.com/monero-ecosystem/PiNode-XMR#hardware-requirements)
   * [Installing - Open Source (option 1)](https://github.com/monero-ecosystem/PiNode-XMR#installing)
      * [Raspberry Pi Self Install](https://github.com/monero-ecosystem/PiNode-XMR#raspberry-pi)
      * [Installing on all other devices - via Armbian Debian Buster OS](https://github.com/monero-ecosystem/PiNode-XMR#all-other-devices---armbian-debian-buster-os)
   * [Download - Pre-Configured Disk Image (option 2)](https://github.com/monero-ecosystem/PiNode-XMR#downloads)
   * [Setup](https://github.com/monero-ecosystem/PiNode-XMR#setup)
* [Web-UI: Getting started & General Usage](https://github.com/monero-ecosystem/PiNode-XMR#web-ui-starting-your-node-and-general-usage)
   * [Welcome Page](https://github.com/monero-ecosystem/PiNode-XMR#welcome-page--)
   * [Advanced Settings & Starting Monero](https://github.com/monero-ecosystem/PiNode-XMR#advanced-settings---starting-monero)
   * [Node Status](https://github.com/monero-ecosystem/PiNode-XMR#node-status--)
   * [Monero Blockchain Explorer](https://github.com/monero-ecosystem/PiNode-XMR#monero-blockchain-explorer)
   * [Transaction Status](https://github.com/monero-ecosystem/PiNode-XMR#transaction-status)
   * [Connection Status](https://github.com/monero-ecosystem/PiNode-XMR#connection-status)
   * [Log](https://github.com/monero-ecosystem/PiNode-XMR#log)
* [Web Terminal: Main System Menu](https://github.com/monero-ecosystem/PiNode-XMR#web-terminal--main-system-menu)
     * [System Settings](https://github.com/monero-ecosystem/PiNode-XMR#system-settings)
       * [Raspi-Config](https://github.com/monero-ecosystem/PiNode-XMR#raspi-config---hardware-management)
       * [Master Login Password set](https://github.com/monero-ecosystem/PiNode-XMR#master-login-password)
       * [Monero RPC password and user name set](https://github.com/monero-ecosystem/PiNode-XMR#monero-rpc-password-and-username)
       * [USB Storage setup](https://github.com/monero-ecosystem/PiNode-XMR#usb-storage-setup)
       * [SDCard Health Checker - via "Agnostics"](https://github.com/monero-ecosystem/PiNode-XMR#agnostics---sd-card-health-checker)
     * [Update Tools](https://github.com/monero-ecosystem/PiNode-XMR#update-tools)
       * [Update Monero](https://github.com/monero-ecosystem/PiNode-XMR#update-monero)
       * [Update PiNode-XMR](https://github.com/monero-ecosystem/PiNode-XMR#update-pinode-xmr)
       * [Update Blockchain Explorer](https://github.com/monero-ecosystem/PiNode-XMR#update-block-explorer)
       * [Update background system dependencies](https://github.com/monero-ecosystem/PiNode-XMR#update-background-system-dependencies)
     * [Node Tools](https://github.com/monero-ecosystem/PiNode-XMR#node-tools)
       * [Start/Stop Blockchain Explorer](https://github.com/monero-ecosystem/PiNode-XMR#startstop-blockchain-explorer)
       * [Prune Node](https://github.com/monero-ecosystem/PiNode-XMR#prune-node)
       * [Pop Blocks](https://github.com/monero-ecosystem/PiNode-XMR#pop-blocks)
     * [Extra Network Tools](https://github.com/monero-ecosystem/PiNode-XMR#extra-network-tools)
       * [Install tor](https://github.com/monero-ecosystem/PiNode-XMR#install-tor)
       * [View tor NYX - (network monitor)](https://github.com/monero-ecosystem/PiNode-XMR#tor-nyx)
       * [Install PiVPN](https://github.com/monero-ecosystem/PiNode-XMR#install-pivpn)
       * [Install No-IP (Dynamic DNS)](https://github.com/monero-ecosystem/PiNode-XMR#noipcom-dynamic-dns)
  
* [A note on tor](https://github.com/monero-ecosystem/PiNode-XMR#tor)
* [Connecting a Wallet -LAN](https://github.com/monero-ecosystem/PiNode-XMR#connecting-a-wallet---lan)
  * [Monero GUI](https://github.com/monero-ecosystem/PiNode-XMR#monero-gui)
  * [Monerujo app](https://github.com/monero-ecosystem/PiNode-XMR#monerujo-app)
* [Connecting a wallet - External Connections](https://github.com/monero-ecosystem/PiNode-XMR#connecting-a-wallet---external-connections)
  * [IP address considerations](https://github.com/monero-ecosystem/PiNode-XMR#ip-address-considerations)
  * [Port Forwarding](https://github.com/monero-ecosystem/PiNode-XMR#port-forwarding)
  
## Features:
* 4 Node modes (click to start)
  * Private Node
  * tor bridging Node - routes your transactions through the tor network
  * Public Node - Using new RPC payment feature* [Monero project commit message for more info](https://github.com/monero-project/monero/commit/2899379791b7542e4eb920b5d9d58cf232806937)
  * Private Node - with mining (For education/experiment only)
* Simple control with Web-UI
  * View Monero node and hardware status
  * Control bandwidth, connection limits and RPC port
  * Transaction pool and summary viewer
  * View connected peer info
  * Monerod log file view page
* Monero Block Explorer [Github - onion-monero-blockchain-explorer](https://github.com/moneroexamples/onion-monero-blockchain-explorer)
* Easy setup menu for config of passwords and Updates.
* **New** - Additional tools
  * raspi-config (Hardware and Wifi settings pre-built into PiNode-XMR menu
  * Agnostics - SD Card read/write health checker included
  * PiVPN - Tool for easy configuration of OpenVPN for Raspbian and Armbian
  * Pop blocks - Monero tool to help recover blockchain problems - UI
  * Systemd Monitor to track running node and explorer functions
  * tor installer - tor is no longer included and running as default due to censorship, political or legal restriction of users host country. Simple select to install and activate on user request.
  * All status boxes have improved scripts for clearer more constant feedback during high CPU loads.
  * Improved helper to setup an external USB storage device to hold the Monero blockchain. This new script allows a user to import a blockchain already held from a PC. Also on SD card failure this storage device can be identified by PiNode-XMR as configured for use, preserving the blockchain and so reducing re-startup time.
* All the other benefits of running a node on a Single Board computer (EG. RasPi, silent/fan-less, low power (approx 15w) for 24/7 node, low cost)
* Headless (No need for extra monitor,keyboard,etc) direct connect via Ethernet or WiFi**


*Public Node has settings configured but requires test and activation on implementation of  [monero-project pull #6260](https://github.com/monero-project/monero/pull/6260) For context of issue see [monero-project issue #3083](https://github.com/monero-project/monero/issues/3083)

**Connection via Ethernet required to configure WiFi

**Check out the repository to see the full README: https://github.com/monero-ecosystem/PiNode-XMR**
