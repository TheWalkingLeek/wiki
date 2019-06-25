# Varianten:

## File-level:

### load

Liest und parst ein file in deinen Code.

### require

Ähnlich wie load, speichert aber den Code in die Memory. Dadurch werden Änderungen am required File während der Laufzeit nicht berücksichtigt. Standardwahl zwischen require und load.

## Language-level:

### include 

Importiert Code in das neue File. Dabei werden alle Methoden als Instanzmethoden importiert.

### extend

Ähnlich wie include, importiert die Methoden aber als Klassenmethoden.