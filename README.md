# Schematic Library

Minecraft-Builds werden nach Kategorie und Thema abgelegt. Alle Ordner- und
Dateinamen verwenden englisches `snake_case`.

## Namensschema

```text
<kategorie>_<thema>[_<variante>]_<groesse>.<format>
```

Beispiele:

- `farm_iron_small.litematic`
- `lobby_medieval_large.schematic`
- `house_dark_oak_prismarine_duplex_small.schem`

Die Dateiendung des ursprünglichen Builds bleibt erhalten. Die Größenklasse
wird aus dem Volumen der in der Datei gespeicherten Bounding Box abgeleitet:

- `small`: weniger als 10.000 Blöcke Volumen
- `medium`: 10.000 bis 99.999 Blöcke Volumen
- `large`: mindestens 100.000 Blöcke Volumen

## Struktur

```text
create/                         Create-Mod-Builds
farms/                          Farmen und technische Builds
lobbies/                        Server-Lobbys und Hubs
medieval/boats/                 Mittelalterliche Schiffe
medieval/buildings/houses/      Mittelalterliche Häuser
medieval/buildings/towers/      Mittelalterliche Türme
```
