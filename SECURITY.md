# Security Policy

## Reporting Security Issues

**Please do not report security vulnerabilities through public GitHub issues.**

Instead, report them privately:

1. **GitHub Security Advisories** (Preferred)
   - Go to the relevant repository (e.g., `tfgrid-compose`)
   - Click "Security" tab → "Advisories" → "Report a vulnerability"
   - Fill out the private security advisory form
   
2. **Direct Contact**
   - Open a private discussion in [GitHub Discussions](https://github.com/orgs/tfgrid-studio/discussions)
   - Tag repository maintainers with security details
   
3. **For Critical Issues**
   - Contact maintainers directly via their GitHub profiles

### What to Include

Please include as much of the following information as possible:

- Type of vulnerability
- Affected component(s)
- Step-by-step reproduction
- Potential impact
- Suggested fix (if you have one)

### Response Timeline

- **24 hours** - Initial acknowledgment
- **7 days** - Detailed response with assessment
- **30 days** - Fix or mitigation plan

## Supported Versions

| Version | Supported          |
| ------- | ------------------ |
| 2.0.x   | :white_check_mark: |
| 1.0.x   | :white_check_mark: |
| < 1.0   | :x:                |

## Security Best Practices

### For Users

**Credentials:**
- Never commit credentials to Git
- Use `.tfvars` files (gitignored) for sensitive data
- Rotate credentials regularly

**SSH Keys:**
- Use strong SSH keys (ED25519 or RSA 4096)
- Protect private keys with passphrases
- Never share private keys

**Network:**
- Use WireGuard for private access
- Keep VPN configurations secure
- Limit exposure of public IPs

### For Developers

**Code Review:**
- Review all pull requests for security issues
- Check for credential leaks
- Validate input sanitization

**Dependencies:**
- Keep dependencies updated
- Monitor for known vulnerabilities
- Use official package sources

**Infrastructure:**
- Follow principle of least privilege
- Enable audit logging
- Use encrypted connections

## Known Security Considerations

### TFGrid Compose

**State Files:**
- Terraform state files contain sensitive data
- Store securely (not in Git)
- Use remote state with encryption when possible

**Credentials:**
- TFGrid credentials required for deployment
- Store in `credentials.auto.tfvars` (gitignored)
- Never hardcode in scripts

**Network Access:**
- WireGuard provides encrypted VPN
- Mycelium provides overlay network
- Both are automatically configured

### TFGrid AI Agent

**Isolation:**
- Runs in isolated VM
- No access to local filesystem
- Qwen API key stored securely

**API Keys:**
- Store Qwen API key in environment variables
- Never commit to Git
- Rotate regularly

## Vulnerability Disclosure

### Our Commitment

- We will respond to security reports promptly
- We will keep you informed of our progress
- We will credit you (if desired) when the issue is fixed
- We will coordinate disclosure timing with you

### Disclosure Process

1. **Private Report** - You report the issue privately
2. **Acknowledgment** - We confirm receipt within 24 hours
3. **Investigation** - We assess and validate the issue
4. **Fix Development** - We develop and test a fix
5. **Coordinated Disclosure** - We agree on disclosure timing
6. **Public Release** - We release the fix and advisory

## Security Updates

Security updates will be:
- Released as soon as possible
- Announced in [GitHub Security Advisories](https://github.com/tfgrid-studio/tfgrid-compose/security/advisories)
- Documented in release notes
- Communicated to users

## Third-Party Dependencies

We regularly monitor and update:
- Terraform providers
- Ansible collections
- System packages
- Docker images
- Node.js packages

## Compliance

TFGrid Studio follows security best practices from:
- OWASP Top 10
- CIS Benchmarks
- NIST Guidelines

## Questions?

For security questions or concerns:
- **Security Issues:** Use GitHub Security Advisories in the relevant repository
- **General Questions:** [GitHub Discussions](https://github.com/orgs/tfgrid-studio/discussions) (for non-sensitive topics only)
- **Direct Contact:** Reach out to maintainers via GitHub

**Remember:** Never disclose security vulnerabilities publicly until coordinated disclosure.

---

**Thank you for helping keep TFGrid Studio secure!** 🔒
