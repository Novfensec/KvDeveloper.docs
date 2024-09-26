---
layout: default
title: Getting Started
commands_active: active
---

# KvDeveloper Commands

KvDeveloper provides several commands to help you manage and create KivyMD projects efficiently. Below is a list of the available commands with their descriptions and usage.

## `create`
Create a new project with the specified template and structure.

### Usage

```bash
kvdeveloper create [OPTIONS] PROJECT_NAME
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
Show the README.md file containing the template info of the project.

### Usage
```bash
kvdeveloper show_readme [DIRECTORY]
```

#### Options and Arguments
`DIRECTORY`: The directory containing the README.md file. Defaults to the current directory `(.)`.

## `list-templates`
List all available templates.

### Usage
```bash
kvdeveloper list_templates
```

## `list-structures`
List all available structures.

### Usage
```bash
kvdeveloper list_structures
```

## `add-screen`
Create screens with specified template and structure.

### Usage

```bash
kvdeveloper add-screen [OPTIONS] NAME_SCREEN...
```

#### Options and Arguments

- `--use-template TEXT`: Name of the template if the specified view exists in it. [default: None]
- `--structure TEXT`: Structure of the project. Defaults to the value of DEFAULT_STRUCTURE which is `none`.
- `NAME_SCREEN`: List containing the name of the screens. _`required`_

### Example

- Create screens with names `TestScreen`, `Test2Screen`, `Test3Screen` following the MVC structure:
```bash
kvdeveloper add-screen TestScreen test2screen test3 --template blank --structure MVC
```

## `config-build-setup`
Generates necessary build files for external build environments (Github/Colab) and linux
systems.

### Usage
```bash
kvdeveloper config-build-setup [OPTIONS] PLATFORM
```

#### Options and Arguments
- `--external TEXT`: External Build Environment. [default: None] _`required`_
- `PLATFORM`: Platform specific to setup build files. [default: None] _`required`_

### Example
- Generate github buildozer workflows for android conversion:
    ```bash
    kvdeveloper config-build-setup android --external github
    ```

    Sample Repository: [Sample-KivyMD-App](https://github.com/Novfensec/SAMPLE-KIVYMD-APP)

- Generate jupyter notebook for colab based android conversion [`Contains commands to import your app folder from your personal drive!`]:
    ```bash
    kvdeveloper config-build-setup android --external colab
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

# FAQs

Have questions? We've compiled a list of [Frequently Asked Questions](faqs.md) to help you troubleshoot common issues and get the most out of KvDeveloper.
