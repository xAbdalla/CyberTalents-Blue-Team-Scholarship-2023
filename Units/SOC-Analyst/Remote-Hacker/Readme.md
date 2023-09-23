# Remote Hacker

## Description
Our SoC L1 reported that she received alert of suspicious login detected by company user “Kvasir” on 13/06/2022.

Please do check and return by your analysis: 

* X: Session Duration spent by the attacker on the system (HH:MM:SS)
* Y: The application used by the user after login (xxxx.exe)
* Z: Identify the SHA256 of this application W: Attacker IP address
* A: Attacker Machine host name

**Flag format:** flag{X:Y:Z:A}

## Files
remotehacker.tar: https://hubchallenges.s3.eu-west-1.amazonaws.com/foren/remotehacker.tar

## Solution

### Flag
```
flag{00:02:40:win32calc.exe:3E2300394C15B59A964EAB45D9EB96D317650E2F7448FD1B4AE825A134402B7A:192.168.1.58:Nitro}
```