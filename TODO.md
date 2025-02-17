Things that could be implemented:

* FcrDNS check (also for mx)
* mta-sts syntax and consistency
* mta-sts: warn about old-style draft syntax
* mta-sts: warn about short max-age (RFC: "weeks or greater")
* SPF syntax
* Warn about old-style SPF records
* SPF all must be last
* SPF number of lookups restricted
* SPF CIDR net with masked 1 bits (probably not RFC incompliant)
* DMARC syntax
* DMARC mailto and reporting mail consistency
* unexpected leading/trailing whitespaces in TXT records
* SMTP TLS reporting syntax
* ANY amplification
* Warn about pre-standard TLS RPT records https://datatracker.ietf.org/doc/draft-ietf-uta-smtp-tlsrpt/16/
* DNSKEY correctness/sytax checks
* Warn about very low TTLs https://blog.apnic.net/2019/11/12/stop-using-ridiculously-low-dns-ttls/
* Warn about obsolete Sender ID/spf2.0 records https://datatracker.ietf.org/doc/status-change-change-sender-id-to-historic/
* CAA record basic correctness
* MX is not allowed to be a CNAME record, see https://www.cloudflare.com/learning/dns/dns-records/dns-mx-record/
* CNAME and conflicting other records (e.g., MX) at the same time
* DKIM key syntax, key type match, encoding (RSA PKCS #8, not #1, ed25519 raw encoding)
