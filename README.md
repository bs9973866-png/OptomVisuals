# OptomVisuals

Fabric client mod project for Minecraft 1.21.4 / Java 21.

## GitHub Actions

The workflow in `.github/workflows/build.yml` builds the mod on pushes to `main` and supports manual runs from the **Actions** tab. When a build succeeds, the JAR is uploaded as the `OptomVisuals-JAR` artifact.

## Required source layout

The repository root must contain `build.gradle`, `settings.gradle`, `gradle.properties`, `gradlew`, `gradle/wrapper/gradle-wrapper.jar`, `src/main/java/`, and `src/main/resources/`.

**Current status:** the GitHub Actions workflow is committed, but the project's source tree has not been transferred into this repository yet. The build will remain blocked until those project files are pushed to `main`.

## Build locally

Requires Java 21 and network access for Gradle/Maven dependencies:

```bash
./gradlew build
```

The resulting JAR should be in `build/libs/`.
