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

## License

The portal site (this repository) is provided as-is for reference.
Each distributed binary inherits the license of its upstream project — please
review the upstream license before use.
