# Classical MP3Tag Templates

A comprehensive collection of classical music work templates for MP3Tag to ensure consistent and properly formatted tags across your classical music library.

## Overview

This repository contains template files organized by composer and work type, designed to be used with MP3Tag to create standardized classical music tags. The templates follow a strict formatting pattern to ensure uniformity in your classical music collection.

## Considerations

These templates are designed to balance informativeness with brevity. In developing this system, several considerations guided the design:

- **Readability**: Tags should be easy to read at a glance on music players with limited display space
- **Consistency**: All works follow the same pattern to ensure a uniform collection
- **Simplicity**: Removing unnecessary punctuation (dots, commas) improves readability without losing meaning
- **Catalog Numbers**: For simplicity, selected catalog numbers are included based on my own familiarity (e.g., BWV for Bach, K for Mozart) while others (such as Hoboken numbers for Haydn) are omitted
- **Movement Names**: To keep tags concise, only the primary tempo marking is retained for movements with multiple tempo indications

These design choices aim to create tags that look clean in music players while still providing all essential information needed to identify works and movements.

## Format Guidelines

All templates follow these formatting rules:

- Composer name formatted as "last name, first name"
- Flats represented as "b" (e.g., "Bb" for B-flat)
- Sharps represented as "#" (e.g., "C#" for C-sharp)
- No periods/dots anywhere (e.g., "No 1" instead of "No. 1", "Op 10" instead of "Op. 10")
- No commas except in composer names
- Nicknames in single quotes (e.g., 'Moonlight', 'Pastoral')
- For movements with multiple tempo indications, only the first is kept (e.g., "Adagio" instead of "Adagio - Allegro")

## Usage Instructions

### Transform these files into tags
Convert -> Text File - Tag ...
%composer% | %WORK% - %movement%/%movementtotal% %movementname%

### Transform generated tags to nice file names
(maybe run Assign Track Numbers before continuing)
Convert -> Tag - Filename
%track% %work% - %movement% %movementname%

## Repository Structure

The repository is organized hierarchically by composer and work type:

```
/Bach
  /Brandenburg Concertos
  /Keyboard Concertos
/Beethoven
  /PianoConcertos
  /Sonatas
  /Symphonies
/Brahms
  /PianoConcertos
  /Symphonies
...
```

## Example

Template line:
```
Beethoven, Ludwig van | Piano Sonata No 14 in C# minor Op 27 No 2 'Moonlight' - 1/3 Adagio sostenuto
```

Will generate tags:
- Composer: Beethoven, Ludwig van
- Work: Piano Sonata No 14 in C# minor Op 27 No 2 'Moonlight'
- Movement: 1
- Movement Total: 3
- Movement Name: Adagio sostenuto

## Contributing

Feel free to contribute additional templates by submitting a pull request. Please follow the formatting guidelines above to maintain consistency.
