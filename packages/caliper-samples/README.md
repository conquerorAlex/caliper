# Caliper Application Example(s)

Basic CLI driven sample(s)

## Working Benchmarks (local)
- Fabric
node run-benchmark.js -c ../benchmark/simple/config.yaml -n ../network/fabric-v1.4/2org1peercouchdb/fabric-node.json

- Fabric CCP
node run-benchmark.js -c ../benchmark/simple/config.yaml -n ../network/fabric-v1.2/2org1peercouchdb/fabric-ccp-node.json

- Composer
node run-benchmark.js -c ../benchmark/composer/config.yaml -n ../network/fabric-v1.3/2org1peercouchdb/composer.json

- Sawtooth
node run-benchmark.js -c ../benchmark/simple/config-sawtooth.yaml -n ../network/sawtooth/simplenetwork/sawtooth.json 

## Benchmarks Under Construction
-Burrow
node run-benchmark.js -c ../benchmark/simple/config.yaml -n ../network/burrow/simple/burrow.json

- Iroha
node run-benchmark.js -c ../benchmark/simple/config-iroha.yaml -n ../network/iroha/simplenetwork/iroha.json 

## Starting and using a Zookeeper client

node start-zoo-client.js -t fabric -n ../network/fabric-v1.4/2org1peercouchdb/fabric-node.json -a 127.0.0.1:2181
node run-benchmark.js -c ../benchmark/simple/config-zookeeper.yaml -t fabric -n ../network/fabric-v1.4/2org1peercouchdb/fabric-node.json
