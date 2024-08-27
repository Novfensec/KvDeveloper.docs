---
layout: default
title: Getting Started
---

# KvDeveloper Commands

KvDeveloper provides several commands to help you manage and create KivyMD projects efficiently. Below is a list of the available commands with their descriptions and usage.

## `create`

### Description

Create a new project with the specified template and structure.

### Usage

```bash
kvdeveloper create [OPTIONS] [PROJECT_NAME]
```

#### Options and Arguments

- `--template TEXT`: Template for the project. Defaults to the value of DEFAULT_TEMPLATE which is `blank`.
- `--structure TEXT`: Structure for the project. Defaults to the value of DEFAULT_STRUCTURE which is `none`.
- `PROJECT_NAME`: The name of the project. Defaults to "NewProject".

### Example
```bash
kvdeveloper create my_project --template blank --structure MVC
```

## `show-readme`

### Description
Show the README.md file containing the template info of the project.

### Usage
```bash
kvdeveloper show_readme [DIRECTORY]
```

#### Options and Arguments
`DIRECTORY`: The directory containing the README.md file. Defaults to the current directory `(.)`.

## `list-templates`

### Description
List all available templates.

### Usage
```bash
kvdeveloper list_templates
```

## `list-structures`

### Description
List all available structures.

### Usage
```bash
kvdeveloper list_structures
```

## `help`

- Run the below command for listing all options and commands.
    ```bash
    kvdeveloper --help
    ```

- Get help with any command by running the below command.
    ```bash
    kvdeveloper [COMMANDS] --help
    ```

### Example:
```bash
kvdeveloper create --help
```

This document serves as a reference for all available commands in KvDeveloper. Use these commands to streamline your KivyMD development process.

# FAQ

Have questions? We've compiled a list of [Frequently Asked Questions](faqs.md) to help you troubleshoot common issues and get the most out of KvDeveloper.
