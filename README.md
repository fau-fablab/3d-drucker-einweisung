3D-Drucker Einweisung
=====================

Einweisung des [FAU FabLab](https://fablab.fau.de) in die [3D-Drucker](https://fablab.fau.de/tool/3d-drucker/) Bambu Lab P1S und X1 Carbon (FDM).

Inhalt
------

- Regeln und Sicherheit, Betriebsanweisung (Aushang am Drucker)
- 3D-Modell vorbereiten: Dateiformate, Bauraum, Druckbarkeit (Überhänge, Brücken, Stützen)
- Material und AMS: PLA, PETG, ASA im Vergleich, Filamentwechsel
- Bambu Studio: Werkzeugleiste, wichtigste Einstellungen, Druck starten per MicroSD oder Netzwerk
- Druck beobachten und abbrechen, Nachbearbeitung, Wiegen und Bezahlen, Mehrfarbendrucke
- Infos für Betreuer: Düse, AMS, typische Fehler, Wartungsintervalle

Download
--------

Die neueste Version aus [GitHub](https://github.com/fau-fablab/3d-drucker-einweisung) ist als PDF abrufbar:

- [Einweisung](https://brain.fablab.fau.de/build/3d-drucker-einweisung/Einweisung_3D-Drucker.pdf)
- [Einweisungsliste](https://brain.fablab.fau.de/build/3d-drucker-einweisung/Einweisungsliste_3D-Drucker.pdf)
- [Betriebsanweisung](https://brain.fablab.fau.de/build/3d-drucker-einweisung/Betriebsanweisung_3D-Drucker.pdf) (Aushang am Drucker)

Außerdem baut eine GitHub Action die PDFs bei jedem Push. Auf dem Hauptbranch entsteht dabei ein
[Release](https://github.com/fau-fablab/3d-drucker-einweisung/releases) mit Datums-Version (`vJJJJ.MM.TT`) und den PDFs.

Auschecken und bauen
--------------------

```bash
git clone --recursive git@github.com:fau-fablab/3d-drucker-einweisung.git
cd 3d-drucker-einweisung
make
```

Die PDFs landen in `output/`. Layout, Kopf- und Fußzeile und das Logo des FAU FabLab (mit
FAU-Schriftzug) kommen aus dem Untermodul [fablab-document](https://github.com/fau-fablab/fablab-document),
das Logo wiederum aus dessen Untermodul [logo](https://github.com/fau-fablab/logo). Bei einem bestehenden
Klon die Untermodule mit `git submodule update --init --recursive` laden.

Technische Details zum Buildserver: [fau-fablab/buildserver](https://github.com/fau-fablab/buildserver)

[![Build Status](https://brain.fablab.fau.de/build/3d-drucker-einweisung/status.svg)](https://brain.fablab.fau.de/build/3d-drucker-einweisung/)
[![TODOs](https://brain.fablab.fau.de/build/3d-drucker-einweisung/status-todos.svg)](https://brain.fablab.fau.de/build/3d-drucker-einweisung/)
[![PDF bauen](https://github.com/fau-fablab/3d-drucker-einweisung/actions/workflows/pdf.yml/badge.svg)](https://github.com/fau-fablab/3d-drucker-einweisung/actions/workflows/pdf.yml)

Lizenz
------

[![Lizenz: CC BY-SA 3.0](https://licensebuttons.net/l/by-sa/3.0/de/88x31.png)</br>CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)
