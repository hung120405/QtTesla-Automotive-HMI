# IVI Dashboard Demo (Qt/QML)

A **Qt Quick / QML** car-dashboard style UI demo project (instrument cluster + panels) built with C++ integrations.

## Important dependency note (GeneralMagic)
This project imports `GeneralMagic 2.0` in QML (see `main.qml`, `Dashboard.qml`, and settings pages) for **maps/navigation services**.

- `GeneralMagic` is a **third-party SDK** and may require a separate license/subscription depending on your usage.
- To build/run the full navigation/map part, you must install and configure the GeneralMagic SDK according to their documentation.
- If you don’t have access to the SDK, the project may still be useful for **UI/Qt/QML learning**, but QML files importing `GeneralMagic 2.0` can fail to load at runtime.

## Features
- Qt Quick (QML) dashboard UI layout
- Theme switching (light/dark)
- Custom controls (e.g. radial bar)
- Media/music UI module
- Weather module

## Tech stack
- **C++ / Qt**
- Qt Quick / QML
- Qt modules used (from `.pro`): `quick`, `svg`, `multimedia`, `widgets`, `network`, `positioning`, `qml`

## Project structure
- `main.cpp` / `main.qml` / `Dashboard.qml`: app entry + main UI
- `teslasettings.*`: persistent settings (e.g. dark mode)
- `Music/`: music player UI + C++ bridge
- `whether/`: weather module
- `Icons/`: icons and assets
- `qml.qrc`: Qt resource collection

## Build & Run (Qt Creator)
1. Open `Tesla.pro` in **Qt Creator**.
2. Configure a Qt Kit (Qt 5.15+ or Qt 6 recommended).
3. Build and run.



