# Build process

## Milestone before continue

At this point you should already have installed:

1. Golang
2. Node.js
3. PNPM
4. PM2

{% hint style="success" %}
**If so, continue, if not, return to the previous page** :wink:
{% endhint %}

## Next step - clone the core repository&#x20;

Use it via GitHub

```sh
git clone https://github.com/KlyntarNetwork/KlyntarCore.git

cd KlyntarCore
```

Now depending on your OS run the following commands:

## Install dependencies

```sh
pnpm install
```

## Link core to make it available from any location

```sh
npm link
```

## Build Golang addons

Run a simple script

{% tabs %}
{% tab title="Unix" %}
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

## Build KLY-EVM

{% tabs %}
{% tab title="Unix" %}
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

## Return to main directory

```sh
cd ../../

// Linux/Mac only
chmod 700 klyntar_core.js
```

{% hint style="success" %}
**At this stage, the build process ends and the preparation of files for work begins**
{% endhint %}

## Prepare configuration and genesis files

Depending on the network you want to connect to, you will need an appropriate genesis file, as well as a set of configurations for your node.

To find the files that suit you, follow the instructions in the section [**Networks**](../networks/)

1. [setup-testnet-node.md](../networks/testnet/public-testnets/setup-testnet-node.md "mention")
2. [setup-mainnet-node.md](../networks/mainnet/setup-mainnet-node.md "mention")
