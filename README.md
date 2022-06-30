# Noritake GU7000 Vacuum Fluorescent Display (VFD) Library

[![Check Markdown Links](https://github.com/Andy4495/Noritake-GU7000/actions/workflows/CheckMarkdownLinks.yml/badge.svg)](https://github.com/Andy4495/Noritake-GU7000/actions/workflows/CheckMarkdownLinks.yml)

Noritake provides Arduino libraries for their displays; however, their [Terms of Use][3] do not allow re-publishing their Arduino libraries.

To download and install the library, follow the [instructions][1] on Noritake's website.

I have been using the GU7000 library with the GU144x16D-7053B display. Libraries for other Noritake displays are available at the [above link][1].

## Using the GU7000 Module

The GU7000 is a 5V device and requires 5V logic levels (Vcc * 0.8)

I measured supply current of up to 230 mA when the module was powered and most pixels were active, down to 200 mA with a blank screen. The module has a low power mode which draws about 40 mA.

Pin Functions (CN1):

1. VCC
2. SIN
3. GND
4. SBUSY
5. SCK (Synchronous Serial and SPI modes) or NC (Async Serial mode)
6. /RESET
7. SPI /CS (NC for other modes)

## References

- Noritake GU7000 Arduino [library][1]
- Noritake [Terms of Use][3]
- Noritake GU144X16D-7053B [Product Support Page][7], including:
  - Simplified Datasheet
  - Application Note
  - [Full Datasheet][2] (registration required)
  - [Command Description][6]

[1]: https://www.noritake-elec.com/support/design-resources/support-guide/arduino-code-library-quick-start-guide
[2]: https://www.noritake-elec.com/user/datasheet?FMTP=2&PSID=5908e690167775b2f6241569268c741e&VFDID=152&SCID=185
[3]: https://www.noritake-elec.com/about/terms-of-use
[4]: https://www.noritake-elec.com/user/download?id=gu144x16d-7053b&category=21
[5]: https://www.noritake-elec.com/products/user/download?category=2&id=a-apn200_e21
[6]: https://www.noritake-elec.com/support/design-resources/support-guide/gu-7000-command-description
[7]: https://www.noritake-elec.com/products/model?part=GU144X16D-7053B
[200]: https://github.com/Andy4495/Noritake-GU7000
