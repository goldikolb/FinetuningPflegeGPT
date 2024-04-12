# Finetuning GPT für die Pflegebegutachtung

Dieses Repository zielt darauf ab, die Entwicklung eines speziell angepassten GPT-Modells für die Pflegebegutachtung voranzutreiben. Durch das Fine-Tuning von GPT auf spezifische Datensätze, die im Bereich der Pflegebegutachtung relevant sind, streben wir an, ein Modell zu entwickeln, das präzise und relevante Antworten auf Fragen in diesem Kontext liefern kann. Unser langfristiges Ziel ist die Schaffung eines leistungsfähigen Chatbots oder eines Pflegebegutachtungs-Agenten, der die Effizienz und Genauigkeit in der Pflegebegutachtung erheblich verbessern kann.

Aktuell stellen wir im Repository Datensätze zur Verbesserung des Moduls 1 der Pflegebegutachtung bereit. Die Entwicklung und Verbesserung der anderen Module erfolgen intern.

## Neue Ressourcen im Repository

### Normalisierung von Inhalten

Der neu hinzugefügte Jupyter Notebook 'normalize_content.ipynb' ist darauf ausgelegt, Inhalte aus HTML-, PPTX- oder PDF-Dateien in ein JSON-Format zu konvertieren. Diese Funktionalität unterstützt die Optimierung der Ausgabe für RAG (Retrieval-Augmented Generation), indem sie die Integration der Informationen in Vektordatenbanken erleichtert. Dies ist besonders nützlich, um die Effizienz der Datenabfrage und -verarbeitung in KI-Anwendungen zu verbessern.

#### Wichtiger Hinweis

Für die Nutzung dieser Funktionalität ist ein API-Schlüssel für Unstructured erforderlich. Bitte stellen Sie sicher, dass Sie einen gültigen API-Schlüssel besitzen, um die APIs vollumfänglich nutzen zu können. Die API-URL, die Sie für Anfragen verwenden, ist: [Webseite](https://api.unstructured.io/general/v0/general)
Weitere Informationen zur API und wie Sie einen API-Schlüssel erhalten können, finden Sie auf der offiziellen API-Seite: [Webseite](https://unstructured.io/api-key-free)

### Benchmarking

Im Ordner `Benchmarking` befindet sich eine Datei, die Ihnen ermöglicht, die Leistung verschiedener Modellversionen miteinander zu vergleichen. Diese Tools sind essentiell für die Erstellung und Auswertung eigener Benchmarks und unterstützen bei der objektiven Beurteilung der Modellperformance.

### bench_data

Im Ordner `bench_data` finden Sie eine Excel-Tabelle mit einem Beispieldatensatz. Dieser Datensatz umfasst unter anderem die zehn Fragen, die für das Benchmarking des Treppensteigens verwendet wurden, zusammen mit den korrekten Bewertungen. Diese Daten sollen Ihnen helfen, eigene Benchmarks zu erstellen und auszuwerten.

### Validierung

Der Ordner `Validierung` enthält nützliche Code-Snippets zur Überprüfung des JSON-Files, das für das Fine-Tuning der GPT-Modelle verwendet wird. Diese Codes sind unerlässlich, um sicherzustellen, dass die Fine-Tuning-Daten korrekt formatiert und für den Tuning-Prozess geeignet sind.

## Wie Sie beitragen können

### Datensätze

Im Ordner `Data` finden Sie die Datensätze, die aktuell für das Fine-Tuning des Moduls 1 verwendet werden. Diese Datensätze sind essenziell für die Entwicklung unseres spezialisierten Modells. Wir laden Sie ein, diese Datensätze anzusehen und uns Ihre Vorschläge für Verbesserungen oder Ergänzungen schriftlich mitzuteilen.

### Fine-Tuning und Modellverbesserung

Das Herzstück dieses Repositories bildet die `fintunegpt.ipynb`-Notebook-Datei, die Anweisungen zum Fine-Tuning des GPT-Modells mit unseren spezifischen Datensätzen enthält. Wir ermutigen Sie, mit diesem Notebook zu experimentieren und Ihre Ergebnisse oder Verbesserungen zu teilen.

## Zukünftige Pläne

Wir planen, dieses Repository regelmäßig zu aktualisieren und auf die Bedürfnisse der Pflegebegutachtung zuzuschneiden. Zukünftige Updates können Folgendes umfassen:

- Erweiterung der Datensätze für eine breitere Abdeckung von Pflegebegutachtungsthemen.
- Entwicklung von Testumgebungen, in denen angepasste Chatbots evaluiert werden können.
- Iterative Verbesserungen des Modells basierend auf Feedback und neuen Erkenntnissen aus der Forschung.

## Wie Sie dieses Projekt verwenden

Aktuell ist das Projekt in einer frühen Entwicklungsphase. Die Hauptnutzung besteht darin, das GPT-Modell mit den bereitgestellten Datensätzen zu finetunen. Folgen Sie den Anweisungen im `fintunegpt.ipynb` für den Einstieg. Zukünftige Updates werden detaillierte Anleitungen zur Verwendung des entwickelten Chatbots und zur Integration in bestehende Systeme enthalten.

## Mitwirkende

Wir laden jeden ein, der an der Verbesserung der Pflegebegutachtung durch künstliche Intelligenz interessiert ist, zu diesem Projekt beizutragen. Ob Sie Datensätze verbessern, am Code arbeiten oder Ideen für neue Funktionen einbringen möchten, Ihre Beiträge sind willkommen.

## Kontakt

Wenn Sie Fragen haben oder einen Beitrag leisten möchten, zögern Sie nicht, uns über unsere Webseite zu kontaktieren: [pflege-ai.de](https://pflege-ai.de/).

[![Website](https://img.shields.io/badge/Pflege--AI-Webseite-%230f0122?style=flat&logo=Web&logoColor=ff8154)](https://pflege-ai.de/)

## Follow me on Social Media

[![Threads](https://img.shields.io/badge/Threads-Follow%20me-blue?style=flat&logo=Thread&logoColor=white)](https://www.threads.net/@pflege_ki)

[![Twitter Follow](https://img.shields.io/twitter/follow/ai_fuerth?style=social)](https://twitter.com/ai_fuerth)

[![Instagram](https://img.shields.io/badge/Instagram-Follow%20@pflege__ki-blue?style=flat&logo=instagram&logoColor=white)](https://www.instagram.com/pflege_ki/)
