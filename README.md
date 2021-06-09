# Solana-Foundation-Delegation-Program-Command-line-Utility
1) ```apt-get update```

2) ```sudo apt-get -y install libssl-dev libudev-dev pkg-config zlib1g-dev llvm clang make```

3) ```curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh```
выбираем 1 опцию

4) ```source $HOME/.cargo/env```

5) ```cargo install solana-foundation-delegation-program-cli```

6) ```solana-keygen new -o mainnet-validator-keypair.json```

7) закидываем 0,002 SOL на тестовый адрес

8) если ваш тестовый ключ имеею название validator-keypair.json

```solana-foundation-delegation-program apply --mainnet mainnet-validator-keypair.json --testnet validator-keypair.json --confirm```

9) Проверяем статус
```solana-foundation-delegation-program status mainnet-validator-keypair.json```
