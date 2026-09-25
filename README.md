# AndroidLauncher Product v1.0

GitHub-ready Android launcher project using Kotlin, Jetpack Compose, Material 3 and Android 17 (API 37).

## Upload to GitHub

**Important:** upload the *contents of this folder* to the root of your repository, not this folder itself.

The repository root should immediately contain:

- `.github/`
- `app/`
- `gradle/`
- `build.gradle.kts`
- `settings.gradle.kts`
- `gradle.properties`

## GitHub Actions

The included `.github/workflows/android-build.yml`:
1. checks out the repository
2. installs JDK 17
3. installs Android SDK 37
4. installs Gradle 9.6
5. builds debug and release APKs
6. uploads both APKs as an artifact

It deliberately uses the installed Gradle command rather than requiring `gradlew`, so a missing Gradle wrapper cannot cause the earlier failure.

## Local build

Use JDK 17 and Android SDK 37:

`gradle assembleDebug`

`gradle assembleRelease`

## Product shell

Includes real installed-app discovery/launching, app search, adaptive grid, launcher settings shortcuts, modern Compose UI, light/dark theme, and a launcher-friendly manifest.

This is an original Android implementation inspired by premium mobile interaction patterns, not a 1:1 copy of proprietary Apple UI.
