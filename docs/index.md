# Introduction

This repository contains a template that will allow you to quickly bring up a documentation site for Hyperledger _PROJECT_. In general, the template provides suggested topics that should be covered in your documentation; however, you can always add/remove content to fit the needs of the project.

The following changes need to be done to update the documentation for your project.

## Configuration Updates

### Site Name

Change the `site_name` tag in `mkdocs.yml` to reflect the name of your Hyperledger project.

!!! example
    ``` yaml
    site_name: Hyperledger Bevel
    ```

### Repo URL

Change the `repo_url` tag in `mkdocs.yml` to reflect the repository of your Hyperledger project.

!!! example
    ``` yaml
    repo_url: https://github.com/hyperledger/_PROJECT_
    ```

### Project Logo

Replace the file `docs/assets/project-logo.png` with the logo for your project.

!!! tip

    White logos with a transparent background works best for the project logo.

!!! warning Logo Filename

    If you use a different name than `project-logo.png`, you will also need to update the `mkdocs.yml` file to replace the `theme.logo` tag to reflect the correct filename. Example:

    !!! example
        ``` yaml
        theme:
          logo: assets/name-of-logo-file.png
        ```

### Project Icon

Replace the file `docs/assets/project-icon.png` with the icon for your project.

!!! tip

    Color or dark icons works best for the project icon.

!!! warning Icon Filename

    If you use a different name than `project-icon.png`, you will also need to update the `mkdocs.yml` file to replace the `theme.favicon` tag to reflect the correct filename. Example:

    !!! example
        ``` yaml
        theme:
          favicon: assets/name-of-icon-file.png
        ```

## Documentation Updates

### Overall

Find and replace the use of `_PROJECT_` with the name of your project in all markdown files and the `mkdocs.yml` file.

### Introduction

Update the `docs/index.md` file to provide an introduction to the project.

### Concepts

The `docs/concepts` directory will contain information about the relevant concepts for your project. Currently there are placeholders for three concepts (`docs/concepts/concepts-[123].md`). You can remove these files and add a separate markdown file for each of the relevant concepts. Then modify the `mkdocs.yml` `nav` section to reflect the concept name and pointer to the concept. The relevant portion of the `mkdocs.yml` file is:

!!! example
    ``` yaml
    nav:
     - Concepts:
       - Concept 1: concepts/concept-1.md
       - Concept 2: concepts/concept-2.md
       - Concept 3: concepts/concept-3.md
    ```

### Getting Started

The files in the Getting Started topic are intended to help people get up and running with your project. 

* Installation (`docs/getting-started/installation.md`) - provide details on how to install the project.
* Running (`docs/getting-started/running.md`) - provide details on how to run the project.

### Tutorials

The `docs/tutorials` directory will contain tutorials that the use can use to learn about your project. There is an introduction page that you can use to describe your tutorials at a high level. In addition, there are placeholders for three tutorials (`docs/tutorials/tutorials-[123].md`). You can remove the placeholder files and add a separate markdown file for each of the relevant tutorials. Then modify the `mkdocs.yml` `nav` section to reflect the tutorial name, and pointer to the tutorial. The relevant portion of the `mkdocs.yml` file is:

!!! example
    ``` yaml
    nav:
     - Tutorials:
       - Introduction: tutorials/index.md
       - Tutorial 1: tutorials/tutorial-1.md
       - Tutorial 2: tutorials/tutorial-2.md
       - Tutorial 3: tutorials/tutorial-3.md
    ```
### Guides

In the Guides section, there are three placeholders:
1. Operations (`docs/guides/operations.md`) - used to guide an operator of your project through critical tasks.
2. Developers (`docs/guides/developers.md`) - used to guide a developer using your project through critical tasks.
3. Upgrading (`docs/guides/upgrading.md`) - used to guide someone through upgrading from one version of your project to another.

!!! note
    The placeholders are not all inclusive. Please add any other reference material that is needed and update the `mkdocs.yml` `nav` section to ensure these references show up on the documentation site.

### References

In the References section, there are three placeholders:

1. Architecture (`docs/references/architecture.md`) - describe the architecture for the project in this file.
2. Commands (`docs/references/commands.md`) - describe the different commands that are available for running the project.
3. Roadmap (`docs/references/roadmap.md`) - describe the roadmap for the project.

!!! note
    The placeholders are not all inclusive. Please add any other reference material that is needed and update the `mkdocs.yml` `nav` section to ensure these references show up on the documentation site.

### Contributing

The files in the Contributing topic are intended to help people who are interested in contributing to your project.

!!! note
    Sample text has been provided in these files. Feel free to modify to fit your project.

* How to Contribute (`docs/contributing/how-to-contribute.md`) - provide details on how to contribute to the project.
* Reporting a Bug (`docs/contributing/reporting-a-bug.md`) - provide details on how to report a bug.
* Requesting a Change (`docs/contributing/requesting-a-change.md`) - provide details on how to request a change. 
* Asking a Question (`docs/contributing/asking-a-question.md`) - provide details on how and where to ask questions.

### FAQs

There is a placeholder (`docs/faqs.md`) for including any frequently asked questions about the project. Please update this document whenever you come across a frequently asked question.

### Glossary

There is a placeholder (`docs/glossary.md`) for capturing terms that are used in the documentation and with relation to the project. Please update the glossary to include relevant terms and definitions.
