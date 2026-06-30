# HoDoKu

A Sudoku generator, solver, analyzer, and trainer written in Java/Swing.

This is a fork of [Hodoku2](https://github.com/wyzelli/Hodoku2) by [wyzelli](https://github.com/wyzelli), which is a fork of [Hodoku](https://github.com/PseudoFish/Hodoku) by [PseudoFish](https://github.com/PseudoFish), which is a fork of [hodoku](https://github.com/yoki123/hodoku) by [yoki123](https://github.com/yoki123), which is a clone of [HoDoKu](https://hodoku.sourceforge.net/en/index.php) originally created by [Bernhard Hobiger (hobiwan)](https://sourceforge.net/u/hobiwan/profile/), who has since passed away.

## Features

- Completely scalable, self-explanatory user interface
- Create random puzzles in five configurable difficulty levels
- Supports over 70 human-style solving techniques (singles, subsets, fish, wings, chains, ALS, and more)
- English and German localization
- Fully configurable via a comprehensive preferences dialog
- Powerful booklet printer and extended print options
- Learning and training modes

## Running

**Windows** — run the provided `HoDoKu.exe` (requires Java 11+ on your PATH).

**All platforms** — run the JAR directly:

```bash
java -Xmx256m -jar HoDoKu-2.3.5.jar
```

## Building

**Prerequisites:** Java 14+ JDK, Maven 3.8+, and one of:

- [Inno Setup 6](https://jrsoftware.org/isinfo.php) — for JDK 18+ builds (recommended)
- [WiX Toolset 3](https://wixtoolset.org/) — for JDK 14–17 builds

```bash
mvn package
```

Outputs:

| File                                | Description                                        |
|-------------------------------------|----------------------------------------------------|
| `target/HoDoKu-2.3.5.jar`           | Runnable JAR — `java -jar` on any platform         |
| `target/HoDoKu.exe`                 | Windows launcher (Launch4J wrapper; requires Java) |
| `target/installer/HoDoKu-2.3.5.exe` | Windows installer — bundles JRE, no Java required  |

## Project structure

```text
src/
  main/
    java/
      generator/   # Puzzle generation
      solver/      # All solving techniques
      sudoku/      # UI, main entry point (sudoku.Main), core data model
    resources/
      help/        # HTML keyboard reference (EN + DE)
      img/         # Icons and images
      intl/        # Localization .properties files (EN + DE)
      templates.dat
forms/             # NetBeans GUI Builder .form files (IDE reference only)
exemplars-1.0.txt  # Example puzzles data
reglib-1.3.txt     # Regression library
templates.dat      # Runtime template data
CHANGELOG.md
```

## Changelog

See [CHANGELOG.md](./CHANGELOG.md) for the full version history.

## Roadmap

See **[TODO.md](./TODO.md)** for the complete and up-to-date list of planned features and tasks.
