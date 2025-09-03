# 🔍 nslookup & dig Full Commands Cheatsheet  

## 📌 nslookup Commands  

| Command | Description |
|---------|-------------|
| `nslookup example.com` | Find IP address (A record) of a domain. |
| `nslookup 8.8.8.8` | Reverse lookup (IP → domain, PTR record). |
| `nslookup -type=A example.com` | Query IPv4 address record. |
| `nslookup -type=AAAA example.com` | Query IPv6 address record. |
| `nslookup -type=MX example.com` | Get mail servers (MX records). |
| `nslookup -type=NS example.com` | Find authoritative name servers. |
| `nslookup -type=TXT example.com` | Show TXT records (SPF, DKIM, DMARC). |
| `nslookup -type=CNAME example.com` | Get alias (CNAME record). |
| `nslookup -type=SOA example.com` | Start of Authority record. |
| `nslookup -type=PTR 8.8.8.8` | Perform reverse lookup. |
| `nslookup -type=ANY example.com` | Fetch all available DNS records (restricted on some servers). |
| `nslookup example.com 1.1.1.1` | Query using a specific DNS server (Cloudflare). |
| `nslookup -port=53 example.com` | Query a specific port (default 53). |

---

## 📌 dig Commands  

| Command | Description |
|---------|-------------|
| `dig example.com` | Query A record (default). |
| `dig example.com A` | Query IPv4 address. |
| `dig example.com AAAA` | Query IPv6 address. |
| `dig example.com MX` | Get mail exchange records. |
| `dig example.com NS` | Get authoritative name servers. |
| `dig example.com TXT` | Show TXT records (SPF, DKIM, etc.). |
| `dig example.com CNAME` | Query canonical name (alias). |
| `dig example.com SOA` | Get Start of Authority record. |
| `dig -x 8.8.8.8` | Reverse lookup (PTR record). |
| `dig example.com ANY` | Query all records (may be restricted). |
| `dig @8.8.8.8 example.com` | Use Google DNS instead of system default. |
| `dig +short example.com` | Short output (just the IP address). |
| `dig +trace example.com` | Trace DNS resolution path (root → TLD → authoritative). |
| `dig +noall +answer example.com` | Show only the answer section. |
| `dig +stats example.com` | Display query statistics. |
| `dig +norecurse example.com` | Disable recursive query. |
| `dig +recurse example.com` | Force recursive query. |
| `dig +dnssec example.com` | Request DNSSEC records. |
| `dig -p 5353 example.com` | Query using a non-standard port (default is 53). |

---
