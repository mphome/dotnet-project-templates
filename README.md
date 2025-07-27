# .NET Project Templates

This repository contains custom project templates for the `dotnet` CLI.

## Templates

This repository provides the following templates:

- **MP Console App (`mp-console`)**: A template for creating a console application.
- **mp-console-7.3-template (`mpc73`)**: A template for creating a console application with specific settings for version C# 7.3 and net472.

## Installation

You can install these templates from GitHub or from a local source.

### From GitHub

To install the templates directly from this GitHub repository, run the following command:

```bash
dotnet new install https://github.com/mphome/dotnet-project-templates
```

### From Local Source

If you have cloned this repository to your local machine, you can install the templates from your local directory.

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/mphome/dotnet-project-templates.git
    cd dotnet-project-templates
    ```

2.  **Install the templates:**
    You can install all templates at once by pointing to the root folder:
    ```bash
    dotnet new install .
    ```
    Or, you can install a specific template by pointing to its directory:
    ```bash
    # Install mp-console-template
    dotnet new install mp-console-template

    # Install mp-console-7.3-template
    dotnet new install mp-console-7.3-template
    ```

## Usage

Once the templates are installed, you can use them to create new projects using the `dotnet new` command.

### List Installed Templates

To see a list of all installed templates, including the ones from this repository, run:

```bash
dotnet new list
```

### Create a New Project

To create a new project from a template, use the template's short name.

**`mp-console`**

```bash
dotnet new mp-console -o MyNewConsoleApp
```

This will create a new directory named `MyNewConsoleApp` with the project files.

**`mpc73`**

```bash
dotnet new mpc73 -o MyNewConsoleApp73
```

This will create a new directory named `MyNewConsoleApp73` with the project files.

## Uninstallation

To uninstall the templates, you can use the following command, pointing to the source from which you installed them:

```bash
# Uninstall from GitHub
dotnet new uninstall https://github.com/tomasz-prasolek/dotnet-project-templates

# Uninstall from local source
dotnet new uninstall .
```
