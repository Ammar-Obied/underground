# 🌍 Underground — City Recommendations CLI

> A super-secret underground organisation for global awesomeness.  
> Discover the best cafés, bars, and restaurants across cities worldwide — straight from the terminal.

---

## 📖 About

**Underground** is a community-driven directory of hidden gems: cafés, bars, and restaurants curated by locals in cities around the world. This repository pairs that data with a Python CLI tool (`tool.py`) that lets you explore, search, and browse entries without leaving your terminal.

Cities currently covered include Berlin, Cologne, Munich, Melbourne, Tokyo, Paris, Zurich, and many more.

---

## 🚀 Quick Start

### 1. Clone the repository

```bash
git clone https://github.com/Ammar-Obied/underground.git
cd underground
```

### 2. Run the tool

```bash
python tool.py clone          # download/update the data
python tool.py list           # browse all cities
python tool.py list Berlin    # see categories in Berlin
python tool.py show Cologne bars   # show bar listings in Cologne
python tool.py search coffee  # search everywhere
```

---

## 🛠 Requirements

- Python 3.10 or newer
- Git (for the `clone` command)
- No external Python packages required

---

## 📂 Repository Structure

```
underground/
├── Berlin/
│   ├── bars.html
│   └── cafes.html
├── Cologne/
│   └── bars.html
├── Munich/
│   └── restaurants.html
├── Tokyo/
│   └── restaurants/
├── ...
├── tool.py          ← CLI tool
├── README.md
└── LICENSE
```

Each city folder contains HTML files organised by category (bars, cafes, restaurants). Anyone can contribute by adding or improving entries.

---

## 🔧 CLI Reference

| Command | Description |
|---|---|
| `python tool.py clone` | Clone or update the repo locally |
| `python tool.py list` | List all cities and their categories |
| `python tool.py list <City>` | List categories for a specific city |
| `python tool.py show <City>` | Show all entries for a city |
| `python tool.py show <City> <category>` | Show entries for one category |
| `python tool.py search <term>` | Full-text search across all cities |

**Options:**

```
--repo PATH    Path to local repo clone (default: ~/underground)
```

---

## 🤝 Contributing

Contributions are very welcome! You can:

- Add a new city folder with an HTML file
- Improve existing listings
- Fix typos or broken links

Please read [CONTRIBUTING.md](CONTRIBUTING.md) before opening a pull request.

---

## 📄 License

This project is licensed under the **MIT License** — see [LICENSE](LICENSE) for details.
