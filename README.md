# AetherCLI

![Go](https://img.shields.io/badge/Go-1.21+-00ADD8?style=for-the-badge&logo=go&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-00ADD8?style=for-the-badge)
![CI](https://img.shields.io/badge/CI-GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)
![CodeQL](https://img.shields.io/badge/CodeQL-Security-00ADD8?style=for-the-badge)
![Version](https://img.shields.io/badge/Version-v1.0.0-00ADD8?style=for-the-badge)

> Zero-dependency security scanner - only Go stdlib, no third-party packages

`security` `scanner` `zero-dependency` `port-scanner` `ssl` `cli` `golang` `network`

---

## What is it?

**AetherCLI** is A blazing-fast security scanner built with ZERO external dependencies. Only Go standard library: net, crypto, os. Port scanning, SSL analysis, banner grabbing - all in a single binary.

## Why should you care?

- **Fast** - Compiled Go binary, zero overhead
- **Secure** - CodeQL analysis + Dependabot
- **Offline-first** - Works without internet
- **Lightweight** - Single binary deployment
- **Developer-friendly** - Clean CLI with docs

---

## Features

- Zero third-party dependencies
- TCP/UDP port scanning
- SSL/TLS certificate analysis
- Banner grabbing
- HTTP header security checks
- DNS enumeration
- WHOIS lookup
- Subdomain discovery
- OS fingerprinting
- Single binary deployment

---

## Quick Start

### Prerequisites
- Go 1.21 or higher

### Install from source
```bash
git clone https://github.com/AetherCodeHQ/aethercli.git
cd aethercli
go build -o aethercli .
```

### Run
```bash
./aethercli --help
```

---

## Usage

./aethercli scan --target 192.168.1.1 --ports 1-1000  OR  ./aethercli ssl --target example.com  OR  ./aethercli audit --target example.com

---

## CLI Flags

| Flag | Description | Default |
|------|-------------|---------|
| `--path` | Target directory | `.` |
| `--format` | Output format (json, text) | `text` |
| `--output` | Output filename | `stdout` |
| `--verbose` | Enable verbose output | `false` |

---

## Development

```bash
git clone https://github.com/AetherCodeHQ/aethercli.git
cd aethercli
go build -o aethercli .
go test ./...
golangci-lint run
```

---

## Contributing

Contributions welcome! See [CONTRIBUTING.md](CONTRIBUTING.md).

## Security

Report to: aethercode.core@gmail.com | See [SECURITY.md](SECURITY.md)

## License

MIT License - see [LICENSE](LICENSE)

---

<p align="center">
  Built with love by <a href="https://github.com/AetherCodeHQ">AetherCode</a> | <a href="https://github.com/AetherCode-Core">AetherCode Core</a>
</p>
