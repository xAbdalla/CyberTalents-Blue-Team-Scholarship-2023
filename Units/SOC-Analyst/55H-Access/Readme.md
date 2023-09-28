# 55H Access

## Description

We observed a huge traffic towards our SSH Server

* X: How many source IPs attempting to connect  → Number
* Y: The Source IP with the most connections → x.x.x.x
* Z: The Source IP with the most connections country → xxxxxxx
* W: The Firewall action taken from the security control → xxxxxxx

**Flag format:** flag{X:Y:Z:W}

**Note:** our company uses Fortinet FortiGate firewall.

## Solution

### Flag

```text
flag{19:91.224.160.108:Finland:blocked}
```
