# Open EEPROM Programmer

Este projeto é um sistema para programar memórias EPROM, EEPROM e Flash. Foi projetada para aceitar memórias de 2KBytes (16KBits) a 1MByte (8MBits).

### Diferença entre memórias de mesmo tipo

Tomando como exemplo as memórias EPROM, vamos comparar a pinagem de alguns modelos.

| 27C512 | 27C256 | 27C128 | 27C64 | 27C32 | 27C16 | DIP | 27C16 | 27C32 | 27C64 | 27C128 | 27C256 | 27C512 |
| :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: | :---: |
| A15 | VPP | VPP | VPP |  -  |  -  | | -   | -   | 5V  | 5V  | 5V  | 5V  |
| A12 | A12 | A12 | A12 |  -  |  -  | | -   | -   | PGM | PGM | A14 | A14 |
|  A7 |  A7 |  A7 |  A7 |  A7 |  A7 | | 5V  | 5V  | NC  | A13 | A13 | A13 |
|  A6 |  A6 |  A6 |  A6 |  A6 |  A6 | | A8  | A8  | A8  | A8  | A8  | A8  |
|  A5 |  A5 |  A5 |  A5 |  A5 |  A5 | | A9  | A9  | A9  | A9  | A9  | A9  |
|  A4 |  A4 |  A4 |  A4 |  A4 |  A4 | | VPP | A11 | A11 | A11 | A11 | A11 |
|  A3 |  A3 |  A3 |  A3 |  A3 |  A3 | | OE  | OE/VPP | OE | OE | OE | OE/VPP |
|  A2 |  A2 |  A2 |  A2 |  A2 |  A2 | | A10 | A10 | A10 | A10 | A10 | A10 |
|  A1 |  A1 |  A1 |  A1 |  A1 |  A1 | | CE/PGM | CE/PGM | CE | CE | CE/PGM | CE/PGM |
|  A0 |  A0 |  A0 |  A0 |  A0 |  A0 | | D7 | D7 | D7 | D7 | D7 | D7 |
|  D0 |  D0 |  D0 |  D0 |  D0 |  D0 | | D6 | D6 | D6 | D6 | D6 | D6 |
|  D1 |  D1 |  D1 |  D1 |  D1 |  D1 | | D5 | D5 | D5 | D5 | D5 | D5 |
|  D2 |  D2 |  D2 |  D2 |  D2 |  D2 | | D4 | D4 | D4 | D4 | D4 | D4 |
| GND | GND | GND | GND | GND | GND | | D3 | D3 | D3 | D3 | D3 | D3 |

