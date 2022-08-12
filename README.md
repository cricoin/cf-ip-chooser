# CF-IP-Chooser

Select the best IP address for your CDN server. This is useful if you have multiple IP addresses and want to choose the one that is most likely to be used.

Both Cloudflare and Cloudfront CDN servers are supported. 

## Quick Start

```bash

```

## [Optional] Update IP address

1. Update Cloudflare IP list

```bash
# ipv4
curl -o cloudflare-ip.txt https://www.cloudflare.com/ips-v4

# ipv6
curl -o cloudflare-ipv6.txt https://www.cloudflare.com/ips-v6
```

2. Update Cloudfront IP list

```bash
curl https://d7uri8nf7uskq.cloudfront.net/tools/list-cloudfront-ips | grep -o -E "([0-9]{1,3}[\.]){3}[0-9]{1,3}\/[0-9]+" > cloudfront-ip.txt
```


## References

https://github.com/XIU2/CloudflareSpeedTest