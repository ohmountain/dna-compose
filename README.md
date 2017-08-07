# DNA docker-compose.yml
> DNA Docker 部署的一个简单例子

## 目录结构

```
├── chain
│   ├── Chain_01
│   ├── Chain_02
│   ├── Chain_03
│   └── Chain_04
├── config
│   ├── config_01.json
│   ├── config_02.json
│   ├── config_03.json
│   ├── config_04.json
├── log
│   ├── Log_01
│   ├── Log_02
│   ├── Log_03
│   └── Log_04
└── wallets

```

## Usage
```shell
git clone https://github.com/ohmountain/dna-compose
cd dna-compose
mkdir -p log/Log_01 log/Log_02 log/Log_03 log/Log_04
mkdir -p chain/Chain_01 chain/Chain_02 chain/Chain_03 chain/Chain_04
mkdir wallets

compose-up
```
