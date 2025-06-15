# 🕵️ OSINT MCP Server

A comprehensive Open Source Intelligence (OSINT) toolkit that integrates with Claude Desktop through the Model Context Protocol (MCP). This server provides access to a wide range of OSINT tools and techniques for cybersecurity professionals, researchers, and investigators.

## 🚀 Features

### Network & Infrastructure Analysis
- **Nmap Scanner** ✅ - Network discovery and security auditing
- **Masscan Scanner** 🔄 - High-speed port scanner
- **Shodan Integration** 🔄 - Internet-connected device search
- **Censys Integration** 🔄 - Internet device and certificate search
- **Subdomain Discovery** 🔄 - Subfinder, Amass, DNS reconnaissance

### Web Application Analysis
- **Technology Detection** 🔄 - WhatWeb, Wappalyzer integration
- **Directory Scanning** 🔄 - Dirb, Gobuster directory enumeration
- **SSL/TLS Analysis** 🔄 - Certificate and security assessment
- **Wayback Machine** 🔄 - Historical website analysis

### Domain & DNS Intelligence
- **WHOIS Lookup** 🔄 - Domain registration information
- **DNS Analysis** 🔄 - Comprehensive DNS record analysis
- **Domain Typosquatting** 🔄 - DNSTwist domain variations
- **Reputation Checking** 🔄 - VirusTotal, URLVoid integration

### Social Media & People Intelligence
- **Username Search** 🔄 - Sherlock username enumeration
- **Social Media Analysis** 🔄 - Platform-specific intelligence
- **Professional Networks** 🔄 - LinkedIn intelligence gathering

### Email & Communication
- **Email Verification** 🔄 - Holehe, H8mail integration
- **Email Reputation** 🔄 - EmailRep analysis
- **Phone Number Analysis** 🔄 - Phone number intelligence

### Media Analysis
- **EXIF Data Extraction** 🔄 - Image metadata analysis
- **Reverse Image Search** 🔄 - Image source identification
- **Steganography Detection** 🔄 - Hidden data detection

### Cryptocurrency & Blockchain
- **Blockchain Explorer** 🔄 - Transaction and address analysis
- **Crypto Intelligence** 🔄 - Cryptocurrency investigation tools

### Threat Intelligence
- **Breach Checking** 🔄 - Data breach verification
- **IOC Analysis** 🔄 - Indicator of Compromise analysis
- **Dark Web Monitoring** 🔄 - Tor network analysis

## 📋 Prerequisites

- Python 3.8 or higher
- Claude Desktop (latest version)
- Internet connection for API-based tools
- Administrative privileges for tool installation

## 🛠 Installation

### Quick Installation (Recommended)

```bash
# Clone the repository
git clone https://github.com/yourusername/osint-mcp-server.git
cd osint-mcp-server

# Run the installation script
chmod +x install.sh
./install.sh
```

### Manual Installation

```bash
# Install Python dependencies
pip install -r requirements.txt

# Install external tools
python scripts/install_dependencies.py

# Configure Claude Desktop
python scripts/setup_claude.py
```

### Docker Installation

```bash
# Build and run with Docker Compose
docker-compose up -d
```

## 🔧 Configuration

1. **Copy environment file:**
   ```bash
   cp .env.example .env
   ```

2. **Configure API keys in `.env`:**
   ```bash
   SHODAN_API_KEY=your_shodan_key
   VIRUSTOTAL_API_KEY=your_virustotal_key
   CENSYS_API_ID=your_censys_id
   CENSYS_SECRET=your_censys_secret
   ```

3. **Configure Claude Desktop:**
   The installation script automatically configures Claude Desktop. Manual configuration details are in `docs/usage/CLAUDE_INTEGRATION.md`.

## 🚀 Quick Start

1. **Start the MCP server:**
   ```bash
   python -m osint_mcp.main
   ```

2. **Open Claude Desktop** and start using OSINT tools:
   ```
   "Can you scan the domain example.com for subdomains?"
   "What technologies are running on https://example.com?"
   "Check if the email test@example.com has been in any data breaches"
   ```

## 📖 Documentation

- [Installation Guide](docs/installation/INSTALL.md)
- [Quick Start Guide](docs/usage/QUICK_START.md)
- [Available Tools](docs/usage/TOOLS.md)
- [Usage Examples](docs/usage/EXAMPLES.md)
- [Troubleshooting](docs/installation/TROUBLESHOOTING.md)

## 🔐 Security & Ethics

This tool is designed for legitimate security research, penetration testing, and investigative purposes. Users must:

- Comply with all applicable laws and regulations
- Obtain proper authorization before testing systems
- Respect privacy and data protection laws
- Follow responsible disclosure practices

See [Security Guidelines](docs/security/SECURITY.md) and [Ethical Guidelines](docs/security/ETHICS.md) for more information.

## 🤝 Contributing

We welcome contributions! Please read our [Contributing Guidelines](docs/development/CONTRIBUTING.md) before submitting pull requests.

### Adding New Tools

See [Adding Tools Guide](docs/development/ADDING_TOOLS.md) for instructions on integrating new OSINT tools.

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## ⚠️ Disclaimer

This software is provided for educational and authorized testing purposes only. The authors are not responsible for any misuse or damage caused by this tool. Users are solely responsible for ensuring their activities comply with applicable laws and regulations.

## 🆘 Support

- 📖 Check the [documentation](docs/)
- 🐛 Report bugs via [GitHub Issues](https://github.com/yourusername/osint-mcp-server/issues)
- 💬 Join our [Discord community](https://discord.gg/yourdiscord)
- 📧 Email: support@yourdomain.com

## 🔄 Status Legend

- ✅ **Implemented** - Fully functional
- 🔄 **In Development** - Currently being developed
- 📋 **Planned** - Scheduled for future release
- ⚠️ **Experimental** - Beta/testing phase

---

**Star ⭐ this repository if you find it useful!**
