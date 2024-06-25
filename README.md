<!--
SPDX-FileCopyrightText: 2024 AFCMS <afcm.contact@gmail.com>
SPDX-License-Identifier: GPL-3.0-or-later
-->

# DevPet Meta

[devpet-repo-meta]: https://github.com/AFCMS/devpet_meta
[devpet-repo-core]: https://github.com/AFCMS/devpet
[devpet-repo-backend]: https://github.com/AFCMS/devpet_backend

## Repositories

| Repository                            | Description                                    |
| ------------------------------------- | ---------------------------------------------- |
| [DevPet Meta][devpet-repo-meta]       | Instructions, 3D models, schemas, explanations |
| [DevPet][devpet-repo-core]            | ESP32 code                                     |
| [DevPet Backend][devpet-repo-backend] | NodeJS serial backend code                     |

## Hardware

### Components

| Name      | Description                          | Link                                                                  |
| --------- | ------------------------------------ | --------------------------------------------------------------------- |
| ESP32     | Microcontroler                       |                                                                       |
| SSD1306   | OLED 128x64 monochrome 0.96" display | [Az-Delivery](https://www.az-delivery.de/fr/products/0-96zolldisplay) |
| Button x3 | 12x12x7.3mm push buttons             | [Amazon FR](https://amzn.eu/d/iSc4HgD)                                |

### 3D Printed Parts

| Description                                                   |
| ------------------------------------------------------------- |
| [STL Files](./hardware/3d)                                    |
| [3MF File (from Bambu Studio)](./hardware/3d/devpet_case.3mf) |
| [Fusion360 Archive](./hardware/3d/devpet_case_v15.f3z)        |
| [Fusion360 Cloud Project](https://a360.co/4bYumfe)            |

The final project have been printed on a [Bambu Lab X1E](https://bambulab.com/en/x1e) using an ABS filament and a 0.4mm nozzle.

### Schematics

[Wokwi Diagram](./hardware/wokwi-diagram.json)

![Wokwi Diagram](./documents/images/wokwi_diagram.png)

## Built with

-   [PlatformIO](https://platformio.org) (embed development toolkit)
-   [image2cpp](https://javl.github.io/image2cpp) (bitmap to C++ array converter)
-   [Octicons](https://primer.style/foundations/icons) (many GitHub icons source)
-   [ASCII Draw](https://github.com/Nokse22/ascii-draw) (backend startup logo)
-   [Marp](https://marp.app) (Markdown presentations)
-   [LibreSprite](https://libresprite.github.io) (the dinosaur sprites)

## Thanks to

-   [@Eladji](https://github.com/eladji) for providing me the Fusion360 models for the base components
-   [@AKArien0](https://github.com/AKArien0) for the [inspiration](https://github.com/AKArien0/arduino-input-handler) for the embed input handler
-   My friend [@Klhmt](https://github.com/Klhmt) for the main dinosaur sprites and animations
