# Devcontainers for Coder

A collection of ready-to-use development container configurations for [Coder](https://coder.com), optimized for various programming languages and frameworks.

## Available Devcontainers

This repository provides devcontainer configurations for the following languages and environments:

### Language-Specific Containers

- **[Python](./python/)** - Python 3.11 with Pylance, Black formatter, and Jupyter support
- **[Node.js](./node/)** - Node.js 20 LTS with TypeScript, ESLint, and Prettier
- **[Go](./go/)** - Go 1.21 with full language server support
- **[Rust](./rust/)** - Latest stable Rust with rust-analyzer and LLDB debugger
- **[Java](./java/)** - Java 17 LTS with Maven and Gradle
- **[.NET](./dotnet/)** - .NET 8.0 SDK with C# Dev Kit
- **[Universal](./universal/)** - Multi-language environment with Python, Node.js, Go, Ruby, PHP, and Docker-in-Docker

## Usage with Coder

### Using a Devcontainer in Coder

1. In your Coder workspace, clone or reference this repository
2. Copy the desired devcontainer configuration to your project's `.devcontainer` directory:
   ```bash
   cp -r /path/to/Devcontainers/python/.devcontainer.json .devcontainer/devcontainer.json
   ```
3. Rebuild your workspace to apply the devcontainer configuration

### Direct Template Usage

You can also directly reference these devcontainers in your Coder template or workspace configuration by pointing to the specific devcontainer directory in this repository.

## Features

All devcontainers include:

- **Git** - Latest version with configuration support
- **Zsh with Oh My Zsh** - Enhanced shell experience
- **VS Code Extensions** - Language-specific extensions pre-installed
- **Post-creation Commands** - Automatic setup and validation

## Customization

Each devcontainer can be customized by editing the `.devcontainer.json` file:

- Add more VS Code extensions
- Modify container features
- Change post-creation commands
- Adjust user settings

## Directory Structure

```
.
├── python/           # Python devcontainer
├── node/             # Node.js/TypeScript devcontainer
├── go/               # Go devcontainer
├── rust/             # Rust devcontainer
├── java/             # Java devcontainer
├── dotnet/           # .NET devcontainer
└── universal/        # Universal multi-language devcontainer
```

Each directory contains:
- `.devcontainer.json` - The devcontainer configuration
- `README.md` - Specific documentation for that container

## Contributing

Feel free to open issues or pull requests to add more devcontainer configurations or improve existing ones.

## License

This repository is provided as-is for use with Coder and other devcontainer-compatible platforms.
