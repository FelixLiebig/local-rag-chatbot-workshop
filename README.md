# 🤖 Lokaler RAG-Chatbot Workshop

Dieses Projekt ermöglicht die lokale Ausführung eines KI-Chatbots mit **Retrieval Augmented Generation (RAG)**. Es wurde im Rahmen einer Aufgabe für das **Mittelstand-Digital Zentrum Magdeburg** entwickelt.

## 🎯 Zielsetzung
Bereitstellung einer portablen und datenschutzkonformen Umgebung, in der KMU eigene Dokumente (z. B. ein Unternehmensleitbild) mithilfe lokaler Sprachmodelle (SLM) analysieren können.

## 🛠️ Voraussetzungen
Bevor du startest, stelle sicher, dass folgende Software installiert ist:
* **Docker Desktop** (für Windows, Mac oder Linux)
* Mindestens 8 GB RAM (empfohlen 16 GB)

## 🚀 Schnellstart
1. **Repository herunterladen:** Lade dieses Projekt als ZIP-Datei herunter und entpacke es.
2. **Container starten:** Öffne dein Terminal im Ordner und starte die Umgebung:
   ```bash
   docker-compose up -d






   
# 🤖 Lokaler RAG-Chatbot für den Mittelstand
**Workshop-Projekt:** Mittelstand-Digital Zentrum Magdeburg

Dieses Projekt zeigt, wie Unternehmen eine eigene, vollständig datenschutzkonforme KI-Infrastruktur aufbauen können, um interne Dokumente (wie das Unternehmensleitbild) sicher zu analysieren.

---

## 💡 Das Konzept: Warum lokal und was ist RAG?
Bevor wir zur Installation kommen, das Wichtigste für die Präsentation:

1. **Datenschutz:** Im Gegensatz zu Cloud-Diensten verbleiben alle Daten auf Ihrer Hardware. Es erfolgt keine Übermittlung an externe Server.
2. **RAG (Retrieval Augmented Generation):** Die KI wird nicht nur mit allgemeinem Wissen genutzt. Durch RAG "liest" die KI Ihre spezifischen PDFs (z. B. das Leitbild) und nutzt diese als exklusive Wissensquelle.
3. **Open WebUI & Ollama:** Ollama ist der "Motor" (das Modell), Open WebUI ist das "Armaturenbrett" (die Benutzeroberfläche).

---

## 🛠️ Schritt 1: Installationsanleitung
Bevor wir starten, müssen die folgenden Software-Komponenten installiert sein:

1. **Docker Desktop:** [Hier herunterladen](https://www.docker.com/products/docker-desktop/) (Verwaltet die Container-Umgebung).
2. **Ollama:** [Hier herunterladen](https://ollama.com/download) (Führt die KI-Modelle lokal aus).
3. **Projekt-Dateien:** Laden Sie dieses Repository als ZIP herunter und entpacken Sie es.

### System starten
Öffnen Sie Ihr Terminal im Projektordner und starten Sie die Umgebung:
```bash
docker-compose up -d
