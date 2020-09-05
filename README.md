# bitcoin-cold-storage-check
Exibe a quantidade de bitcoin armazenado em endereços de armazenamento refrigerado. Usa api.bitfinex.com e insight.bitpay.com para dados.

Setup
-----
Comece instalando as dependências:

    npm install

Copie o addresses.json.example para addresses.json:

    cp addresses.json.example addresses.json

Edite e adicione os endereços que deseja rastrear.

Run
---
Find out the present value in USD of the addresses in addresses.json:

    node app

Notes
-----
This package first gets the current USD / BTC price from Bitfinex. Support 
for other exchanges isn't yet available.

This tool also relies on [Insight from BitPay](https://github.com/bitpay/insight). You can run your own copy of 
Insight locally so you aren't "tipping your hand" to the world about your
cold storage addresses.
