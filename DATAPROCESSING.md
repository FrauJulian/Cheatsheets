# Data Processing

## Grundlagen

- **Bit (Binary Digit)**
- Kleinste Informationseinheit
- Werte: `0` oder `1`
- **Byte**
- 1 Byte = 8 Bit
- Kleinste adressierbare Speichereinheit

## Binärpräfixe und Dezimalpräfixe

Binärpräfixe und Dezimalpräfixe sind zwei verschiedene Systeme zur Angabe von Datenmengen:

- **Binärpräfixe** (IEC-Standard - International Electrotechnical Commission): Verwenden eine Basis von `2^10 = 1024` und werden häufig für Speichergrößen verwendet.
- Beispiel: 1 Kibibyte (KiB) = 1024 Byte
- Gängige Präfixe: KiB, MiB, GiB, TiB
- **Dezimalpräfixe** (SI-Standard - Internationales Einheitensystem): Verwenden eine Basis von `10^3 = 1000` und werden oft für Datenübertragungsraten genutzt.
- Beispiel: 1 Kilobyte (KB) = 1000 Byte
- Gängige Präfixe: KB, MB, GB, TB

## Datenmengen und ihre Einheiten

### 2er Potenzen (Binärpräfixe)

| Größe        | Bezeichnung       |
|-------------|------------------|
| 8 Bit       | 1 Byte           |
| 1024 Byte   | 1 Kibibyte (KiB) |
| 1024 KiB    | 1 Mebibyte (MiB) |
| 1024 MiB    | 1 Gibibyte (GiB) |
| 1024 GiB    | 1 Tebibyte (TiB) |
| 1024 TiB    | 1 Pebibyte (PiB) |
| 1024 PiB    | 1 Exbibyte (EiB) |

### 10er Potenzen (Dezimalpräfixe)

| Größe        | Bezeichnung      |
|-------------|-----------------|
| 8 Bit       | 1 Byte          |
| 1000 Byte   | 1 Kilobyte (KB) |
| 1000 KB     | 1 Megabyte (MB) |
| 1000 MB     | 1 Gigabyte (GB) |
| 1000 GB     | 1 Terabyte (TB) |
| 1000 TB     | 1 Petabyte (PB) |
| 1000 PB     | 1 Exabyte (EB)  |

## Datenübertragung

### Maßeinheiten
| Einheit    | Bedeutung                |
|-----------|-------------------------|
| 1 Bit/s   | 1 Bit pro Sekunde        |
| 1 Kbit/s  | 1000 Bit pro Sekunde     |
| 1 Mbit/s  | 1000 Kbit/s              |
| 1 Gbit/s  | 1000 Mbit/s              |

### Netzwerkprotokolle
- **TCP (Transmission Control Protocol)**: Zuverlässige, verbindungsorientierte Übertragung
- **UDP (User Datagram Protocol)**: Schnelle, aber unzuverlässige Übertragung
