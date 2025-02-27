# Change list

The list of the most significant changes made in Netis Packet Agent over time.
## Netis Packet Agent 0.6.0
### Features
* Remove libpcap lib dependency
* Support daemonset capturing (in k8s & kvm)
* Support auto-detection of network interface
* Support multi-interface capturing
* Support auto-detction of the direction with mac
* Support MPLS encapsulate for ZMQ
* Support log module
* Support VXLAN port configurable(default is 4789) 

## Netis Packet Agent 0.5.2
### Features
* Supprot vlan packets

## Netis Packet Agent 0.5.1
### Features
* Supprot packet forword by vxlan

## Netis Packet Agent 0.5.0

### Features
* Support GRE direction in key.


## Netis Packet Agent 0.3.6

### Features
* Support agent control plane for agent daemon over zeromq.


## Netis Packet Agent 0.3.5

### Features
* Support option check for '--nofilter' option invalid usage. In version 0.3.5 or later, pktminerg will exit directly in the following cases:
    - if you enable '--nofilter' option without specifying gre bind device(-B) in online mode.
    - if you enable '--nofilter' option and gre bind device(-B) is same as packet captured interface(-i) in online mode. 

## Netis Packet Agent 0.3.4

### Features
* Support MTU discovery strategy.

## Netis Packet Agent 0.3.3

### Features
* Support send GRE packets to multi-remoteip
* Support send GRE packets from binded device (network interface).
* Support systemd

## Netis Packet Agent 0.3.2

### Features
* Add Windows support

## Netis Packet Agent 0.3.1

### Bug Fixes
* Remove rpm install boost library dependencies.


## Netis Packet Agent 0.3.0

Initial release.

### Features
* Capture packets from an NIC interface, encapsulate them with GRE and send them to a remote machine for monitoring and analysis. All with ease.

### Documentation:

* For first use: [README](README.md), [INSTALL](INSTALL.md), [USAGE](USAGE.md), [BUILD](BUILD.md), [CHANGES](CHANGES.md), [LICENSE](LICENSE.md).

### Packaging:

* Package for Linux installs EM64T bits.
* Linux installer allows root, RPM installs.
