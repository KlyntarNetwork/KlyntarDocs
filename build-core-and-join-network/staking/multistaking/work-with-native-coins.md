---
icon: ethereum
---

# Work with native coins

## Intro

By placing your native network coins on a multistaking contract, you receive similar liquidity tokens in a 1:1 ratio.

This way, you can earn rewards on Klyntar (helping to decentralize the network) and at the same time continue to use the tokens in DeFi applications, lending protocols, etc.

In this tutorial we will show how to multistake the native coins on EVM chains - ETH, AVAX, BNB, TRON etc.

You can repeat the multistaking process through the interface on our website:

{% embed url="https://klyntar.org/multistaking" %}

## 1. Stake native chain coins to get liquidity tokens back and earn staking points

Visit the page

<figure><img src="../../../.gitbook/assets/image (120).png" alt=""><figcaption></figcaption></figure>

You will see the following interface

<figure><img src="../../../.gitbook/assets/image (121).png" alt=""><figcaption></figcaption></figure>

Now select the chain and wallet to connect

{% hint style="info" %}
In this tutorial we'll work with Sepolia network (Ethereum testnet)
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (122).png" alt=""><figcaption></figcaption></figure>

Right after connection you will see how much you already multistaked on appropriate contract in dollar equivalent

<figure><img src="../../../.gitbook/assets/image (123).png" alt=""><figcaption></figcaption></figure>

Choose the appropraite operation **Deposit** and token to stake - in this case native coin of network

<figure><img src="../../../.gitbook/assets/image (124).png" alt=""><figcaption></figcaption></figure>

The next steps:

1. Input amount - let's say you want to stake 0.01 Sepolia ETH
2. Choose the pool from list

<figure><img src="../../../.gitbook/assets/image (125).png" alt=""><figcaption></figcaption></figure>

Finally - just press **Deposit** and confirm the transaction from your wallet extension

### What is under the hood :thinking:

Let's check the explorer to see what transactions are actually called and what happens in detail. As you can see, we transferred 0.01 SepoliaETH and received 0.01 KETH(KlyntarETH) back.

<figure><img src="../../../.gitbook/assets/image (84).png" alt=""><figcaption></figcaption></figure>

### So, what you have

At this stage you have:

1. 0.01 KETH already on your balance - it's ERC-20 token which is 1:1 to native network coin. This avoids freezing liquidity. You can continue to use your KETH in DeFi applications or simply continue to HODL
2. At the same time, the pool you staked on will share some of its rewards with you. With your staking points, you increase the pool's chance of being elected to a quorum and/or generating blocks.

### Wait 3 epoches to make your stake active

Your stake will not become active immediately - the activation time currently takes 3 epochs - which is equivalent to 3 days.

### Check the stakers list

After a while, you can go to the page of the pool you staked on and find yourself in the list of stakers

<figure><img src="../../../.gitbook/assets/image (85).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (87).png" alt=""><figcaption></figcaption></figure>

## 2. Unstaking these liquidity tokens to get back your real ETHes, BSCs, AVAXes, etc.

So you have 0.01 KETH and you want to get your original SepoliaETH back.

Choose **Unstake** and input all the required data

<figure><img src="../../../.gitbook/assets/image (127).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
The field with amount will show you have much you can unstake
{% endhint %}

### Unstaking details

During the unstaking process, you burn the wrapped KETH token and release your real SepoliaETH tokens

<figure><img src="../../../.gitbook/assets/image (91).png" alt=""><figcaption></figcaption></figure>

### Wait for a while to release your stake

The unstaking time also takes **3 epochs**, so initially your stake gets into **withdrawal requests**

<figure><img src="../../../.gitbook/assets/image (92).png" alt=""><figcaption></figcaption></figure>

## 3. The last step - withdraw your stake

Choose **Withdraw** section and press a button to initiate a transaction

<figure><img src="../../../.gitbook/assets/image (128).png" alt=""><figcaption></figcaption></figure>

{% hint style="success" %}
After that you will finally get your original coins back
{% endhint %}

## FAQ

<details>

<summary>How to unstake from multiple pools immediately</summary>

TODO

</details>

