# squarebash
> ![SquareBash Mainframe](https://github.com/Gr3ytrac3/SquareBash/blob/18b520f89f5cdb3ee6d6de16220e9b2dde35797f/squarebashmainframe.png)

A comprehensive collection of bash scripts, tools, and frameworks for system administration, security, and automation.
[![License](https://img.shields.io/badge/license-MIT-9D00FF)](https://github.com/Gr3ytrac3/SquareBash/blob/f319893654018e75289e8defeaa3abf255e23d7a/LICENSE)
[![Safe Usage](https://img.shields.io/badge/Safe%20Usage-Research%20%26%20Education-blue)](SAFE_USAGE.md)
## Repository Structure

```
bash-projects/
├── README.md
├── LICENSE
├── CONTRIBUTING.md
├── .github/
│   ├── workflows/
│   │   ├── shellcheck.yml
│   │   └── tests.yml
│   ├── ISSUE_TEMPLATE/
│   │   ├── bug_report.md
│   │   └── feature_request.md
│   └── PULL_REQUEST_TEMPLATE.md
├── beginner/
│   ├── dotfile-manager/
│   ├── auto-installer/
│   └── syshealth/
├── intermediate/
│   ├── network-scanner/
│   ├── system-hardener/
│   └── audit-toolkit/
├── advanced/
│   ├── kernelscout/
│   ├── offensive-recon-framework/
│   ├── kernelpatch-detector/
│   ├── stealth-persistence-framework/
│   └── privesc-automator/
├── utilities/
│   ├── common-functions/
│   ├── logging/
│   └── error-handling/
├── docs/
│   ├── bash-best-practices.md
│   ├── security-considerations.md
│   ├── testing-guide.md
│   └── deployment-guide.md
├── tests/
│   ├── unit/
│   ├── integration/
│   └── test-utils.sh
└── examples/
    ├── basic-scripts/
    ├── advanced-examples/
    └── real-world-scenarios/
```

## Project Categories

### 🟢 Beginner Projects
Perfect for those starting with bash scripting and system administration.

- **[Dotfile Manager](beginner/dotfile-manager/)** - Synchronize configuration files across machines
- **[Auto Installer Script](beginner/auto-installer/)** - Distribution-aware package installer
- **[SysHealth Report Generator](beginner/syshealth/)** - System performance monitoring

### 🟡 Intermediate Projects
For users with solid bash fundamentals looking to tackle more complex scenarios.

- **[Network Scanner CLI](intermediate/network-scanner/)** - Unified network discovery interface
- **[System Hardener Script](intermediate/system-hardener/)** - Security best practices automation
- **[Audit Toolkit](intermediate/audit-toolkit/)** - Security misconfiguration detection

### 🔴 Advanced Projects
Sophisticated tools for security professionals and experienced system administrators.

- **[KernelScout](advanced/kernelscout/)** - Kernel analysis and vulnerability detection
- **[Offensive Recon Framework](advanced/offensive-recon-framework/)** - Modular reconnaissance toolkit
- **[KernelPatch Detector](advanced/kernelpatch-detector/)** - Unauthorized kernel modification detection
- **[Stealth Persistence Framework](advanced/stealth-persistence-framework/)** - Educational persistence demonstration
- **[Privilege Escalation Automator](advanced/privesc-automator/)** - Comprehensive privilege escalation toolkit

## Quick Start

```bash
# Clone the repository
git clone https://github.com/yourusername/bash-projects.git
cd bash-projects

# Make scripts executable
find . -name "*.sh" -exec chmod +x {} \;

# Run a beginner project
cd beginner/syshealth
./syshealth.sh

# Try an intermediate tool
cd ../../intermediate/network-scanner
./netscan.sh --cidr 192.168.1.0/24
```

## Features

- 📁 **Well-organized structure** - Projects categorized by complexity level
- 🧪 **Comprehensive testing** - Unit and integration tests included
- 📚 **Detailed documentation** - Each project includes thorough README files
- 🔒 **Security-focused** - Tools for security assessment and system hardening
- ⚡ **Production-ready** - Scripts designed for real-world usage
- 🛠️ **Utilities included** - Common functions and error handling modules

## Installation

### Prerequisites

- Bash 4.0 or higher
- Standard Linux utilities (find, grep, awk, etc.)
- Root access (for some security tools)

### System Dependencies

Most projects will automatically check for and install required dependencies. For manual installation:

```bash
# Ubuntu/Debian
sudo apt-get update
sudo apt-get install curl wget nmap netdiscover arp-scan

# RHEL/CentOS/Fedora
sudo yum install curl wget nmap netdiscover arp-scan

# Arch Linux
sudo pacman -S curl wget nmap netdiscover arp-tools
```

## Usage Examples

### System Health Monitoring
```bash
cd beginner/syshealth
./syshealth.sh --format json --modules cpu,memory,disk
```

### Network Discovery
```bash
cd intermediate/network-scanner
./netscan.sh --cidr 192.168.1.0/24 --type full --output csv
```

### Security Hardening
```bash
cd intermediate/system-hardener
sudo ./harden.sh --modules services,kernel,firewall --dry-run
```

## Testing

Run the test suite to ensure all scripts work correctly on your system:

```bash
# Run all tests
./tests/run_all_tests.sh

# Run tests for specific project
./tests/run_tests.sh beginner/syshealth

# Run shellcheck on all scripts
find . -name "*.sh" -exec shellcheck {} \;
```

## Contributing

Contributions are welcome! Please read [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines.

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-tool`)
3. Commit your changes (`git commit -m 'Add amazing tool'`)
4. Push to the branch (`git push origin feature/amazing-tool`)
5. Open a Pull Request

### Coding Standards

- Follow bash best practices (see [docs/bash-best-practices.md](docs/bash-best-practices.md))
- Include comprehensive error handling
- Add logging where appropriate
- Write tests for new functionality
- Update documentation

## Security Considerations

⚠️ **Important Security Notice**: Many tools in this repository are designed for security testing and system administration. Please note:

- Advanced tools are for **authorized testing only**
- Always get proper permission before running security tools
- Test in isolated environments first
- Some tools require root privileges
- Be aware of legal implications in your jurisdiction

See [docs/security-considerations.md](docs/security-considerations.md) for detailed guidelines.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Author

**[Your Name]**
- GitHub: [@yourusername](https://github.com/yourusername)
- Email: your.email@example.com

## Acknowledgments

- Thanks to the bash community for inspiration
- Security researchers who document techniques
- Open source contributors who make tools like shellcheck possible

## Support

If you find this repository helpful:

- ⭐ Star the repository
- 🍴 Fork it for your own use
- 🐛 Report issues
- 💡 Suggest improvements

---

**Disclaimer**: These tools are for educational and authorized testing purposes only. Users are responsible for complying with applicable laws and obtaining proper authorization before using security-related tools.
