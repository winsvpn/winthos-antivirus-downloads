# Winthos AI & Antivirus Public Binary Releases

Official public binary distribution and cryptographic checksum repository for **Winthos AI & Antivirus** (`https://www.winthosantivirus.com`).

This repository hosts release checksum manifests, detached OpenSSL ECDSA P-256 attestation signatures, third-party open-source notices, and binary release assets only. Source code is maintained in private custody by Win's VPN Inc.

## Verify Any Download

```bash
curl -fsSLO https://www.winthosantivirus.com/releases/SHA256SUMS
curl -fsSLO https://www.winthosantivirus.com/releases/SHA256SUMS.sig
curl -fsSLO https://www.winthosantivirus.com/releases/release-attestation.pub.pem

openssl dgst -sha256 \
  -verify release-attestation.pub.pem \
  -signature SHA256SUMS.sig \
  SHA256SUMS

# macOS: shasum -a 256 --ignore-missing -c SHA256SUMS
# Linux: sha256sum --ignore-missing -c SHA256SUMS
```

## Official Website & Security Policy

* Website & Download Matrix: https://www.winthosantivirus.com
* Security & Attestation Guide: https://www.winthosantivirus.com/security.html
* Zero-Ad-ID Privacy Policy: https://www.winthosantivirus.com/privacy.html
