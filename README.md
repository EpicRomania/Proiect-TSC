# Proiect-TSC

## Block Diagram

![](https://i.imgur.com/6ZMxgxg.jpeg)



## ESP32-C6

Microcontrolerul central care coordoneaza procesarea datelor si comunicarea cu modulele.

**Pentru conectarea memoriei externe, sunt folositi urmatorii pini:**

- MOSI  
- MISO  
- SCK  
- CS

**Pentru conectarea ceasului real si a senzorilor, se utilizeaza:**

- SDA  
- SCL

Pinii de debug si programare sunt accesibili prin interfata dedicata.

## Memorie Externa

Conectata la ESP32-C6 cu pinii: MOSI, MISO, SCK, CS.

Stocheaza datele e-book si firmware-ul.

## Ceas Real si Module Senzoriale

Dispozitivele de timp real si senzorii se conecteaza pe pinii SDA si SCL.

Aceste module asigura sincronizarea si monitorizarea mediului.

## Aspecte de Design

Componentele sunt asezate astfel incat accesul la conectori sa fie relatic simplu.



## Bill of Materials

| Component                          | Buy Link                                                                                                      | Datasheet Link                                                                                                                 |
|------------------------------------|---------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------|
| ADAFRUIT_LEDCHIP-LED0603           | [Mouser](https://ro.mouser.com/c/optoelectronics/led-lighting/?m=Adafruit)                                    | [Datasheet](https://ro.mouser.com/c/optoelectronics/led-lighting/?m=Adafruit)                                                  |
| SJ                                 | [GrabCAD](https://grabcad.com/library/solder-jumpers-1)                                                       | [GrabCAD](https://grabcad.com/library/solder-jumpers-1)                                                                        |
| ESP32_WROVER_EAGLE-LTSPICE_CC0402  | [Mouser](https://ro.mouser.com/c/passive-components/capacitors/ceramic-capacitors/?q=CC0402)                  | [Datasheet](https://componentsearchengine.com/Datasheets/2/CC0402MRX5R5BB106.pdf)                                              |
| ESP32_WROVER_EAGLE-LTSPICE_RR0402  | [Mouser](https://ro.mouser.com/c/passive-components/resistors/smd-resistors-chip-resistors/?case%20code%20-%20in=0402) | [Datasheet](https://www.yageo.com/upload/media/product/products/datasheet/rchip/PYu-RC_Group_51_RoHS_L_12.pdf)                 |
| RCL_CPOL-EUCT3528                  | [Mouser](https://ro.mouser.com/c/passive-components/antennas/?m=Linx+Technologies&series=RCL)                 | [Mouser](https://ro.mouser.com/c/passive-components/antennas/?m=Linx+Technologies&series=RCL)                                  |
| 112A-TAAR-R03_ATTEND               | [Comet](https://store.comet.srl.ro/Catalogue/Product/43497/)                                                   | [SnapEDA](https://www.snapeda.com/parts/112A-TAAR-R03/Attend/datasheet/)                                                       |
| DMG2305UX-7                        | [DigiKey](https://www.digikey.com/en/products/detail/diodes-incorporated/DMG2305UX-7/4340666)                 | [Datasheet](https://www.diodes.com/assets/Datasheets/DMG2305UX.pdf)                                                            |
| 744043680IND_4828-WE-TPC_WRE       | [Mouser](https://ro.mouser.com/ProductDetail/Wurth-Elektronik/744043680?qs=PGXP4M47uW6VkZq%252BkzjrHA%3D%3D)  | [Datasheet](https://www.we-online.com/components/products/datasheet/744043680.pdf)                                             |
| BME680                             | [Mouser](https://ro.mouser.com/ProductDetail/Bosch-Sensortec/BME688?qs=IS%252B4QmGtzzqQoVDscqwx3A%3D%3D)      | [Datasheet](https://ro.mouser.com/datasheet/2/783/bst_bme688_fl000-2307034.pdf)                                                |
| BUTTON_CUSYOMV1                    | [Panasonic](https://industry.panasonic.com/global/en/products/control/switch/light-touch/number/evqpuj02k)    | [Datasheet](https://industry.panasonic.com/global/en/downloads?tab=catalog&small_g_cd=203&part_no=EVQPUJ02K)                   |
| DS3231SN#                          | [Mouser](https://ro.mouser.com/ProductDetail/Analog-Devices-Maxim-Integrated/DS3231SN?qs=1eQvB6Dk1vhUlr8%2FOrV0Fw%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/609/DS3231-3421123.pdf)                                                          |
| ESP32-C6-WROOM-1-N8                | [Mouser](https://ro.mouser.com/ProductDetail/Espressif-Systems/ESP32-C6-WROOM-1-N8?qs=8Wlm6%252BaMh8ST02Gmwp74cw%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/891/Espressif_ESP32_C6_WROOM_1__Datasheet_V0_1_PRELIMI-3239987.pdf)              |
| ESP32C6_VARISTORCN1812             | [Mouser](https://ro.mouser.com/c/circuit-protection/varistors/?package=1812)                                 | [Mouser](https://ro.mouser.com/c/circuit-protection/varistors/?package=1812)                                                   |
| SD0805S020S1R0                     | [Mouser](https://ro.mouser.com/ProductDetail/KYOCERA-AVX/SD0805S020S1R0?qs=jCA%252BPfw4LHbpkAoSnwrdjw%3D%3D)  | [Datasheet](https://ro.mouser.com/datasheet/2/40/schottky-3165252.pdf)                                                         |
| MCP73831                           | [Mouser](https://ro.mouser.com/ProductDetail/Microchip-Technology/MCP73831T-2ATI-OT?qs=yUQqVecv4qsZbioEUu%252B83g%3D%3D) | [Datasheet](https://ro.mouser.com/datasheet/2/268/MCP73831_Family_Data_Sheet_DS20001984H-3441711.pdf)                          |

