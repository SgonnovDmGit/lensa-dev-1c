<p align="center">
  <a href="../../releases/latest"><img src="https://img.shields.io/github/v/release/SgonnovDmGit/lensa-dev-1c?label=Releases&color=0fa97a" alt="Latest release"></a>
  <img src="https://img.shields.io/badge/Windows-10%20and%2011%20x64-555" alt="Windows 10 and 11 x64">
  <img src="https://img.shields.io/badge/1C:Configurator-8.3%20and%208.5-555" alt="1C:Configurator 8.3 and 8.5">
</p>

# LenSa Dev 1C

A Windows app in which an AI model works as an **operator of the 1C Configurator**: it sees open
windows, reads modules, edits code and checks it with the platform's own module check. Not by
copy-pasting through a chat, but by itself, in your Configurator.

[Русская версия](README.md)

## What it does

- **Reads and edits code in the open module.** A module of thousands of lines is read by procedures
  and regions, edited precisely, and the changes are marked.
- **Checks a module with the platform.** Runs the standard module check, reads the Messages panel and
  fixes the error it found. It reports success only when the platform confirms it.
- **Finds configuration objects.** "What attributes does the Контрагенты catalog have? Open its object
  module": the model finds the object, lists the attributes and opens the module.
- **Sandbox with a code editor.** 1C highlighting, region folding, a module from disk or EDT, without
  a running Configurator. Finished code moves to the Configurator window with one button.
- **Task board.** The model plans work on the board, you edit the plan by hand, and it survives a
  restart.
- **You see what the work costs.** Metrics of every turn and dialog spending per model.

## Requirements

| | |
|---|---|
| System | Windows 10 or 11, x64 |
| 1C | 1C:Enterprise 8.3 or 8.5 Configurator, needed for working with a configuration; the sandbox works without it |
| Network | Required: models are connected through the Lensa service |

## Getting started

1. Download the ZIP from [Releases](../../releases/latest) and unpack it. Inside is a single
   `LenSaDev1C.exe`: nothing to install, the editor engine is included.
2. Run `LenSaDev1C.exe` and enter your Lensa service access key. Keys are issued in your account at
   [digitalmechanics.dev](https://digitalmechanics.dev).
3. Open the Configurator with your database, the app finds it by itself.

Make a copy before the first run on a production database: the model can edit code.

## Documentation

- [What's new](docs/WhatsNew.en.md): changes by version
- [Planned](docs/Planned.en.md): what we work on next
- [Guide](docs/Справка.md): user guide (Russian), it is also built into the app, the "?" button

## License

The app is distributed free of charge; the Lensa service is connected separately. This is **not open
source**: the rights to the product belong to the right holder. Terms: [LICENSE.md](LICENSE.md).

## Feedback

Send questions, bugs and wishes to [Issues](../../issues).
