# OptomVisuals

Fabric client mod source project for Minecraft 1.21.4 / Java 21.

## Build with GitHub Actions

The workflow at [Build OptomVisuals](.github/workflows/build.yml) runs on pushes to `main` and can also be started manually from the **Actions** tab. On success, it uploads `build/libs/*.jar` as an artifact named `OptomVisuals-JAR`.

## Current repository status

The build workflow has been committed and validated by GitHub Actions, but the actual Java source tree has **not** been uploaded yet. The latest workflow run fails at the source-file check because this repository does not currently contain `build.gradle`, `gradlew`, and `src/main/java/`.

The prepared source archive is organized under an `OptomVisuals/` directory. The workflow supports either that nested layout or files placed directly at the repository root, once those files are transferred.

## Build locally

After the source tree is present, use Java 21 and run:

```bash
./gradlew build
```

(or run `./gradlew build` from the nested `OptomVisuals/` folder). The built JAR should be in `build/libs/`.
