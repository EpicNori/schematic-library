# Schematic Library

Die Bibliothek hat zwei Hauptbereiche:

- `farms/<farmtyp>/` enthält alles, womit Ressourcen, Mobs oder XP erzeugt
  werden. Die verwendete Technik oder Redstone-Komplexität spielt dabei keine
  Rolle.
- `builds/<bauwerk>/` enthält Bauwerke und eigenständige technische Module.

Alle Ordner- und Dateinamen verwenden englisches `snake_case`.

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
farms/
  bamboo/                       Bambusfarmen
  bonemeal/                     Knochenmehlfarmen
  cactus/                       Kaktusfarmen
  cobblestone/                  Bruchsteinfarmen
  concrete/                     Betonfabriken
  creeper/                      Creeperfarmen
  dirt/                         Erdfarmen und Konverter
  honey/                        Honig- und Bienenfarmen
  iron/                         Eisenfarmen
  mob/                          Allgemeine Mobfarmen
  moss/                         Moosfarmen
  obsidian/                     Obsidianfarmen
  potions/                      Automatische Trankbrauer
  raid/                         Raidfarmen
  resin/                        Harzfarmen
  sand/                         Sandfarmen und Sandduper
  snow/                         Schneefarmen
  tree/                         Baumfarmen aller Holzarten
  tripwire_hook/                Stolperhakenfarmen
  wither_rose/                  Witherrosenfarmen
  wool/                         Wollfarmen
  xp/                           XP-Farmen

builds/
  boats/                        Schiffe und Boote
  houses/                       Häuser und Geschäfte
  lobbies/                      Server-Lobbys und Hubs
  redstone/                     Eigenständige Redstone-Module
  storage/                      Lager- und Sortiersysteme
  towers/                       Türme

third_party_licenses/           Lizenztexte importierter Dateien
```

## Drittanbieter-Builds

Importierte Drittanbieter-Dateien bleiben ihren ursprünglichen Urhebern und
Lizenzbedingungen zugeordnet. Quellen, feste Commit-Stände und Nutzungsrechte
sind in [THIRD_PARTY_ATTRIBUTION.md](THIRD_PARTY_ATTRIBUTION.md) dokumentiert.
