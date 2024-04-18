# Projektbericht: Online-Zahlungsbetrugserkennung mit maschinellem Lernen

## Projektübersicht

Das Ziel dieses Projekts ist die Entwicklung eines maschinellen Lernmodells zur Erkennung von Online-Zahlungsbetrug. Wir verwenden Transaktionsdaten, um betrügerische Aktivitäten von legitimen Transaktionen zu unterscheiden. Das Projekt umfasst die Datenvorbereitung, die Modellentwicklung, die Evaluierung und die Bereitstellung des Modells für die Betrugserkennung.

## Datenbeschreibung

Die verwendeten Daten stammen aus einem öffentlichen Datensatz von Kaggle ([Link zum Datensatz](https://www.kaggle.com/datasets/ealaxi/paysim1)) und enthalten Informationen zu Online-Zahlungstransaktionen. Die Merkmale umfassen den Transaktionstyp, den Betrag, die Kontostände vor und nach der Transaktion sowie Informationen über den Sender und den Empfänger der Transaktion.
Um Online-Zahlungsbetrug mithilfe von maschinellem Lernen zu identifizieren, müssen wir ein maschinelles Lernmodell trainieren, um betrügerische und nicht betrügerische Zahlungen zu klassifizieren. Dazu benötigen wir ein Datenset, das Informationen über Online-Zahlungsbetrug enthält, damit wir verstehen können, welche Art von Transaktionen zu Betrug führen. Für diese Aufgabe habe ich ein Datenset von Kaggle gesammelt, das historische Informationen über betrügerische Transaktionen enthält und verwendet werden kann, um Betrug bei Online-Zahlungen zu erkennen. Unten sind alle Spalten aus dem Datenset aufgeführt, das ich hier verwende:

- Schritt: repräsentiert eine Zeiteinheit, wobei 1 Schritt 1 Stunde entspricht
- Typ: Art der Online-Transaktion
- Betrag: Der Betrag der Transaktion
- nameOrig: Kunde, der die Transaktion startet
- oldbalanceOrg: Kontostand vor der Transaktion
- newbalanceOrig: Kontostand nach der Transaktion
- nameDest: Empfänger der Transaktion
- oldbalanceDest: Anfangsguthaben des Empfängers vor der Transaktion
- newbalanceDest: das neue Guthaben des Empfängers nach der Transaktion
- isFraud: Betrugstransaktion
## Projektstruktur

- **data**: Enthält den Datensatz und etwaige zusätzliche Daten.
- **notebooks**: Jupyter-Notebooks für die Datenanalyse, Modellentwicklung und -evaluation.
  - `Online Payments Fraud Detection with Machine Learning-Mohsen.Sabziyan.ipynb`: Hauptnotebook mit dem gesamten Projektverlauf.
- **scripts**: Python-Skripte für die Datenverarbeitung und Modellentwicklung.
- **models**: Gespeicherte Modelle nach dem Training.
- **reports**: Berichte, Dokumentation und Visualisierungen.
  - `project_report.md`: Projektbericht mit Zusammenfassung, Methoden, Ergebnissen und Schlussfolgerungen.
  - `figures`: Visualisierungen und Diagramme für den Bericht.

## Methoden

- **Datenbereinigung**: Bereinigung von fehlenden Werten und Anpassung von Datentypen.
- **Explorative Datenanalyse**: Analyse der Verteilungen, Korrelationen und Muster in den Daten.
- **Feature Engineering**: Erstellung neuer Merkmale zur Verbesserung der Modellleistung.
- **Modellentwicklung**: Training verschiedener maschineller Lernmodelle, einschließlich Decision Trees und Random Forests.
- **Modellbewertung**: Evaluierung der Modelle anhand von Metriken wie Genauigkeit, Präzision, Recall und F1-Score.
- **Visualisierung**: Erstellung von Visualisierungen wie Confusion Matrices und ROC-Kurven zur Analyse der Modellleistung.

## Ergebnisse

Das Notebook zeigt den gesamten Prozess von der Datenvorbereitung über die Modellentwicklung bis hin zur Evaluierung der Modelle. Es umfasst auch Visualisierungen wie Confusion Matrices und ROC-Kurven, um die Leistung der Modelle zu analysieren. Die Ergebnisse zeigen eine hohe Genauigkeit bei der Erkennung von betrügerischen Transaktionen.

## Schlussfolgerungen

Die Entwicklung von maschinellen Lernmodellen zur Erkennung von Online-Zahlungsbetrug ist ein wichtiger Schritt, um finanzielle Verluste zu minimieren und die Sicherheit von Zahlungssystemen zu verbessern. Die vorgestellten Modelle haben vielversprechende Ergebnisse erzielt und könnten in Echtzeit-Systeme integriert werden, um Betrug zu erkennen und zu verhindern.
