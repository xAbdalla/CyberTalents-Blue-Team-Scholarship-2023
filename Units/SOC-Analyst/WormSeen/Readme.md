# WormSeen

## Description
OOur EDR has flagged suspicious traffic from production endpoint, after reviewing the respective process generating the traffic and another alert has been alerted “Worm Detected” in our SIEM

You decided to escalate the case to IR team to further investigate and answer the below questions 
* What is the range of worm spreading (x.x.x.x/xx) ?
* Destination target port of the attack (XX)?
* How many hosts might be affected by the worm (XX)?

**Flag format: flag{Answer1:Answer2:Answer3}.**

## Files
worm.zip: https://hubchallenges.s3.eu-west-1.amazonaws.com/foren/worm.zip
* Password: **infected**

## Solution

### Flag
```
flag{192.168.1.0/24:22:85}
```