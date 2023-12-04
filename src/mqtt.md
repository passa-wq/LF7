# MQTT

„**M**essage **Q**ueuing **T**elemetry **T**ransport“

* Publish/Subscribe

* Clients können ein „Topic“ abonnieren
  * TCP-Verbindung wird offen gehalten
  * Server kann Clients über bestehende Verbindung über Updates informieren

```bash
mosquitto_sub -h 192.168.88.47 -p 1883 -u fi22 -P geheim -t fi22/buttonGPIO2
mosquitto_pub -h 192.168.88.47 -p 1883 -u fi22 -P geheim -t fi22/buttonGPIO2 -m '1'
```
