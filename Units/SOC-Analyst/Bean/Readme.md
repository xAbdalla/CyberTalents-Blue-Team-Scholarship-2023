# Bean

## Description
Come back home Mr. Bean.

## Solution

The lab is hosted at CyberTalents website, so I can't share the generated URL.
You can find a similar lab at

**Introduction to Cybersecurity » Directory Traversal » [bean](https://www.vulnhub.com/entry/mr-bean-1,705/)**.

Let's open the URL in the browser.

<p align="center">
    <img src="./1.png">
</p>

Just a photo of Mr. Bean. Let's see the page source.

<p align="center">
    <img src="./2.png">
</p>

Nothing useful again! LEt's see if there is a robots.txt file.

<p align="center">
    <img src="./3.png">
</p>

There is not a robots.txt file. but we got a hint that the website is running on Nginx 1.13.0.

Now, let's try [dirsearch](https://github.com/maurosoria/dirsearch/) to find hidden directories.

<p align="center">
    <img src="./4.png">
</p>

We got a directory named `files`. Let's open it.

<p align="center">
    <img src="./5.png">
</p>

Let’s try to go back to previous directory by using Path Traversal attack, aims to access files and directories that are stored outside the web root folder.

```
http://bean.cybertalentslabs.com/files/../../../../../etc/passwd
```

<p align="center">
    <img src="./6.png">
</p>

It didn't work. Let's try to find a Nginx vulnerability.
I found this [article](https://www.acunetix.com/vulnerabilities/web/path-traversal-via-misconfigured-nginx-alias/) that explains how to exploit Nginx 1.13.0.

```
http://bean.cybertalentslabs.com/files/files../
```

<p align="center">
    <img src="./7.png">
</p>

<p align="center">
    <img src="./8.png">
</p>

We got the flag.

### Flag

```
FLAG{Nginx_nOt_aLWays_sEcUre_bY_The_waY}
```