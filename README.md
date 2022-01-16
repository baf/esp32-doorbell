# esp32-doorbell

A fork of https://github.com/sweharris/esp32-doorbell, with the only difference being support for a username/password on the MQTT server.

You will need to make a file `network_conn.h` with contents similar to

    const char* ssid         = "your-ssid";
    const char* password     = "your-wpa-passwd";
    const char* mqttServer   = "your-MQTT-server";
    const int mqttPort       = 1883;
    const char* mqttUsername = "your-MQTT-username";
    const char* mqttPassword = "your-MQTT-password";

in order to provide details of your network and MQTT server.