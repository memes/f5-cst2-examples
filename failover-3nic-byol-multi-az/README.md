# 3NIC Failover with BYOL and multiple AZs

This folder contains an example to demonstrate deploying a 3NIC BIG-IP HA pair
that are using declared license keys, and deployed to separate AZs in a region.

## Differences from upstream CSTv2 examples

### gdm-config.yaml

The [gdm-config.yaml] file is based on the upstream file [sample_failover_existing_network.yaml], but modified to import GDM resources through GitHub links, and to support
multiple zones under the `zones` key.

### custom.py

[custom.py] contains an edited version of upstream's [failover-existing-network.py]
to support deploying to multiple availability zones.

### custom.py.schema

[custom.py.schema] contains an edited version of upstream's [failover-existing-network.py.schema] to support declaring multiple availability zones.

[gdm-config.yaml]: gdm-config.yaml
[sample_failover_existing_network.yaml]: https://github.com/F5Networks/f5-google-gdm-templates-v2/blob/v2.4.0.0/examples/failover/sample_failover_existing_network.yaml
[custom.py]: custom.py
[failover-existing-network.py]: https://github.com/F5Networks/f5-google-gdm-templates-v2/blob/v2.4.0.0/examples/failover/failover-existing-network.py
[custom.py.schema]: custom.py.schema
[failover-existing-network.py.schema]: https://github.com/F5Networks/f5-google-gdm-templates-v2/blob/v2.4.0.0/examples/failover/failover-existing-network.py.schema
