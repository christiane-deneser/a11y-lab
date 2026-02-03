# Messy notes 1.1.1 Non-text Content

## a) Text alternatives for interactive graphics / controls

* Grafiken/Abbildungen als Bedienelemente (Menüs, Logos, Teaserbilder oder Schaltflächen (Link, Button))
* Icon Fonts als Bedienelemente (Menüs, Logos, Teaserbilder oder Schaltflächen (Link, Button))
* SVGs als Bedienelemente (Menüs, Logos, Teaserbilder oder Schaltflächen (Link, Button))

## Hate: Icons with CSS generated content -> Closer look!
## Hate: Icon Fonts
## Hate: SVGs

### Logos

```
<div>
  <a href="/" title="Go to homepage" aria-current="page">
    <svg role="img" aria-label="Logo Component Library" focusable="false" xmlns="http://www.w3.org/2000/svg" width="120" height="120" viewBox="0 0 120 120" role="img" aria-label="Black circle"><circle cx="60" cy="60" r="40" fill="#000" /></svg>
  </a>
</div>
```

```
<div>
  <a href="/" title="Go to homepage" aria-current="page">
    <img src="/assets/img/logo.png" alt="Logo Component Library">
  </a>
</div>
```

### Bei verlinkten Abbildungen gibt es folgende Möglichkeiten

* Generell gilt:
  * Alternativtexte sollen kurz sein.
  * Ausführliche Beschreibungen von Abbildungen sollen nicht im Alternativtext, sondern im Kontext der Abbildung zur Verfügung gestellt werden.

#### 1) Wenn Abbildung nicht dekorativ und Linkziel aus Abb. hervor geht (z.B. Logo. Hier anderes Bspl.: Gegenstand wird in der Textalternative beschrieben

```
<a href="/">
  <img src="/assets/img/example.png" alt="Logo Component Library">
</a>
```

#### 2) Abbildung ist dekorativ und unwichtig: Das Ziel des Links wird über die Textalternative vermittelt

```
<a href="/methodik/taktilographie">
  <img class="image" src="/assets/img/example.png" width="350" height="150" alt="Taktilographie">
</a>
```

#### 3) Beides ist wichtig: Abbildung und Linkziel: Der sinnhafte Inhalt des abgebildeten Gegenstandes und Ziel des Links bzw. die Aktion werden über die Textalternative vermittelt

```
<a href="/">
  <img src="/assets/img/example.png" alt="A painting of a face on a field of flowers - go to detail page.">
</a>
```

### Alternativtexte für redundant verlinkte Abbildungen

* Wenn eine Abbildung und ein danebenstehender Textlink auf dasselbe Ziel verweisen, muss geprüft werden, ob Abbildung und Text in den selben Link eingeschlossen sind.

#### 1) Abbildung und Text innerhalb des selben Links

* Wenn Abbildung und Text innerhalb des selben Links stehen, soll der Alternativtext der Abbildung nicht den Text des Links wiederholen. 
* Je nach Inhalt der Abbildung kann das `alt`-Attribut dann leer bleiben _oder_ den abgebildeten Inhalt beschreiben,
* während der Linktext Zweck oder Ziel des Links beschreibt.

```
<a href="/methodik/taktilographie">
  <img src="/assets/img/example.png" alt="Hand untersucht Brust">
  <span>Taktilographie</span>
</a>
```

#### 2) Abbildung und Text in verschiednenen Links (mit selbem Linkziel)

* Wenn Abbildung und Text zwei unabhängige Links auf dasselbe Ziel sind, dann kann das `alt`-Attribut dagegen _nicht_ leer bleiben.
* Denn gängige Screenreader verlassen sich nicht darauf, dass leere `alt`-Attribute sachgerecht eingesetzt werden,
* sie behandeln bei Bedienelementen leere wie fehlende `alt`-Attribute und lesen den Dateinamen der Grafik / die URL der Zieldatei vor.

```
<a href="/methodik/taktilographie">
  <img src="/assets/img/example.png" alt="Taktilographie">
</a>
<a href="/methodik/taktilographie">
  <span>Taktilographie</span>
</a>
```
