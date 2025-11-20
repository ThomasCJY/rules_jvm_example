### Repro Steps
IDE: Android Studio 2025.2.1 Otter
Plugin: Bazel for Android Studio 14432022

Local build pass:
```
bazelisk build //src:lib
```

Result: Go to `rules_jvm_example/src/BUILD` and run enable analysis. Then go to `rules_jvm_example/src/java/com/example/bazel/MainActivity.kt` and verify IDE cannot resolve the external dependency introduced by rules_jvm_external.