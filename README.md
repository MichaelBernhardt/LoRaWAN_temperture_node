# LoRaWAN_temperture_node
A basic LoRaWAN temperture node. Based on the Madunio LoRa Radio v2.0

A basic Arduino sketch for the the Maduino LoRa Radion v2.0 to post temperature and humidity from a DHT11 sensor to The Things Network

The Maduino LoRa Radio v2.0 is based on the ATmega328 + RFM95 868MHz

The base of this Sketch is from this excellent tutorial - https://www.mobilefish.com/developer/lorawan/lorawan_quickguide_build_lora_node_rfm95_arduino_uno.html with support added for the DHT11 sensor.

The pinout for the RFM95 on the Maduino is as follows:

```
const lmic_pinmap lmic_pins = {
    .nss = 10,
    .rxtx = LMIC_UNUSED_PIN,
    .rst = LMIC_UNUSED_PIN, // hardwired to AtMega RESET
    .dio = {4, 5, 7},
};
```
