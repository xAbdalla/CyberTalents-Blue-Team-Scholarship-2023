# Beans Detector

## Description
You have received the alert in your company WAF that web attack happened recently. Please check and identify the below details

**Follow the below format in order to submit the flag**

* X: Attacker IP Address
* Y: Name of vulnerability scanner used by the attacker
* Z: number of bytes in the sensitive file leaked
* W: Data and time of the successful attack (xx/xx/xxxx:xx:xx:xx)

**Flag Format:** flag{X:Y:Z:W}

## Files
beansdetectorlogs: https://hubchallenges.s3.eu-west-1.amazonaws.com/foren/beansdetectorlogs

## Solution

### Flag
```
flag{172.17.0.1:Wfuzz:49:12/06/2022:11:05:12}
```