# OptomVisuals

A visual-only Fabric client mod fork based on the supplied project (Minecraft 1.21.4 / Java 21).

## Changes in this cleanup
- Renamed the Fabric mod metadata to `optomvisuals` / `OptomVisuals`.
- Disabled registration of the legacy Reform module system.
- Restricted the remaining module registry to visual/render modules. Combat, movement, player automation, and exploit modules are not registered.

## Build
Requires Java 21 and network access for Gradle/Maven dependencies.

Linux/macOS: `./gradlew build`
Windows: `gradlew.bat build`

The resulting mod jar should be in `build/libs/`.

## Not yet implemented
Spotify-synchronized World Lyrics and configurable Hit Sounds (CJ / Pderfvb / UWU / optional moan sound) are not included in this cleanup build. Spotify lyrics require a lyrics source/API and user-authorized Spotify playback integration; lyric availability and synchronization vary by track. These should be implemented and tested separately rather than represented as already working.

## GitHub
Create a repository named `OptomVisuals` under your account and push this project. A GitHub login/token or connected GitHub account is required to publish directly; none was provided for this task.
