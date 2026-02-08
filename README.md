# OneBlock

A HyTale plugin built with Java 25 and Gradle.

---

## Prerequisites

- **Java 25 JDK** — [Download](https://www.oracle.com/java/technologies/downloads/)
- **IntelliJ IDEA** — [Download](https://www.jetbrains.com/idea/download/) (Community Edition works)
- **HyTale** — Installed via the official launcher

## Setup

1. Clone the repository and open it in IntelliJ IDEA.
2. Let Gradle sync. The build script will automatically detect your HyTale installation.
3. If HyTale is installed to a non-default location, set `hytale_home` in `gradle.properties`.

## Building

```bash
gradlew.bat build
```

Your plugin JAR will be in `build/libs/OneBlock-0.1.0.jar`.

## Running

The Gradle build generates an IntelliJ IDEA run configuration called **HytaleServer**. Just hit Run to launch the HyTale server with your plugin loaded.

## Project Structure

```
OneBlock/
├── gradle/wrapper/
├── src/main/
│   ├── java/com/hytale/stolen/oneblock/
│   │   └── OneBlock.java
│   └── resources/
│       ├── Common/
│       ├── Server/
│       └── manifest.json
├── build.gradle
├── gradle.properties
├── settings.gradle
├── gradlew
├── gradlew.bat
└── README.md
```

## Configuration

All project settings live in `gradle.properties`:

| Property         | Description                          | Default          |
|------------------|--------------------------------------|------------------|
| `version`        | Plugin version (semver)              | `0.1.0`          |
| `maven_group`    | Java package group                   | `com.hytale.stolen` |
| `java_version`   | Java toolchain version               | `25`             |
| `includes_pack`  | Plugin includes asset pack           | `true`           |
| `patchline`      | HyTale release channel               | `release`        |
| `load_user_mods` | Load mods from user mods folder      | `false`          |
| `hytale_home`    | Custom HyTale install path (optional)| Auto-detected    |

## License

This project is licensed under the [GNU General Public License v3.0](LICENSE).