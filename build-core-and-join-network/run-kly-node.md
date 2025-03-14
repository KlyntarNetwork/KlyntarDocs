# ☁️ Build the core

## Node.js installation

<figure><img src="../.gitbook/assets/image (6) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Since the core is written on Node.js you should to install it. If you already have installed, we recommend checking the version. The recommended version is **v21.4.0**

{% tabs %}
{% tab title="Linux" %}
```sh
johndoe@klyntar:~$ node -v
v21.4.0
```
{% endtab %}

{% tab title="Windows" %}
```sh
C:\Users\JohnDoe>node -v
v21.4.0
```
{% endtab %}
{% endtabs %}

Use official guides to install Node.js for your platform (Windows/Linux/Mac)

{% embed url="https://nodejs.org/en/download/package-manager" %}

## Go installation

<figure><img src="../.gitbook/assets/image (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

Some parts of KLY is written on Go(for example, PQC schemes), so you need to install it too. Use this guide to install Golang for your platform & architecture

{% embed url="https://go.dev/doc/install" %}

Or, check if you already have Go

```sh
go version
```

## PNPM install

<figure><img src="../.gitbook/assets/image (2) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

As a package manager for Node.js we use pnpm. To install it globally, run:

```sh
npm install -g pnpm
```

## Install PM2 for production process management

<figure><img src="../.gitbook/assets/image (112).png" alt=""><figcaption></figcaption></figure>

PM2 is a production process manager for Node.js applications with a built-in load balancer. It allows you to keep applications alive forever, to reload them without downtime and to facilitate common system admin tasks.

**You can install it globally using the command:**

```sh
npm install pm2 -g
```

{% embed url="https://www.npmjs.com/package/pm2" %}

PM2 allows you to manage and monitor a node/validator in production mode. So, you can simply start the node/validator via PM2 to:

1. Run the node as a background service - so you can close the console, close the SSH connection to server and node will work on background
2. Have access to logs stream to monitor node status

Here are some useful commands

```
pm2 start <service_name> - to start the core as background service
pm2 stop <service_name> - to stop the core
pm2 monit <service_name> - start console dashboard with logs, memory usage, etc.
pm2 logs <service_name> - start logs stream
pm2 logs <service_name> --lines <x> --nostream - read last X lines of logs from error stream and normal logs stream
```

## After all

Now, clone the core repository

```sh
git clone https://github.com/KlyntarNetwork/KlyntarCore.git

cd KlyntarCore
```

Now depending on your OS run the following commands:

### Install dependencies

```sh
pnpm install
```

### Link core to make it available from any location

```sh
npm link
```

### Build Golang addons

Run a simple script

{% tabs %}
{% tab title="Linux" %}
```bash
chmod 700 build_must_have_addons.sh

./build_must_have_addons.sh
```
{% endtab %}

{% tab title="Windows" %}
```sh
build_must_have_addons.bat
```
{% endtab %}
{% endtabs %}

### Build KLY-EVM

{% tabs %}
{% tab title="Linux" %}
```sh
cd KLY_VirtualMachines/kly_evm

pnpm install

chmod 700 build_kly_evm.sh

./build_kly_evm.sh
```
{% endtab %}

{% tab title="Windows" %}
```sh
cd KLY_VirtualMachines\kly_evm

pnpm install

build_kly_evm.bat
```
{% endtab %}
{% endtabs %}

### Return to main directory

```sh
cd ../../

//Linux only
chmod 700 klyntar_core.js
```

{% hint style="success" %}
**At this stage, the build process ends and the preparation of files for work begins**
{% endhint %}

## Prepare configuration and genesis files

Depending on the network you want to connect to, you will need an appropriate genesis file, as well as a set of configurations for your node.

To find the files that suit you, follow the instructions in the section [**Networks**](networks/)

1. [setup-testnet-node.md](networks/testnet/public-testnets/setup-testnet-node.md "mention")
2. [setup-mainnet-node.md](networks/mainnet/setup-mainnet-node.md "mention")
