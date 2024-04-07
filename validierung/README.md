# Vorbereitung und Validierung der Daten für den Finetuning-Prozess

Dieses Verzeichnis enthält alle erforderlichen Codes und Anleitungen, um deine Daten für den Finetuning-Prozess von `FinetuningPflegeGPT` vorzubereiten. Hier findest du Schritte zur Datenvalidierung, -reinigung und -transformation, die für die Optimierung des Modells notwendig sind.

## Nützliche Ressourcen

- **Fragegenerator**: Für Projekte, die strukturierte Fragen aus Text generieren möchten, empfehlen wir den Einsatz des [Fragegenerators](https://trainmy.ai/qa-generator/).

## Schritt 1: Hinzufügen eines Suffix in der Tabelle

Um die Daten für die Verarbeitung vorzubereiten, beginnen wir mit dem Ausgangsdatensatz `validierung/trainingsdaten_modul1_roh.xlsx`. 

- **Ziel**: Füge neben der gewünschten Spalte eine neue Spalte mit der Funktion `=Spalte & "\n"` hinzu.
- **Durchführung**:
  - Verwende die AutoFill-Funktion, um dies auf alle Zeilen anzuwenden.
  - Kopiere die gesamte Spalte und füge sie als Werte in die ursprüngliche Spalte ein (Achtung: Nur Werte übertragen).
  - Lösche die temporäre Funktionsspalte.
- **Ergebnis**: Der aufbereitete Datensatz sollte als `validierung/trainingsdaten_modul1_clean.xlsx` gespeichert werden.

## Schritt 2: Reinigung des Datensatzes

Für die Reinigung verwenden wir den Datensatz `validierung/trainingsdaten_modul1_clean.xlsx` und das Jupyter Notebook `dataclean_colab.ipynb`.

- **Ziel**: Entferne doppelte und fehlende Zeilen zur Optimierung der Finetuning-Daten.
- **Tool**: [![Open in Colab](https://img.shields.io/badge/Open%20in%20Colab-%F0%9F%9A%80-blue)](https://colab.research.google.com/drive/1iaAI5izpQmU2BcRGkTrHClrUfqAlM9SF?usp=sharing)

## Schritt 3: Umwandlung der gereinigten Daten in das finale JSON-Format

Nach der Reinigung liegen die Daten als `validierung/outputs/formatted_trainingsdaten_modul1.xlsx` vor und müssen für das Finetuning in ein JSON-Format umgewandelt werden.

- **Tool**: Verwende das Notebook `exceltojson.ipynb` für die Umwandlung. Beachte, dass die CSV-Datei vorher z.B. in Google Sheets hochgeladen und in ein echtes `.xlsx`-Format umgewandelt werden muss.
- **Google Colab**: [![Open in Colab](https://img.shields.io/badge/Open%20in%20Colab-%F0%9F%9A%80-blue)](https://colab.research.google.com/drive/1PHUco4pQMcOsRbDIFREDdZVvo9pSdbT_?usp=sharing)

## Nützliche Tools

Im Notebook `Chat_finetuning_data_prep.ipynb` findest du weitere nützliche Tools zur Validierung deines Datensatzes und zur Berechnung der Kosten für das Finetuning.

---

Durch die Befolgung dieser Schritte stellst du sicher, dass deine Daten korrekt für den Finetuning-Prozess vorbereitet sind. Für weitere Fragen oder Anregungen, eröffne bitte ein Issue im Repository oder kontaktiere uns direkt.

[![Website](https://img.shields.io/badge/Pflege--AI-Webseite-%230f0122?style=flat&logo=Web&logoColor=ff8154)](https://pflege-ai.de/)