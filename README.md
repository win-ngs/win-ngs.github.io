# win-ngs

A portal site for **NGS (Next-Generation Sequencing) analysis tools that run on Windows**.

Live site: **https://win-ngs.github.io/**

Most NGS tools assume Linux or macOS, and information about running them natively on
Windows is scattered. This site collects in one place:

- Tools that work on Windows out of the box (official Windows binaries)
- Binaries we compiled ourselves from upstream sources
- Curated links to useful external tools

## Featured tools

### Basic RNA-seq

| Tool | Role | Source |
| --- | --- | --- |
| [Falco 1.3.0](https://github.com/win-ngs/falco-windows-build) | Read QC | win-ngs build |
| [STAR 2.7.11b](https://github.com/win-ngs/star-windows-build) | Spliced alignment | win-ngs build |
| [featureCounts (Subread 2.1.1)](https://subread.sourceforge.net/) | Read counting | Official upstream binary |

See the [portal site](https://win-ngs.github.io/) for the full list.

## Repository layout

```
.
├── index.html   # Main portal page
├── style.css    # Styling (dark/light mode via prefers-color-scheme)
└── README.md
```

This is a plain static site. No build step, no Jekyll, no dependencies.
GitHub Pages serves `index.html` directly.

## Local preview

Just open `index.html` in a browser. For a proper local server:

```powershell
python -m http.server 8000
```

Then visit http://localhost:8000/.

## Contributing

Additions, corrections, and broken-link reports are welcome via
[Issues](https://github.com/win-ngs/win-ngs.github.io/issues) and
[Pull Requests](https://github.com/win-ngs/win-ngs.github.io/pulls).

When adding a tool, please include:

- **Role** (QC, alignment, variant calling, etc.)
- **Upstream link** to the original project
- **Build environment** if it's a custom build (e.g. MSYS2 MSYS / UCRT64)
- **License** (inherited from upstream)
- **SHA256** of the distributed archive if applicable

## Related repositories

- [win-ngs/falco-windows-build](https://github.com/win-ngs/falco-windows-build) — Falco Windows build
- [win-ngs/star-windows-build](https://github.com/win-ngs/star-windows-build) — STAR Windows build

## License

The portal site (this repository) is provided as-is for reference.
Each distributed binary inherits the license of its upstream project — please
review the upstream license before use.
