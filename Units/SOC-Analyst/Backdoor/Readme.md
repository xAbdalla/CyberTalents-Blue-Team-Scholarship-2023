# Backdoor

## Description
Our server compromised due to known vulnerability introduced from many years, Kindly check and identify this flow 

* X: Attack source → EX. “Internal/External”
* Y: The Source IP → x.x.x.x
* Z: CVE Num of the attack → xxx
* W: Destination Mac Address

**Flag format: flag{X:Y:Z:W}**

## Files
backdoor.pcap: https://hubchallenges.s3.eu-west-1.amazonaws.com/foren/backdoor.pcap

## Solution

### Flag
```
flag{Internal:192.168.1.58:CVE-2011-2523:08:00:27:66:e3:8b}
```