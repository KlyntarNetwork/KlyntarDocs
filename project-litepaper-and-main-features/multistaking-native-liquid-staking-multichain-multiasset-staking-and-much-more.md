---
icon: square-dollar
---

# Multistaking - native liquid staking, multichain multiasset staking and much more!

## Intro

In an effort to increase the user experience and add more network features we are introducing a **multistaking mechanism**.

{% hint style="success" %}
**Multistaking** is a general collective name for advanced staking mechanisms that are aimed at maximum security, decentralization of the network. It also improves the user experience for users, validators and stakers.
{% endhint %}

Multistaking includes:

1. [#native-liquid-staking](multistaking-native-liquid-staking-multichain-multiasset-staking-and-much-more.md#native-liquid-staking "mention")
2. [#multichain-multiasset-staking-and-social-value-points](multistaking-native-liquid-staking-multichain-multiasset-staking-and-much-more.md#multichain-multiasset-staking-and-social-value-points "mention")
3. Other future options and improvements

## Native liquid staking

Since our network relies on the optimistic assumption that most validators will be honest, we decided to follow the Avalanche path - **we have no slashing**

{% embed url="https://docs.cdp.coinbase.com/delegation/docs/avalanche-faq" %}

The network remains decentralized and fault-tolerant, and in addition - validators and stakers are protected. This creates excellent opportunities for us to implement **native liquid staking**:

{% hint style="info" %}
In simple terms - you will be able to transfer coins to other addresses even if they are sent to staking. Since there is no slashing - the rate of the native coin will always be equal to the rate of the liquid staking token
{% endhint %}

## Multichain multiasset staking & social value points

In an effort to increase decentralization rates and protect the network, as well as other chains in the ecosystem, we are introducing a new mechanism - now you can protect the network by delegating your coins, tokens from other projects. Also, you can use **social value points** - details will be later :wink:

This increases the number of potential validators in the Klyntar network, which makes the network stronger, more resilient and reliable!

### How it works ?

On the page with information about the validator, you will notice the **multistaking points** section. These points are credited to the validator when you stake coins/tokens on other blockchains in smart contracts or use your social value points to delegate to validator.

For this, validators will credit you with part of their rewards depending on the % that you staked.

<figure><img src="../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

### What coins/tokens/else can be used for multistaking

See here:

{% embed url="https://docs.klyntar.org/build-core-and-join-network/staking/multistaking/supported-networks-and-tokens" %}

See also

{% embed url="https://docs.klyntar.org/build-core-and-join-network/staking/multistaking/social-media-multistaking" %}

### Unfrozen liquidity

When you stake your coins, ERC-20 tokens, LSTs, LRTs and others - you receive a token in return equal to 1:1 - to maintain liquidity.

For example, if you stake 1 TRON($TRX), you will receive 1 KLYTRON in return. This way, you can continue to use your coins.

### No slashing

Our smart contracts **do not provide for the possibility of slashing**. This means that only you have access to your funds. If the validator that you staked on violates the rules of the Klyntar network, it will simply be excluded from the set, but your tokens on other blockchains **cannot be slashed**.

Please, DYOR the smart contracts yourself:

{% embed url="https://github.com/KlyntarNetwork/MultistakingContracts" %}

## How to start ?

Find more details in appropriate section in our docs

{% embed url="https://docs.klyntar.org/build-core-and-join-network/staking/multistaking" %}

Also, here are three examples of multistaking - with native coins of other networks, ERC-20 tokens in these networks and **social points**:

{% embed url="https://docs.klyntar.org/build-core-and-join-network/staking/multistaking/work-with-native-coins" %}

{% embed url="https://docs.klyntar.org/build-core-and-join-network/staking/multistaking/work-with-erc-20-tokens" %}

{% embed url="https://docs.klyntar.org/build-core-and-join-network/staking/multistaking/social-media-multistaking" %}
