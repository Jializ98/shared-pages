# shared-pages

Here is a simple flow chart:

## Workflow Graph

```mermaid
flowchart TD
    A([Tidy LOTVS DM]):::done --> B([Taxonomy clean]):::done
    C([Download GBIF snapshot]):::done --> D([Retrieve & clean species occurrences]):::progress
    B --> D
    E([Download CHELSA data]):::done --> F([Get occurrence climate info]):::progress
    D --> F
    F --> G([Niche info]):::progress

    classDef done fill:#90ee90,stroke:#333,stroke-width:2px;
    classDef progress fill:#ffe599,stroke:#333,stroke-width:2px;

    class A,B,C,E done;
    class D,F,G progress;
```

# Example Repo

[![CI](https://github.com/Jializ98/shared-pages/actions/workflows/blank.yml/badge.svg)](https://github.com/Jializ98/shared-pages/actions/workflows/blank.yml)

This repository demonstrates how to use workflow status badges in GitHub Actions.
