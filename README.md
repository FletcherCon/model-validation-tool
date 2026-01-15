# Model Validation Tool Documentation

A comprehensive Revit model auditing solution designed to enforce best practices and maintain model health throughout the project lifecycle.

## 🌐 View Documentation

**[View the live documentation →](https://YOUR_USERNAME.github.io/YOUR_REPO_NAME/)**

> Replace `YOUR_USERNAME` and `YOUR_REPO_NAME` with your actual GitHub username and repository name.

## 📋 Overview

The Model Validation Tool is a pyRevit extension that performs systematic checks across 7 categories:

| Category | Checks | Description |
|----------|--------|-------------|
| Model Performance | 7 | Warnings, file size, in-place families, imported DWG, etc. |
| Project Settings | 4 | Project info, units, starting view, browser organization |
| External Files | 5 | Linked/imported CAD, Revit links, point clouds, images |
| Datum & Location | 6 | Base point, survey point, levels, grids, reference planes |
| Views | 6 | Views not on sheets, templates, schedules, legends |
| Model Elements | 10 | Rooms, areas, design options, groups, worksets, phases |
| Annotative Elements | 7 | Text, dimensions, tags, revision clouds, sheets |

## 🚀 Validation Presets

- **Quick Check** (5 checks) - Fast validation for daily checks
- **Standard Validation** (18 checks) - Balanced coverage for milestone reviews
- **Full Best Practices** (45 checks) - Comprehensive audit

## 🛠️ Installation

1. Install [pyRevit](https://github.com/eirannejad/pyRevit)
2. Copy the extension folder to your pyRevit extensions directory
3. Reload pyRevit

## 📄 License

Internal use - Digital Engineering Services

---

*Documentation built for the BIM Team*
