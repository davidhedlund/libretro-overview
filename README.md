# Libretro Core Metadata & Buildbot Audit Pipeline

> 🔍 **Quick Access:** **[Complete Master Report (`docs/all.md`)](docs/all.md)** — View all core metadata, documentation status, and OS/architecture support matrices combined in a single document.

## Overview & Goal

The goal of this project is to consolidate key technical data, metadata, and core information into organized, easy-to-reference tables. Having a centralized overview like this helps speed up research, streamline decision-making, and eliminate the need to repeatedly look up scattered details across different sources.

This aggregated data provides a convenient overview of supported operating systems and architectures for users, while also serving as a practical diagnostic tool for developers to identify missing or obsolete `.info` files and documentation across Libretro projects.

This repository serves as an automated metadata parser and report generator that cross-references local Libretro core info files, documentation indexes, and Libretro Buildbot binary availability across platforms and architectures.

Feedback, ideas, and suggestions for additional data points to make this even more useful for contributors are always welcome! Feel free to open an issue or start a discussion.

## Features

- **Automated Data Fetching**: Retrieves the latest `.info` file archives and Libretro documentation indexes.

- **Buildbot Auditing**: Scans nightly Buildbot indexes across multiple platforms (Android, Apple, GNU/Linux, Nintendo, PlayStation, Windows, etc.).

- **Data Standardization**: Converts raw Buildbot indexes into normalized JSON data (`cache/core-index.json`).

- **Comprehensive Markdown Reporting**: Generates interactive cross-reference tables and OS/architecture support matrices.

## Published Reports (`docs/`)

> [!NOTE]
> All Markdown files inside the `docs/` directory are **automatically generated** on a daily schedule via GitHub Actions running `generate.sh`. Any manual changes made to files in `docs/` will be overwritten.

Standalone category breakdowns (such as specific core file availability, documentation status, and individual OS/architecture matrices) can be found in the individual `.md` files within the `docs/` directory.
