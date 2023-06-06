`ord-api`
=====

`ord-api` ord-api is forked from ordinals/ord.
Added some APIs for obtaining inscription information.
See [ordinals/ord](https://github.com/ordinals/ord) for guides.


APIs
------------

1. http://host:port/api/inscriptions?page=1&size=100
2. http://host:port/api/inscription/:inscription_id

Run
--------

use bitcoind cookie-file:

```
./ord_api  --bitcoin-data-dir=/path/to/bitcoin/data/dir  --cookie-file=/path/to/cookie/file --rpc-url=http://bitcoind-rpc-url --data-dir=/path/to/save/index/dir  server --http-port 7070
```
use bitcoind username and password:

```
./ord_api  --bitcoin-data-dir=/path/to/bitcoin/data/dir   --bitcoin-rpc-pass="test" --bitcoin-rpc-user="test" --rpc-url=http://bitcoind-rpc-url --data-dir=/path/to/save/index/dir  server --http-port 7070
```

For test net:

```
./ord_api  --bitcoin-data-dir=/path/to/bitcoin/data/dir  --cookie-file=/path/to/cookie/file --rpc-url=http://bitcoind-rpc-url --data-dir=/path/to/save/index/dir -t server --http-port 7070
```
