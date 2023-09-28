# USB Case

## Description

Your Team Lead ask you to develop splunk use case for detecting USB plugged on any device in your environment. He shared with you also this [https://lantern.splunk.com/Security/Use_Cases](https://lantern.splunk.com/Security/Use_Cases).

Develop the use case and answer the below questions based on botsv1 dataset

* X: Date and time when the USB plugged on device  (YYYY-MM-DD:HH:MM:SS)
* Y: The Machine name
* Z: Name of the USB device

**Flag format:** flag{X:Y:Z:A}

## Solution

### Flag

```text
flag{2016-08-24:10:42:17:we8105desk:MIRANDA_PRI}
```
