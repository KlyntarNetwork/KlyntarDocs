---
icon: magnifying-glass-waveform
---

# Netrunner and PM2

## Using PM2 for production management

<figure><img src="../../../../.gitbook/assets/image (129).png" alt=""><figcaption></figcaption></figure>

PM2 allows you to run services in the background, monitor server resource usage, write logs, and more.

{% hint style="info" %}
**PM2 is the recommended way to run and maintain a node (regular and validator) for Klyntar**
{% endhint %}

To run & work with a testnet you can use these simple commands:

## 1. Start a testnet in a single command:

```
pm2 start runner2.js
```

## 2. Check the active background services

You will see the following

<figure><img src="../../../../.gitbook/assets/image (130).png" alt=""><figcaption></figcaption></figure>

## 3. Enter monitoring dashboard

```
pm2 monit runner2
```

<figure><img src="../../../../.gitbook/assets/image (131).png" alt=""><figcaption></figcaption></figure>

## 4. Read the logs stream

```
pm2 logs runner2
```

<figure><img src="../../../../.gitbook/assets/image (132).png" alt=""><figcaption></figcaption></figure>

## 5. Read last N lines of logs from stdout / stderr streams (`nostream` mode)

```
pm2 logs --lines <N> --nostream runner2
```

{% hint style="info" %}
#### Reading logs available even if the service was stopped - so it's useful to understand reasons of downtimes and so on
{% endhint %}

## 6. Stop a testnet

```
pm2 stop runner2
```

{% hint style="info" %}
#### When you stop the testnet and then run it again - the progress will be dropped and testnet will start from height 0 and epoch 0
{% endhint %}
