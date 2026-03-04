# Апогей БК 01/Apogee BK 01
Information about the Soviet Apogee BK 01 computer, an implementation of the Радио 86РК/Radio 86RK design.

## [New Power Supply](/Apogee-BK_01_Power)
As the Apogee uses the 8080 it requries a tri-voltage power supply, ±5VDC and +12VDC, via a 7-pin DIN.  This is my simple implementation of a replacement using a single +12VDC power source, generating the ±5V via two switching regulators.<br>

- Pin 1 = +5V regulated
- Pin 2 = +5V regulated
- Pin 3 = +12V regulated
- Pin 4 = -5V unregulated
- Pin 5 = ground (общий)
- Pin 6 = ground (общий)
- Pin 7 = fault (авария)

The fault/авария signal on the motherboard monitors the +5V rail relative to the -5V rail.  If the +5V rail drifts too far out of range (over/undervoltage) then it will signal the power supply to shut off the linear regulators (КР142ЕН1Б, similar to Western UA723).

## [Schematics](/Schematics)
High quality scans of the original schematics.
