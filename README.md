# OFM-OTAUpdateModule

Dieses ist ein Modul dient zum Firmeware Update über das Arduino OTA-Update Protokoll.

## Hardware Unterstützung

|Prozessor | Status     | Anmerkung                  |
|----------|------------|----------------------------|
|RP2040    | ungetestet |                            |
|ESP32     | release    |                            |

Getestete Hardware:
- Adafruit ESP32 Feather V2

## Einbindung in die Anwendung

In main.cpp muss das WLANModule ebenfalls hinzugefügt werden:

```
[...]
#include "OTAUpdateModule.h"
[...]

void setup()
{
    [...]
    openknx.addModule(4, openknxOTAUpdateModule);
    [...]
}
```

## Lizenz

[GNU GPL v3](LICENSE)