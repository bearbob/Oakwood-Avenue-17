<!-- PROJECT LOGO -->
<p align="center">
  <a href="https://github.com/bearbob/Oakwood-Avenue-17">
    <img src="img/repo-cover.jpg" alt="Logo" width="85" height="85">
  </a>

  <h3 align="center">Oakwood Avenue 17</h3>

  <p align="center">
    A german adventure where you choose what comes next!
    <br />
    <a href="https://github.com/bearbob/Oakwood-Avenue-17/wiki"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/bearbob/Oakwood-Avenue-17/issues/new">Report Bug</a>
    ·
    <a href="https://github.com/bearbob/Oakwood-Avenue-17/issues">Request Feature</a>
  </p>
</p>
# COYA Latex Template

Dieses Template soll einen einfachen Weg zeigen, um eigene Abenteuer im Choose-Your-Own-Adventure-Stil zu entwerfen - ohne zu viel Zeit mit dem Setup zu verschwenden.
Mit Hilfe einfacher Definitionen in LaTeX und dem großartigen Template [rpgtex/DND-5e-LaTeX-Template](https://github.com/rpgtex/DND-5e-LaTeX-Template) wird ein kurzes Abenteuer beschrieben.

## Hilfsdefinitionen

### \block{<Name_des_Markers>}{<Überschift>}

Beginnt einen neuen Textblock und generiert eine Referenznummer, die im Text aufgerufen werden kann.
Beispiel: ```\block{theIntersectionRoomFromDungeon}{Ich habe die Wahl}```

### \goto{<Name_des_Markers>}

Erzeugt eine neue Referenz auf einen Textblock, der mit `\block{..}{..}` erzeugt wurde.
Im Text wird die Nummer des referenzierten Blocks ausgegeben.

### \getItem{<Name_des_Markers>}

Erzeugt eine neue Referenz auf eine Gegenstandsbeschreibung, die mit `\inventory{..}` erzeugt wurde.
Im Text wird der Buchstabe 'G' und die Nummer des referenzierten Gegenstands ausgegeben, z.B. `G16`.

### \inventory{<Name_des_Markers>}

Erzeugt eine neuen Zielreferenz für eine Gegenstandsbeschreibung.

### \setEvent{<Name_des_Markers>}

Erzeugt eine neuen Zielreferenz für eine Ereignisbeschreibung.

### \getEvent{<Name_des_Markers>}

Erzeugt eine neue Referenz auf eine Ereignisbeschreibung, die mit `\setEvent{..}` erzeugt wurde.
Im Text wird der Buchstabe 'E' und die Nummer des referenzierten Gegenstands ausgegeben, z.B. `E4`.
