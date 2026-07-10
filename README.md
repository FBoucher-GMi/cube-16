# SudoCube 1.10.15.6 (MultiPlatform)

SudoCube is a cross-platform .NET MAUI puzzle game inspired by Sudoku, built around a 4x4x4 cube logic format (Cube-16).

This document provides a product-level summary of the app and its capabilities.

Web Site: https://cube-16.ca

## Application Overview

SudoCube focuses on three goals:

- Offer a clear and enjoyable logic puzzle experience.
- Support multiple platforms with a consistent interface.
- Provide flexible personalization (language, theme, and visual style).

The app is designed for everyday play, with integrated guidance and persistent preferences so users can continue where they left off.

## Core Features

- Cube-16 puzzle gameplay with multiple puzzle sources.
- Difficulty-aware hint system.
- Solution reveal option.
- New grid generation flow.
- Persistent game state and user preferences.

## Personalization and UI

- Theme system with a catalog of built-in themes.
- Custom photo background mode (user-selected image).
- Country/language selection driven by configuration.
- Adaptive title bar styling on Windows.
- Android system bar color integration aligned with the active theme.

## Localization and Help

- Localized user interface (French/English and country-dependent options).
- Integrated help page available from inside the app.
- Online/offline help fallback behavior.

## Reliability and Data Handling

- Structured local logging for diagnostics.
- Local persistence for settings and session continuity.
- Defensive handling around file-based personalization flows.
- Mobile crash telemetry support (Android/iOS) when platform files are configured.

## Supported Platforms

- Android (`net10.0-android`)
- Windows (`net10.0-windows10.0.19041.0`)
- iOS (`net10.0-ios`)

## Technology Stack

- .NET 10
- .NET MAUI
- Shared project architecture for common game logic/resources
- JSON-based runtime configuration and theme metadata

## Quick Start (Developers)

From the `SudoCube` root folder:

```powershell
dotnet build .\1.10.15.6MultiPlatform\SudoCube.csproj -f net10.0-windows10.0.19041.0
dotnet run --project .\1.10.15.6MultiPlatform\SudoCube.csproj -c Debug -f net10.0-windows10.0.19041.0
```

## Notes

- This file is intentionally focused on app summary and features.
- It does not include version-to-version change details.

