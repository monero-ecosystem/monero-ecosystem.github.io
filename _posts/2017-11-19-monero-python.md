---
layout: post
title: 'Monero python'
repo_name: 'monero-python'
description: 'A comprehensive Python module for handling Monero cryptocurrency'
introduction: 'A comprehensive Python module for handling Monero cryptocurrency'
date: 2019-04-05 00:00:00
maintainer: 'emesik'
maintainer_uid: '407107'
main-class: 'utility'
tags:
- emesik
- python
- RPC
image: 
---

Python Monero module
====================

A comprehensive Python module for handling Monero cryptocurrency.

* release 0.5.2
* open source: https://github.com/monero-ecosystem/monero-python
* works with Monero 0.12.x and [the latest source]\(at least we try to keep up\)
* Python 2.x and 3.x compatible
* comes with [documentation]
* generously funded by [Monero FFS] donors

[the latest source]: https://github.com/monero-project/monero
[documentation]: http://monero-python.readthedocs.io/en/latest/
[Monero FFS]: https://forum.getmonero.org/9/work-in-progress

Copyrights
----------

Released under the BSD 3-Clause License. See [LICENSE.txt].

Copyright (c) 2017-2018 Michał Sałaban <michal@salaban.info> and Contributors: [lalanza808], [cryptochangements34], [atward], [rooterkyberian], [brucexiu],
[lialsoftlab], [moneroexamples].

Copyright (c) 2016 The MoneroPy Developers (``monero/base58.py`` and ``monero/ed25519.py`` taken from [MoneroPy])

Copyright (c) 2011 thomasv@gitorious (``monero/seed.py`` based on [Electrum])

[LICENSE.txt]: LICENSE.txt
[MoneroPy]: https://github.com/bigreddmachine/MoneroPy
[Electrum]: https://github.com/spesmilo/electrum
[lalanza808]: https://github.com/lalanza808
[cryptochangements34]: https://github.com/cryptochangements34
[atward]: https://github.com/atward
[rooterkyberian]: https://github.com/rooterkyberian
[brucexiu]: https://github.com/brucexiu
[lialsoftlab]: https://github.com/lialsoftlab
[moneroexamples]: https://github.com/moneroexamples

Want to help?
-------------

If you find this project useful, please consider a donation to the following address:
``481SgRxo8hwBCY4z6r88JrN5X8JFCJYuJUDuJXGybTwaVKyoJPKoGj3hQRAEGgQTdmV1xH1URdnHkJv6He5WkEbq6iKhr94``


Development
-----------

1. Clone the repo
2. Create virtualenv & activate it
    ```bash
    python3 -m venv .venv
    source .venv/bin/activate
    ```
3. Install dependencies
    ```bash
    pip install -r requirements.txt -r test_requirements.txt
    ```
4. Do your thing
5. Run tests
    ```bash
    pytest
    ```
