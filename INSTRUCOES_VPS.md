# Instruções para VPS

Para configurar o Bitcoin Wallet na VPS (Debian 11):

1. Clone o repositório
2. Extraia o arquivo compactado: tar -xzf codigo_bitcoin.tar.gz
3. Compile o executável Go: cd BitcoinWallet-2 && go build -o bitcoinwallet cmd/main.go
4. Configure permissões: chmod +x *.sh
5. Inicie o servidor: ./start.sh

O servidor estará disponível na porta 8080.

Para ajustar o desempenho, edite o arquivo start.sh e aumente o valor de NUM_WORKERS de acordo com o número de cores da CPU.
