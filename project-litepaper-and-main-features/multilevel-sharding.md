# Multilevel sharding

<figure><img src="../.gitbook/assets/image (102).png" alt=""><figcaption></figcaption></figure>

## Intro

As we think about the future, we are trying to solve the problem of network scaling right away. Dividing the network into several smaller networks (**shards**) has become a standard in the industry.

We decided to go further and use a multilevel sharding system for greater efficiency. It is like classic sharding, but it has its advantages.

## Level 1 - appchains

At the first level, the networks will be divided according to their purpose. These will be independent projects that will join our ecosystem for common shared security, as well as various bonuses such as gasless cross-chain transfers and much more.

{% hint style="success" %}
The first project and blockchain in the ecosystem will obviously be our native blockchain - **Klyntar**
{% endhint %}

## Level 2 - single chain default sharding

This level of sharding is the most familiar to you - you may have seen it in other projects where there is also sharding.

At this level, we will divide the **Klyntar** blockchain into several independent subnetworks that:

1. Will use the same validator space - if there are N validators in the network in total, then there will be N validators on each shard (the same level of security)
2. Will work independently of each other and generate blocks in parallel - this increases the network throughput

We will use user migration mechanisms and smart contracts on new shards to load them evenly.

Such mechanisms include:

1. Bonuses for users for account migration - several gasless transactions, various boosts, etc.
2. [**Storage-by-subscription**](../web1337/advance-web1337-usage/abstraction/storage-abstraction/pay-for-storage-rent.md) mechanism for smart contracts - allow a smart contract not to pay for storage for some time on a new shard
3. A **coercion mechanism** that will limit the ability to use contracts or user accounts until they move to a new shard

## Level 3 - additional levels of parallelization

At the third level, we are also trying to improve the scalability of the network by parallelizing the execution environment. Find out more here:

{% content-ref url="../web1337/advance-web1337-usage/parallel-execution.md" %}
[parallel-execution.md](../web1337/advance-web1337-usage/parallel-execution.md)
{% endcontent-ref %}

In the future, we also plan to add the ability to separate the block verification process from the approval process, which will make the network more modular and, for example, run two modules on different machines
