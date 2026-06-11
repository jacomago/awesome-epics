# Contributing

Thanks for helping improve **Awesome EPICS**! Contributions are welcome via pull
request. Please follow the guidelines below so the list stays consistent and
passes our automated checks.

## What belongs here

- Tools, modules, libraries, applications, and resources that are **directly
  related to [EPICS](https://epics-controls.org/)**.

## Entry format

Each entry is a single list item:

```markdown
- [Name](https://example.com) - Short description ending with a period.
```

Rules (enforced by [awesome-lint](https://github.com/sindresorhus/awesome-lint)):

- Keep descriptions concise — say *what it is* and *why it's useful*, don't just
  repeat the name.
- Add new entries in the most appropriate existing section. If a project comes
  from a specific facility, note it in parentheses at the end of the
  description, e.g. `... (PSI).` Common facility codes:
  - PSI — Paul Scherrer Institute
  - KIT — Karlsruhe Institute of Technology
  - PCDS — SLAC Photon Controls & Data Systems
  - SLAC — SLAC National Accelerator Laboratory
  - ORNL — Oak Ridge National Laboratory
  - ISIS — ISIS Neutron and Muon Source
  - ESS — European Spallation Source
  - ALS-U — Advanced Light Source Upgrade (LBNL)
  - Diamond — Diamond Light Source
- Mark inactive projects by ending the description with `Archived.`

## Before opening a pull request

Run the linters locally and make sure they pass:

```bash
npx awesome-lint   # awesome-list structure & entry format
npx lychee README.md   # dead-link check
```

If you have [prek](https://github.com/j178/prek) (or pre-commit) installed, the
formatting hooks run automatically on commit:

```bash
prek -a
```
