## Général

- [x] Relire les requirements
- [x] Tests Pads sur bus I2C, I2S, UART et SPI
- [x] Vérifier chaque bloc et voir si tous les signaux sont bien reliés
- [ ] pour les 4 couches, alimentation au centre et signaux extérieur
- [ ] Récupérer les DRC de JLC PCB
- [ ] Rajoutter les labels sur headers
- [ ] Trouver un moyen concret de croisier les informations des différents

## USB

- [x] Résistances pour alimentation 5V
- [x] Protection ESD
- [ ] Attention règles générale de design USB
  - [ ] Impédance 90 ohms
  - [ ] Paire différentielle

## Régulation

- [x] Buck puis LDO

## UWB

- [ ] Attention à garder antenne en dehors du PCB ![](image.png)

## ESP32

- [ ] Attention à garder antenne en dehors du PCB

### Pin Mapping

**I2C (BME288, PIR)**

- SCL -> GPIO16
- SDA -> GPIO15

**I2S (ICS-43434)**

- SCK -> GPIO4
- SD -> GPIO6
- WS -> GPIO5

**SPI (DWM3000)**

- SCLK -> GPIO12
- MISO -> GPIO13
- MOSI -> GPIO11

**UART (LD2410)**

- TX -> GPIO17
- RX -> GPIO18

**LD2410**

- LD2410_INT -> GPIO8

**PIR**

- PIR_INT -> GPIO7 (si présent)

**UWB**

- UWB_CS -> GPIO10
- UWB_INT -> GPIO14 (Pull Down)
- UWB_RST -> GPIO9 (Open Drain GPIO)

**USB**

- D+ -> GIO19
- D- -> GPIO20

**JTAG**

- MTCK -> GPIO39
- MTDO -> GPIO40
- MTDI -> GPIO41
- MTMS -> GPIO42
