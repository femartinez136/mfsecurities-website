# MFSecurities.org - Business Cybersecurity Services

Official business cybersecurity services website for MFranklin, LLC.

## Services Offered
- Security Assessments ($500+)
- Compliance Roadmaps ($1,200+)
- Security Training ($800+)
- Quick Security Services ($150+)

## Architecture

This site is intentionally hosted separately from the personal mentorship platform (mfranklin.org) to demonstrate **defense in depth** security principles:

- **Infrastructure Isolation**: Separate GitHub repository and Cloudflare Pages project
- **Attack Surface Separation**: Compromise of one domain doesn't affect the other
- **Credential Isolation**: Different origins prevent session/cookie sharing
- **Independent Deployment**: Updates to personal site don't risk business operations

## Related Sites
- **Personal Site**: https://mfranklin.org ([Repository](https://github.com/femartinez136/mfranklin-website))
- **Business Site**: https://mfsecurities.org (this repository)

## Deployment
- **Hosting**: Cloudflare Pages
- **Framework**: Static HTML/CSS (no build required)
- **Domain**: mfsecurities.org
- **SSL**: Cloudflare managed certificate

## Local Development
```bash
# Simply open index.html in a browser
open index.html
```

No build process required - pure HTML/CSS site.

## Security
Security headers configured via `_headers` file:
- X-Frame-Options: DENY
- Content Security Policy (CSP)
- X-Content-Type-Options: nosniff
- Referrer-Policy

## Contact
For service inquiries: https://www.fiverr.com/mfrankline
