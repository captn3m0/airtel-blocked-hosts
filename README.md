# blocked-hosts
[![Statistics](https://img.shields.io/badge/sites-1,362-brightgreen)](https://github.com/captn3m0/airtel-blocked-hosts)
![GitHub last commit](https://img.shields.io/github/last-commit/captn3m0/airtel-blocked-hosts?color=blue)

This repository houses a periodically updated list of websites (root domains only) that are decidedly known to be blocked for Airtel Broadband users. A current list of blocked hostnames can be found [here](https://github.com/captn3m0/blocked-hosts/blob/airtel-fiber/airtel-fiber-blocked-hosts.txt).

**Note:** The lists published here are not fully representative of all hostnames that might be blocked by Airtel Fiber at a given time.

| date of test   | total hosts  | removed since last test    | added since last test            |
|----------------|--------------|----------------------------|----------------------------------|
| Nov 13 , 2021  | 1362         | -                          | -                                |

# Replication Instructions

The `input.txt` file is generated from the same primary sources as upstream, but limits itself to 100k domains from Alexa instead of 10M to keep the scan reasonably timed.

Airtel uses a CNAME to `dotblocking.dummy` to block DNS queries, so the output needs to be filtered accordingly.

# Scan Details

The scan was run from `AS24560` on a Airtel Premium Plan as [detailed here](https://www.airtel.in/wifi-plans).

# Credits

All of the code and work is based on [qurbat/blocked-hosts](https://github.com/qurbat/blocked-hosts/), which tracks ACT Fibernet in Bangalore. Please see the upstream for methodology, reproducibility instructions, and notes.