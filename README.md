# 🚀 Installationsanleitung: Lokaler RAG-Chatbot

Diese Anleitung führt Sie durch die Einrichtung einer vollständig lokalen KI-Umgebung. Alle Daten verbleiben auf Ihrem Rechner – ideal für sensible Unternehmensdaten wie das Leitbild des Mittelstand-Digital Zentrums.

---

⚠️ Speicherplatz-Check: Vergewissern Sie sich vor dem Start, dass mindestens 15 GB freier Festplattenspeicher verfügbar sind. Die KI-Modelle und Docker-Container benötigen diesen Platz initial für den Download.


---
## 1. Grundinstallation der Software
Laden Sie die folgenden Programme herunter und installieren Sie diese:

1. **Docker Desktop:** [https://www.docker.com/products/docker-desktop/](https://www.docker.com/products/docker-desktop/) (Wichtig für die Container-Umgebung).
2. **Ollama:** [https://ollama.com/download](https://ollama.com/download) (Die Engine, die das Sprachmodell lokal ausführt).
3. **Open WebUI:** Über dieses Repository bereitgestellt (Start via Docker).

---

## 2. System starten
Vorraussetzung:

Installiere Docker Desktop und stelle sicher, dass es läuft (Wal-Symbol in der Menüleiste).

**Schritt 1:** Projekt herunterladen
  - Lade dieses Repository als ZIP herunter und entpacke es oder nutze git clone.

**Schritt 2:** Im Terminal zum Ordner navigieren
  - Öffne das Terminal.
  - Tippe cd  (mit Leerzeichen danach).
  - Ziehe den entpackten Projektordner per Drag-and-Drop in das Terminalfenster und drücke Enter.

**Wichtig:** Du musst dich im selben Ordner befinden, in dem auch die Datei **docker-compose.yml** liegt!

**Schritt 3:** Installation starten
  - Führe diesen Befehl aus:

```Bash
docker-compose up -d
```
-> Hinweis: Falls Fehlermeldungen zur Formatierung kommen, stelle sicher, dass die Datei als "Reiner Text"(.yml) gespeichert wurde.

---

## 3. Verbindung prüfen
