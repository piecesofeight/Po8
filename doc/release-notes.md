0.1.0 changes
=============

- Coin Control - experts only GUI selection of inputs before you send a transaction

- Disable Wallet - reduces memory requirements, helpful for miner or relay nodes

- 20x reduction in default mintxfee.

- Up to 50% faster PoW validation, faster sync and reindexing.

- Internal miner added back to PiecesofEight.  setgenerate now works, although it is generally a bad idea as it is significantly slower than external CPU miners.

- New RPC commands: getbestblockhash and verifychain

- Improve fairness of the high priority transaction space per block

- OSX block chain database corruption fixes
  - Update leveldb to 1.13
  - Use fcntl with `F_FULLSYNC` instead of fsync on OSX
  - Use native Darwin memory barriers
  - Replace use of mmap in leveldb for improved reliability (only on OSX)

- Fix nodes forwarding transactions with empty vins and getting banned

- Network code performance and robustness improvements

- Additional debug.log logging for diagnosis of network problems, log timestamps by default

- Fix rare GUI crash on send


