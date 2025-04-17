# CyberDeck on Orange Pi 5 Ultra

![CyberDeck](/image/1.jpg)

## Part list

1. Orange Pi 5 Ultra
2. SURENOO SUR10801920D055A 5.5" DSI Display Orange Pi
3. Li-Ion battery 21700 LiitoKala 5000mah
4. DC/DC Step Down converter XL4016
5. Mini keyboard Rii 518BT
6. INA226 Volt-ampere module
7. Power supply 5.1V 5A Official for Orange Pi
8. Brass Fused Studs M2.5 different sizes
9. Copper radiator
10. TZT 2S 20A BMS balancing board
11. 2S Charge module for Li-ion 8.4V
12. SMD Resistor 0.01 Om
13. 35mm Colling fan

`TODO: add url links`

## 3D printing

All 3D models are at an early stage of development, still need to be adjusted in size!

The model for printing consists of 3 parts: the main body, the battery pack and the back cover.

`TODO: Add 3D models to the repository`

## Soldering of parts

The connection diagram is presented in a separate [repository.](https://github.com/DrHo1y/ina226-battery-driver)

## LLM local launch

To use LLM localy, I prepared tools for myself and posted them in a separate [repository.](https://github.com/DrHo1y/rkllm-gradio-server)

## Install OS

Use my [Debian 12 6.1.x LXCF build](https://github.com/DrHo1y/orangepi-build/releases/tag/v1.0.0), I added the latest version of the driver for the NPU and added support for SURENOO SUR10801920D055A 5.5" DSI Display and INA226 battery driver.

To record the system, use the standard instructions from the manufacturer.

To enable the Display you need to add an overlay `Orangepi-5-Plus-LCD`

To flip an image use the command:

```bash
sudo set_lcd_rotate.sh left
```

To calibrate the touch screen, replace the file:

`TODO: Find the exact location of the file`