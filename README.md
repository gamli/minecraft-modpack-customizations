# Anpassungen für Minecraft Modpacks

Dieses Repository enthält Anpassungen für verschiedene Minecraft Modpacks, die auf unserem ZAP-Server laufen. Die Idee
ist, dass man den Ordner eines bestimmten Modpacks, z.B. `All the Mods 6 - To the Sky - ATM6sky - Skyblock`, einfach
direkt über den Ordner des lokal installierten Modpacks,
z.B. `C:\Users\mad\Documents\Curse\Minecraft\Instances\All the Mods 6 - To the Sky - ATM6sky - Skyblock`, wenn man das
Pack mit Curse installiert hat, kopieren kann. Das gleiche gilt z.B. nach einer Neuinstallation des ZAP-Servers. Der
Ordner enthält etwa zusätzliche Mods oder überschriebene Config-Dateien.

## All the Mods 6 - To the Sky

### Zusätzliche Mods

<dl>
   <dt>Chunk Loaders</dt>
   <dd>
      ist ein Mod, der Chunkloader in Form von Blöcken bereitstellt. Sie nennen sich, oh Wunder, (Single|Basic|Advanced|Ultimate) Chunk Loader.
      <a href="https://www.curseforge.com/minecraft/mc-mods/chunk-loaders">Projektseite</a>
   </dd>
</dl>

# Troubleshooting

## Ich sitze an einer Position fest oder habe Probleme beim Login

Im Notfall können die, in der Welt gespeicherten, Daten direkt editiert werden.
Im Hauptverzeichnis des Modpacks befindet sich die Welt im Ordner `world` und in
`world\playerdata\` findet man die Spielerdaten. Für jeden Spieler gibt es eine
`<Spieler-UUID>.dat`-Datei, in der auch die aktuelle Position und Dimension des
Spielers gespeichert ist. Das Format der Datei ist das, von Minecraft verwendete,
[NBT-Format](https://minecraft.fandom.com/wiki/NBT_format). Am besten editiert man
sie mit [NBTExplorer](https://github.com/jaquadro/NBTExplorer/releases). Man ändert
nun die Tags `Dimension` (z.B. minecraft:overworld) und `Pos` (z.B. 0, 64, 0) auf die
Werte, die man haben will.
