# AndroidLauncher Product v1.0

A modern Android launcher shell built with Kotlin + Jetpack Compose.

## Product features
- Real installed-app discovery through PackageManager
- Real app launching
- App search
- Adaptive app grid
- Live clock/date
- Default Home/launcher role request
- System settings shortcuts
- Edge-to-edge Compose UI
- Material 3 surfaces and original translucent/glass-inspired styling
- Dark/light system theme
- Release minification and resource shrinking
- GitHub Actions build workflow

## Build requirements
- Android Studio Quail 4 (or a compatible newer/older supported Studio)
- JDK 17
- Android SDK API 37
- Gradle 9.6 / Android Gradle Plugin 9.4.0

Build:
`./gradlew assembleDebug`

Release:
`./gradlew assembleRelease`

## Important Android policy note
QUERY_ALL_PACKAGES is declared because a launcher needs to discover launchable apps. Google Play distribution has package-visibility policy requirements; review the current Play policy before publishing.

## Design
The design uses premium mobile patterns—large rounded surfaces, translucency, adaptive spacing and gesture-friendly controls—but is not an exact copy of Apple's proprietary interface.
