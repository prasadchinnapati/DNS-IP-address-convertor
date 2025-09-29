# DNS-IP-address-convertor
Converts multiple domain names to IP addresses.
Stores resolved IP addresses persistently in a JSON file (dns_cache.json).

On subsequent runs, if a domain was previously resolved, it asks the user whether to use the cached IPs or perform a fresh DNS lookup.

Mimics a simple DNS cache system.

Allows the user to clear cache if needed.
# On start, user chooses to resolve domains or clear cache.

When resolving, it loads cache from dns_cache.json.

For each domain, if cached IPs exist, user is prompted to use them or fetch fresh.

Freshly resolved IPs update the cache.

Cache persists across runs.
