# Noritake GU7000 Vacuum Fluorescent Display (VFD) Library

[![Check Markdown Links](https://github.com/Andy4495/Noritake-GU7000/actions/workflows/CheckMarkdownLinks.yml/badge.svg)](https://github.com/Andy4495/Noritake-GU7000/actions/workflows/CheckMarkdownLinks.yml)

Noritake provides Arduino libraries for their displays; however, their [Terms of Use][3] do not allow re-publishing their Arduino libraries.

To download and install the library, follow the [instructions][1] on Noritake's website.

I have been using the GU7000 library with the GU144x16D-7053B display. Libraries for other Noritake displays are available at the above link.

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

+ Noritake GU7000 [library][1]
+ Noritake [Terms of Use][3]
+ Noritake GU144X16D-7053B [simplified datasheet][4]
+ Noritake Model GU144x16D-7053B Vacuum Fluorescent Display [full datasheet][2] (registration required)
+ GU-7000 Series [Application Note][5]

[1]: https://www.noritake-elec.com/support/design-resources/support-guide/arduino-code-library-quick-start-guide
[2]: https://www.noritake-elec.com/user/datasheet?SCID=185&VFDID=152&PSID=5908e690167775b2f6241569268c741e&FMTP=2
[3]: https://www.noritake-elec.com/about/terms-of-use
[4]: https://www.noritake-elec.com/user/download?id=gu144x16d-7053b&category=21
[5]: https://www.noritake-elec.com/support/design-resources/user/download?category=2&id=a-apn200_e21
[200]: https://github.com/Andy4495/Noritake-GU7000
