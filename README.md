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

1. 环境
```shell
git clone https://github.com/ohmountain/dna-compose
cd dna-compose
mkdir -p log/Log_01 log/Log_02 log/Log_03 log/Log_04
mkdir -p chain/Chain_01 chain/Chain_02 chain/Chain_03 chain/Chain_04
mkdir wallets
```

2. 生成wallet
```shell
docker-compose up -d

# 分别进入四个容器
cd /var/DNASamle/
./nodectl wallet -c -p=`${密码}` # 记录公钥并填入config.json中

# 完成后退出容器
docker-compose down
```
3. 运行
```shell
# 把上一步骤的密码替换掉docker-compose.yml中./DNA -p=passwordtest 的passwordtest


docker-compose up -d
```
