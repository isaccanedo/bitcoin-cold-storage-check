# Verificação de armazenamento de Bitcoin
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
Descubra o valor presente em dólares dos endereços em addresses.json:

    node app

Notas
-----
Este pacote obtém primeiro o preço atual em USD / BTC da Bitfinex. O suporte para outras trocas ainda não está disponível.

Esta ferramenta também depende de [Insight from BitPay](https://github.com/bitpay/insight). 
Você pode executar sua própria cópia do Insight localmente para não "denunciar" ao mundo sobre o seu
endereços de armazenamento frio.
