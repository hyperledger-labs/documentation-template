# Introduction

This repository contains a template that will allow you to quickly bring up a documentation site for Hyperledger _Project_. The following changes need to be done to update the documentation for your project.

# Configuration Updates

## Site Name

Change the `site_name` tag in `mkdocs.yml` to reflect the name of your Hyperledger project. Example:

``` yaml
site_name: Hyperledger Bevel
```

## Project Logo

Replace the file `docs/assets/project-logo.png` with the logo for your project.

!!! warning Logo Filename

    If you use a different name than `project-logo.png`, you will also need to update the `mkdocs.yml` file to replace the `theme.logo` tag to reflect the correct filename. Example:

    ``` yaml
    theme:
      logo: assets/name-of-logo-file.png
    ```

# Documentation Updates

## Introduction

Update the `docs/index.md` file to provide an introduction to the project.
