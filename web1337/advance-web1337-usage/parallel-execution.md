---
icon: grip-lines
description: Learn how to speed up your transaction in EVM / WASM
---

# Parallel execution

## Intro

Klyntar was created to implement best practices. That is why parallel transaction execution was implemented.

We have 4 types of transactions available below. Currently, parallel transaction execution is supported for:

<table><thead><tr><th width="274">Transaction type</th><th width="269">Description</th><th data-type="checkbox">Implementation status</th></tr></thead><tbody><tr><td><strong>TX</strong></td><td>Default address to address coins transfer</td><td>true</td></tr><tr><td><strong>WVM_DEPLOY</strong></td><td>Contract deployment to WASM vm</td><td>true</td></tr><tr><td><strong>WVM_CALL</strong></td><td>Call smart-contract in WASM vm</td><td>true</td></tr><tr><td><strong>EVM_CALL</strong></td><td>Interaction with EVM</td><td>true</td></tr></tbody></table>

In the interface of explorer you can see the **execution type** of transaction. This is example of parallel transaction:

<div data-full-width="true"><figure><img src="../../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure></div>

And this transaction is not parallel - it was executed in a sync way

<div data-full-width="true"><figure><img src="../../.gitbook/assets/image (37).png" alt=""><figcaption></figcaption></figure></div>

## Parallel execution for native transactions and WASM vm

See  [#transfer-coins-from-native-kly-environment-to-evm](../transactions-and-smart-contracts/transfer-coins-between-evm-and-native-environment.md#transfer-coins-from-native-kly-environment-to-evm "mention")

## Parallel execution for EVM

See [#transfer-coins-from-evm-to-native-kly-environment](../transactions-and-smart-contracts/transfer-coins-between-evm-and-native-environment.md#transfer-coins-from-evm-to-native-kly-environment "mention")
