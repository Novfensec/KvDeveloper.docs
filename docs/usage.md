---
layout: default
title: Usage
permalink: usage/
---

# Usage

Learn how to effectively use KvDeveloper for your projects.

## Basic Commands

- ### Creating a New Project
    Below command creates a new KivyMD project with a `blank` template and default structure `none`:

    ```bash
    kvdeveloper create my_project
    ```

- ### Including templates
    Create a new KivyMD project using [nav_toolbar](/templates/#nav-toolbar) template:

    ```bash
    kvdeveloper create my_project --template nav_toolbar
    ```

- ### Including structures
    Create a new KivyMD project using [nav_toolbar](/templates/#nav-toolbar) template with MVC architecture:

    ```bash
    kvdeveloper create my_project --template nav_toolbar --structure MVC
    ```