      # spendwise1 — Agent Guide

      This project lives inside **Derle**, an on-device mobile IDE. Your terminal, build tools,
      and this project all run inside a **proot Ubuntu Linux** environment on an Android device
      (no root required). Standard Linux tooling is available — `bash`, `git`, `apt`, plus any
      toolchains the user installed from Derle's **Components / SDKs** screen.

      Detected project type: **Flutter**.

      ## Running this project
      The **Run / Build** button builds and installs this app through Derle's built-in build pipeline (it injects the right toolchain env — JAVA_HOME / ANDROID_HOME / Flutter — which a plain shell does NOT have). **Do not** add a `.derle/run.sh` to change the run: customize the build through the standard build files instead (`build.gradle` / `build.gradle.kts` / `pubspec.yaml`, `AndroidManifest.xml`).

      - This project is **not** run via a shell script. Edit the standard build files to
customize it; the app's build pipeline handles toolchain env and installation.

      ## Environment notes
      - Installed toolchains live under `/home/root/` and expose their binaries on `PATH` via
        `/usr/local/bin`. Once installed, compilers (`gcc`, `g++`, `clang`), `node`/`npm`, and
        Python (as `python3.x`) are directly runnable.
      - A few SDKs (JDK, Flutter, Android SDK) are wired into their language's build flow rather
        than the global `PATH`. Prefer the project's build tool (the `gradlew`, `flutter`, or
        `mvnw` wrapper) so the right toolchain and env vars are used.
      - C/C++ builds output to `build/`. Keep generated artifacts there.
      - Install more dependencies with the environment's package managers (`apt`, `pip`, `npm`)
        or from Derle's Components screen.
      - Long-running commands (dev servers, builds) survive backgrounding — Derle keeps the
        shell alive with a foreground service.

      ## Conventions
      - Don't change the build-system flavor (CMake ↔ Makefile, Gradle, Vite, …) unless asked.
      - Keep edits minimal and match the surrounding code style.
