# ipify

ipify is a simple, reliable, and high-availability API service that allows developers to get their public IP address (IPv4 or IPv6). Built with a focus on transparency, performance, and open access, ipify is trusted by millions of developers, enterprises, and open-source projects. It is fully open-source, logs no visitor data, and is designed for both humans and machines.The service is sustainably funded and maintained by its creator, with support from the open-source community and ongoing sponsorship to ensure long-term availability and operational continuity

## Documentation

- [Official ipify Docs](https://www.ipify.org) — Overview, setup, and FAQs.
- [ipify GitHub Repository](https://github.com/rdegges/ipify-api) — Source code and deployment info.
- [ipify Blog](https://rdegges.com/) — Posts from the creator and updates.

## API Endpoints

All endpoints support **plain text**, `?format=json`, and `?format=jsonp&callback=yourFunction`.

- **[Universal Endpoint (IPv4 or IPv6)](https://api.ipify.org)** — Automatically detects the best IP version.
- **[IPv4-only Endpoint](https://api4.ipify.org)** — Always returns the IPv4 address.
- **[IPv6-only Endpoint](https://api6.ipify.org)** — Returns the IPv6 address if available.
- **[IPv6 alias (fallback-friendly)](https://api64.ipify.org)** — Same as `api6.ipify.org`, but useful in clients handling both stacks.

### Quick Examples

- **Plain text (default):**  
  `curl https://api.ipify.org` → `203.0.113.45`

- **JSON format:**  
  `curl https://api.ipify.org?format=json` → `{"ip":"203.0.113.45"}`

- **JSONP callback:**  
  `https://api.ipify.org?format=jsonp&callback=myCallback` → `myCallback({"ip":"203.0.113.45"})`

## Language Libraries

- [Python: `requests`](https://github.com/rdegges/ipify-api#python-example)
- [JavaScript / Node.js](https://github.com/rdegges/ipify-api#nodejs-example)
- [Go](https://github.com/rdegges/ipify-api#go-example)
- [Java](https://github.com/rdegges/ipify-api#java-example)
- [Ruby](https://github.com/rdegges/ipify-api#ruby-example)

## Service Policies

- **Unlimited usage** — No rate limits for standard use.
- **High availability** — Globally distributed infrastructure with automatic failover.
- **No logging** — ipify does not collect or store IP addresses or visitor information.
- **Open-source** — Entire service is published and maintained openly on GitHub.
- **Commercial and free use** — Used by both personal projects and large enterprises.

### Best Practices

- Implement client-side caching where possible to reduce redundant requests.
- Use [`api64.ipify.org`](https://api64.ipify.org) for IPv6-aware clients to simplify fallback logic.
- Always use HTTPS to protect IP data in transit.

## Support & Contributions

- [GitHub Issues](https://github.com/rdegges/ipify-api/issues) — Report bugs or request features.
- [Author Contact](https://rdegges.com/contact/) — Reach out to Randall Degges.
- [Pull Requests](https://github.com/rdegges/ipify-api/pulls) — Contribute to the open-source project.

## Maintenance Metadata

- **Last updated:** 2025-10-11  
- **Review cadence:** Quarterly (Jan, Apr, Jul, Oct)  
- **Maintained by:** [Randall Degges](https://rdegges.com)  
- **AI/robots notice:** This file supplements ipify’s `robots.txt` and `sitemap.xml`. It is designed to guide language models and automated agents to respectful and correct usage of ipify resources.
