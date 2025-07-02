# Best Practice Lehre 2025: Jupyter Notebooks in der Ingenieurausbildung

## Über diesen Vortrag

Dieser Vortrag und das dazugehörige Repository entstanden aus der praktischen Erfahrung, dass Programmieren im Ingenieurstudium oft als Hürde empfunden wird. Studierende sehen häufig nicht den direkten Bezug zwischen abstrakten Programmierkonzepten und ihren zukünftigen Aufgaben als Ingenieur:innen. 

Hier setzen Jupyter Notebooks an: Sie verbinden Code, Dokumentation und Visualisierungen in einem interaktiven Format, das besonders gut für das Lernen und Verstehen geeignet ist. Der Vortrag zeigt anhand eines konkreten Windenergie-Projekts, wie diese Technologie das Programmierenlernen revolutionieren kann.

## Das Jupyter Notebook: Windenergie-Analyse

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/greenenergylab/bestpractice25/HEAD?urlpath=%2Fdoc%2Ftree%2F%2Fnotebooks%2Fbestpractice25.ipynb)

Das Herzstück dieses Repositories ist ein interaktives Jupyter Notebook, das eine vollständige Windenergie-Analyse durchführt. Es wurde bewusst so gestaltet, dass es sowohl die technischen Möglichkeiten von Notebooks demonstriert als auch ein spannendes Ingenieursproblem löst.

### Was passiert im Notebook?

Das Notebook führt Sie durch eine realistische Windenergie-Studie:

**Datensammlung**: Wir holen uns echte Wetterdaten vom Deutschen Wetterdienst für Münster (NRW) der letzten 30 Tage. Dabei lernen Sie, wie man APIs nutzt und mit echten, "unaufgeräumten" Daten arbeitet.

**Ingenieur-Berechnungen**: Die gemessenen Windgeschwindigkeiten werden mit der Leistungskurve einer realen Windkraftanlage verknüpft. So sehen Sie, wie aus Naturphänomenen elektrische Energie wird.

**Machine Learning**: Mit verschiedenen Algorithmen versuchen wir, die Windenergie-Produktion vorherzusagen. Dabei erkunden wir, welche Faktoren (Windgeschwindigkeit, Temperatur, Luftdruck) am wichtigsten sind.

**Wirtschaftliche Bewertung**: Am Ende bewerten wir, ob sich eine Windkraftanlage an diesem Standort lohnen würde - mit allen Unsicherheiten und Annahmen, die in der echten Ingenieurspraxis auftreten.

### Warum gerade dieses Beispiel?

Windenergie ist ein Thema, das viele Studierende interessiert und das verschiedene Ingenieurdisziplinen verbindet. Gleichzeitig ist es komplex genug, um die Stärken von Jupyter Notebooks zu zeigen: die Möglichkeit, Berechnungen Schritt für Schritt nachzuvollziehen, Zwischenergebnisse zu visualisieren und verschiedene Szenarien durchzuspielen.

## Schnellstart - Notebook ausprobieren

**Am einfachsten**: Klicken Sie auf den Binder-Button oben im Repository. Das Notebook startet direkt im Browser - ohne Installation, ohne Setup.

**Für Fortgeschrittene**: Repository klonen und lokal ausführen (siehe Installationsanleitung unten).

## Was Sie aus dem Notebook mitnehmen

Nach dem Durcharbeiten verstehen Sie:

- **Jupyter Notebooks**: Warum sie das Programmierenlernen erleichtern und wie sie in der Praxis eingesetzt werden
- **Datenverarbeitung**: Vom rohen Datensatz zur aussagekräftigen Analyse
- **Machine Learning**: Grundprinzipien und praktische Anwendung für Ingenieursprobleme  
- **API-Nutzung**: Wie man externe Datenquellen anzapft
- **Projektbewertung**: Technische und wirtschaftliche Faktoren bei Ingenieursentscheidungen

## Technische Details

### Verwendete Tools
- **Python**: Die Basis für alles
- **Pandas & NumPy**: Für Datenmanipulation und Berechnungen
- **Matplotlib**: Für aussagekräftige Diagramme
- **Scikit-learn**: Machine Learning Bibliothek
- **Bright Sky API**: Zugang zu den DWD-Wetterdaten

### Datengrundlage
- **Quelle**: Deutscher Wetterdienst (DWD) via Bright Sky API
- **Standort**: Münster, Nordrhein-Westfalen
- **Zeitraum**: Jeweils die letzten 30 Tage (automatisch aktualisiert)
- **Parameter**: Windgeschwindigkeit, -richtung, Temperatur, Luftdruck

## Lokale Installation

Falls Sie das Notebook auf Ihrem eigenen Rechner ausführen möchten:

```bash
# Repository klonen
git clone https://github.com/greenenergylab/bestpractice25.git
cd bestpractice25

# Python-Pakete installieren
pip install -r requirements.txt

# Jupyter Notebook starten
jupyter notebook bestpractice_demo.ipynb
```

**Systemvoraussetzungen**: Python 3.8 oder neuer

## Typische Ergebnisse

Die Analyse zeigt normalerweise:
- Durchschnittliche Windgeschwindigkeiten von 3-7 m/s in NRW
- Kapazitätsfaktor der Windkraftanlage zwischen 15-25%
- Machine Learning Modelle mit R²-Werten von 0.7-0.9
- Amortisationszeiten von 8-12 Jahren (je nach Annahmen)

*Hinweis: Da echte, aktuelle Wetterdaten verwendet werden, variieren die Ergebnisse je nach Ausführungszeitpunkt.*

## Für wen ist das gedacht?

**Studierende**: Praktisches Beispiel, wie Programmierung in der Ingenieurspraxis aussieht

**Lehrende**: Erprobtes Material für interaktive Lehrveranstaltungen zu Data Science oder erneuerbaren Energien

**Praktikerinnen und Praktiker**: Einstieg in datengetriebene Methoden im Ingenieurswesen

**Neugierige**: Verständlicher Einblick in Windenergie und maschinelles Lernen

## Hinweise zur Nutzung

- Das Notebook ist für die interaktive Ausführung konzipiert
- Führen Sie die Zellen nacheinander aus (Shift+Enter)
- Die komplette Ausführung dauert etwa 10-15 Minuten
- Bei der ersten Ausführung werden die Wetterdaten live abgerufen

## Nützliche Links

- [Jupyter Notebooks Dokumentation](https://jupyter-notebook.readthedocs.io/)
- [Deutscher Wetterdienst Open Data](https://opendata.dwd.de/)
- [Bright Sky API](https://brightsky.dev/)
- [Scikit-learn Benutzerhandbuch](https://scikit-learn.org/stable/user_guide.html)

## Mitwirken

Feedback, Verbesserungsvorschläge und Pull Requests sind herzlich willkommen! Erstellen Sie gerne ein Issue oder kontaktieren Sie uns direkt.

## Lizenz

Dieses Projekt steht unter der GNU General Public License v3.0 - siehe LICENSE für Details.

---

*Entwickelt zur Förderung der Data Literacy im Ingenieurstudium* 🎓⚡
