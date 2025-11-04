# DigitClassifer

Android + Kotlin 기반 MNIST 숫자 분류기 프로젝트

---

## 프로젝트 소개

- **AndroidX** 기반
- **TensorFlow Lite** 사용
- **AndroidDraw** 라이브러리 활용 (JitPack)
- **ViewBinding** 사용
- 최소 SDK 24, Target SDK 36

---

## 🛠 환경 세팅

### 1. Gradle 저장소 설정

`settings.gradle.kts`:

```kotlin
pluginManagement {
    repositories {
        google()
        mavenCentral()
        gradlePluginPortal()
        maven { url = uri("https://jitpack.io") }
    }
}

dependencyResolutionManagement {
    repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
    repositories {
        google()
        mavenCentral()
        maven { url = uri("https://jitpack.io") }
    }
}

rootProject.name = "DigitClassifer"
include(":app")
