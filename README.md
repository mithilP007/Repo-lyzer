<h1 align="center">Repo-lyzer</h1>
<p align="center">
  <img src="https://res.cloudinary.com/dhyii4oiw/image/upload/v1767324445/Screenshot_2026-01-02_085503_ros5gz.png" alt="Repo-lyzer Logo" width="300">
</p>

**Repo-lyzer** is a modern, terminal-based CLI tool written in **Golang** that analyzes GitHub repositories and presents insights in a beautifully formatted, interactive dashboard.

---

## Features
- **Deep Analytics** – Repository health, maturity scores, and bus factor.
- **Interactive TUI** – Fully navigable keyboard-driven menu system.
- **Visual Data** – Language breakdown bars and horizontal commit graphs.
- **File Explorer** – Browse repository structures directly in the dashboard.
- **Multi-Format Export** – Save reports as JSON, Markdown, CSV, or HTML.

---

## Quick Start

### Installation
```bash
go install [github.com/agnivo988/Repo-lyzer@v1.0.6](https://github.com/agnivo988/Repo-lyzer@v1.0.6)
repo-lyzer
```

### Basic Usage
```bash
# Get a 5-line quick summary
repo-lyzer summary golang/go

# Run full interactive analysis
repo-lyzer analyze microsoft/vscode
```

---

## Architecture Overview

```
┌────────────────────────────────────────────┐
│               main.go                      │
└────────────────────────────────────────────┘
                    │
                    ▼
┌────────────────────────────────────────────┐
│                 cmd/                       │
└────────────────────────────────────────────┘
                    │
                    ▼
┌────────────────────────────────────────────┐
│             internal/ui/                   │
└────────────────────────────────────────────┘
          │           │           │
          ▼           ▼           ▼
┌──────────────┐ ┌──────────────┐ ┌──────────────┐
│   github     │ │   analyzer   │ │   output     │
└──────────────┘ └──────────────┘ └──────────────┘
```

---

## Documentation

### For Contributors
- [ARCHITECTURE.md](docs/ARCHITECTURE.md) – Complete architecture guide  
- [ANALYZER_INTEGRATION.md](docs/ANALYZER_INTEGRATION.md) – Adding new analyzers  
- [IMPLEMENTATION_DETAILS.md](docs/IMPLEMENTATION_DETAILS.md) – Technical deep dive
- [PROJECT STRUCTURE.md](docs/PROJECT_STRUCTURE.md) - Project Structure and Workflow

### Reference
- [DOCUMENTATION_INDEX.md](docs/DOCUMENTATION_INDEX.md) – Master index  
- [QUICK_REFERENCE.md](docs/QUICK_REFERENCE.md) – Quick usage guide  
- [CHANGE_LOG.md](docs/CHANGE_LOG.md) – Version history  

---

## Maintainers & Contributors
### Maintainer: @agnivo988

<p align="left">
<a href="https://github.com/Aamod007"><img src="https://github.com/Aamod007.png" width="40" height="40" alt="Aamod007"></a>
<a href="https://github.com/Aditya8369"><img src="https://github.com/Aditya8369.png" width="40" height="40" alt="Aditya8369"></a>
</p>

---

## License
**MIT License © 2026 Agniva Mukherjee**
