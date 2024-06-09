# Bitcoin Wallet Generator - Formação Blockchain Specialist Bootcamp

Este projeto foi desenvolvido como parte do bootcamp Formação Blockchain Specialist, com o objetivo de construir um gerador de carteiras Bitcoin, importar para um software gerenciador de carteiras (Electrum) e realizar transações de envio e recebimento de Bitcoin utilizando a rede de teste (testnet).

## Descrição

O código fornecido é um script em JavaScript que utiliza as bibliotecas `bip32`, `bip39`, e `bitcoinjs-lib` para gerar uma carteira Bitcoin. Ele cria um mnemonic (conjunto de palavras de senha), a partir do qual uma seed (semente) é gerada. Essa seed é então usada para criar a raiz da carteira HD (Hierarchical Deterministic), da qual pares de chaves privadas e públicas são derivados. O script configura a rede para testnet, permitindo o desenvolvimento e teste sem o uso de Bitcoin real.

### Funcionalidades

- Geração de mnemonic para seed.
- Criação da raiz da carteira HD.
- Derivação de contas e endereços.
- Geração de endereços Bitcoin para receber fundos na rede testnet.
- Exibição do endereço Bitcoin, chave privada e mnemonic.

### Instruções Iniciais

Para iniciar o desenvolvimento, foi necessário:

1. Instalar o Node.js no Linux.
2. Iniciar o projeto com `npm init`.
3. Instalar as dependências com o comando `npm install bip39 bip32@2.0.6 bitcoinjs-lib --save`.

### Importação para Electrum

Para importar a carteira gerada para o Electrum:

- Abrir o Electrum normalmente e seguir os procedimentos padrões para importação.
- Para usar como testnet, é necessário iniciar o Electrum com o argumento `--testnet`. No Linux, isso pode ser feito através do programa Gear para gerenciar imagens AppImage, instalando-o como flatpak e configurando o argumento `--testnet` em Command Line Argumments (Ex.: `%u --testnet`) nas configurações do programa.

### Recursos Adicionais

- **Verificação de Transações no Testnet:** [Blockstream Info Testnet](https://blockstream.info/testnet/)
- **Obtenção de Bitcoin de Teste (Faucet):** [Coin Faucet Testnet](https://coinfaucet.eu/en/btc-testnet/)

Este projeto é uma introdução prática ao desenvolvimento com Bitcoin, permitindo explorar a criação de carteiras, a gestão de chaves e a realização de transações de forma segura na rede de teste.
