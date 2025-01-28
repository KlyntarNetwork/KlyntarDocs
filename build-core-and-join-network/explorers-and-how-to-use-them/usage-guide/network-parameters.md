# Network Parameters

This is the simplest section that will tell you about the current network parameters

<figure><img src="../../../.gitbook/assets/image (108).png" alt=""><figcaption></figcaption></figure>

These parameters are specified in the genesis and they regulate the operation of the network. Here you will find information about the network ID, the bet size for the validator, the duration of the epoch, and so on.

So, for example, if you look at genesis, you will see similar indicators - they will be displayed in the interface.

```json
"NETWORK_PARAMETERS":{

        "VALIDATOR_STAKE":50000,
        "MINIMAL_STAKE_PER_ENTITY":20,
        "QUORUM_SIZE":127,
        "EPOCH_TIME":90000,
        "LEADERSHIP_TIMEFRAME":60000,
        "BLOCK_TIME":1000,
        "MAX_BLOCK_SIZE_IN_BYTES":12288000,
        "TXS_LIMIT_PER_BLOCK":30000
    
}
```
