# Installation Options

At its core Proton runs on top of EOS which means it's fully compatible with the existing EOS toolset (nodeos, cleos, ...).

You can either use EOS's binaries and use our custom `genesis.json` file or you can use our precompiled EOS binaries.

## Precompiled binaries

We've released prebuilt binaries for a couple of widely used platforms:

  - Ubuntu 16.04
  - Ubuntu 18.04
  - RPM-based (CentOS, Amazon Linux, etc.)

Please visit [this page](prebuilt-binaries.md) for more information on how to install the Proton binaries for these platforms.

?> **Is your platform not mentioned above?** Then your best option is to compile these from the Proton source code. Please visit [this page](build-from-source.md) for more information on how to compile the Proton binaries yourself.

## Use official EOS binaries

Since Proton is fully compatible with EOS's binaries you can also EOS's official binaries and configure those to use the Proton network by feeding it our `genesis.json` file. However, since changes to the Proton codebase are likely to occur we still recommend you install our binaries or compile them from the Proton source-code.

```javascript
{
  "initial_timestamp": "2020-04-22T17:00:00",
  "initial_key": "EOS5XPRJt1zUiLH98rtDLj9TnPi52DLQ7gTZbkRvBGJXLv6ak6Cdq",
  "initial_configuration": {
    "max_block_net_usage": 1048576,
    "target_block_net_usage_pct": 1000,
    "max_transaction_net_usage": 524288,
    "base_per_transaction_net_usage": 12,
    "net_usage_leeway": 500,
    "context_free_discount_net_usage_num": 20,
    "context_free_discount_net_usage_den": 100,
    "max_block_cpu_usage": 200000,
    "target_block_cpu_usage_pct": 2500,
    "max_transaction_cpu_usage": 150000,
    "min_transaction_cpu_usage": 100,
    "max_transaction_lifetime": 3600,
    "deferred_trx_expiration_window": 600,
    "max_transaction_delay": 3888000,
    "max_inline_action_size": 4096,
    "max_inline_action_depth": 6,
    "max_authority_depth": 6,
    "max_ram_size": 34359738368
  }
}
```