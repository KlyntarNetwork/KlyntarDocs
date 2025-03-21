# Block API

## Get block by ID

Block ID consists of 3 parts:

1. Epoch index when block was created
2. Pubkey of pool who created this block
3. Index of block in own sequence. It's individual for each new creator

For example, to get the block 15th by pool `9GQ46rqY238rk2neSwgidap9ww5zbAN4dyqyC7j5ZnBK` created in epoch 1 you need to call

```javascript
let blockID = "1:9GQ46rqY238rk2neSwgidap9ww5zbAN4dyqyC7j5ZnBK:15"

await web1337.getBlockByBlockID(blockID)
```

## Get block by SID

SID stands for **shard index**. Each shard in Klyntar exists as a separate chain so it has linear sequence of blocks.

Just like in non-sharded blockchains like Bitcoin, Ethereum, Solana etc. you just need to find for wished height

For example, to get the most first block on just find:

```javascript
let absoluteHeight = 0;

await web1337.getBlockBySID(absoluteHeight);
```

## Get sequence of N blocks on shard

The same as previous API, but returns the multiple N blocks started from some index.

For example, to get the list of 20 blocks from block 34 to block 34-20=**14 ,** just try:

```javascript
let startIndex = 34;

let limit = 20;

await web1337.getLatestNBlocks(shard,startIndex,limit);
```

{% hint style="info" %}
This route is useful for explorer pages, pagination, etc.
{% endhint %}

## Get total number of blocks, transactions and successful transactions

This API returns general stats - from genesis to the current time. Number of blocks and transactions during the whole time - on each shard

```javascript
await web1337.getTotalBlocksAndTxsStats()
```
