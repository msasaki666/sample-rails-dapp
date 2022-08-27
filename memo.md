# docker composeでやったときのメモ

- gethのブロックチェーンネットワークにアクセスする際、hostをblockchainにする必要

```ruby
 client = Eth::Client.create 'http://blockchain:8545'
```

- webコンテナ内で、以下を実行しないと表示でエラー(docker-compose.ymlでは、foremanで実行されるはずの以下のコマンドが実行されていないため)

```shell
bin/rails tailwindcss:watch
```

- コンテナ起動のたびにコントラクトデプロイrake taskを実行する必要がある
