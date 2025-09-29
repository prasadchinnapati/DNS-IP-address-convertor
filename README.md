#DNS-IP-address-convertor
Converts multiple domain names to IP addresses.
Stores resolved IP addresses persistently in a JSON file (dns_cache.json).

On subsequent runs, if a domain was previously resolved, it asks the user whether to use the cached IPs or perform a fresh DNS lookup.

Mimics a simple DNS cache system.

Allows the user to clear cache if needed.
On start, user chooses to resolve domains or clear cache.

When resolving, it loads cache from dns_cache.json.

For each domain, if cached IPs exist, user is prompted to use them or fetch fresh.

Freshly resolved IPs update the cache.

Cache persists across runs.

# Example interaction:

DNS Resolver with Cache
Options:
1. Resolve domains
2. Clear cache
Select option (1/2): 1
Enter domain names separated by spaces or commas: google.com, github.com
Use cached IPs for google.com?
['142.250.72.206', '142.250.72.238'] (y/n): n
IP addresses for google.com:
142.250.72.206, 142.250.72.238
Use cached IPs for github.com?
 ['140.82.114.4'] (y/n): y
IP addresses for github.com: 140.82.114.4

