# shared-pages

Here is a simple flow chart:

## Workflow Graph

```mermaid
flowchart TD
    A([Tidy LOTVS DM]):::done --> B([Taxonomy clean<br>(based on A)]):::done
    C([Download GBIF snapshot]):::done --> D([Retrieve & clean<br>species occurrences<br>(based on B & C)]):::progress
    B --> D
    E([Download CHELSA data]):::done --> F([Get occurrence<br>climate info<br>(based on D & E)]):::progress
    D --> F
    F --> G([Niche info<br>(based on F)]):::progress

    classDef done fill:#90ee90,stroke:#333,stroke-width:2px;
    classDef progress fill:#ffe599,stroke:#333,stroke-width:2px;
```

# Example Repo

[![CI](https://github.com/Jializ98/shared-pages/actions/workflows/blank.yml/badge.svg)](https://github.com/Jializ98/shared-pages/actions/workflows/blank.yml)

This repository demonstrates how to use workflow status badges in GitHub Actions.
