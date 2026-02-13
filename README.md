# HarmonyOS Development Skill (`harmonyos-dev`)

A specialized skill for the Gemini CLI designed to streamline the development of HarmonyOS applications. This skill provides automated project scaffolding, build verification, and architectural guidance for both Standard ArkTS and Native C++ templates.

## 🚀 Features

- **Project Scaffolding:** Quickly initialize HarmonyOS projects using pre-configured templates.
  - **Standard Template:** Pure ArkTS-based application structure.
  - **Native C++ Template:** Integrated ArkTS and Native API (C/C++) structure.
- **Environment Verification:** Automated checks for required tools (`ohpm`, `hvigorw`, `codelinter`).
- **Build & Dependency Management:** Integrated `ohpm install` and initial build verification.
- **Git Integration:** Automatic repository initialization and initial commit after successful scaffolding.
- **Linting Support:** Enforces quality through `codelinter` integration.
- **Clean Architecture:** Promotes a structured approach with clear separation between Domain, Data, and Presentation layers.
- **API Mapping:** Built-in reference for HarmonyOS versions to API levels.

## 📁 Project Structure

```text
harmonyos-dev/
├── SKILL.md            # Skill definition and instructions for Gemini CLI
├── assets/             # Project templates (Standard and Native C++)
├── scripts/            # Environment check and verification scripts
├── references/         # Detailed technical documentation
│   ├── architecture.md     # Clean Architecture guidelines
│   ├── arkts-strict.md     # ArkTS coding standards
│   ├── troubleshooting.md  # Common issues and solutions
│   └── agency-workflow.md  # Workflow best practices
└── README.md           # This file
```

## 🛠️ Getting Started

### Prerequisites

Ensure you have the HarmonyOS SDK and related command-line tools installed:
- `ohpm` (OpenHarmony Package Manager)
- `hvigorw` (HarmonyOS Build Tool)
- `codelinter`

### Activation

In your Gemini CLI session, activate the skill:

```bash
activate_skill harmonyos-dev
```

### Usage

Once activated, you can use natural language commands to perform tasks:

- **"Initialize a new HarmonyOS project"**: Scaffolds a standard ArkTS project in the current directory.
- **"Create a new Native C++ HarmonyOS app"**: Scaffolds a project with Native API support.
- **"Build and verify the project"**: Checks the environment, installs dependencies, and runs an initial build.

## 🏗️ Architectural Principles

This skill encourages the use of **Clean Architecture** to ensure your HarmonyOS apps remain maintainable and scalable:

1.  **Domain Layer:** Business logic and entities (Pure ArkTS).
2.  **Data Layer:** Data retrieval, storage, and mapping.
3.  **Presentation Layer:** UI state management (ViewModels) and ArkUI components.

## 📊 API Level Reference

| HarmonyOS Version | API Level |
| :--- | :--- |
| 4.0 | 10 |
| 4.1 | 11 |
| 5.0.0 | 12 |
| 5.0.1 | 13 |
| 5.0.2 | 14 |
| 5.0.3 | 15 |
| 5.1.0 | 18 |
| 5.1.1 | 19 |
| 6.0 | 20 |

## 🤝 Contributing

This skill is designed to be extensible. Feel free to contribute by adding new templates or improving the verification scripts and documentation.

---
*Created for use with the Gemini CLI.*
