# 🚀 Installationsanleitung: Lokaler RAG-Chatbot

Diese Anleitung führt Sie durch die Einrichtung einer vollständig lokalen KI-Umgebung. Alle Daten verbleiben auf Ihrem Rechner – ideal für sensible Unternehmensdaten wie das Leitbild des Mittelstand-Digital Zentrums.

---

⚠️ Speicherplatz-Check: Vergewissern Sie sich vor dem Start, dass **mindestens 20 GB freier Festplattenspeicher** verfügbar sind und der **Arbeitsspeicher(min 8GB RAM) relativ leer** sein sollte. Die KI-Modelle und Docker-Container benötigen diesen Platz initial für den Download.


---
## 1. Grundinstallation der Software
Laden Sie die folgenden Programme herunter und installieren Sie diese:

✅ **Docker Desktop:** [https://www.docker.com/products/docker-desktop/](https://www.docker.com/products/docker-desktop/) (Wichtig für die Container-Umgebung).
**WICHTIG beim Öffnen**
  - Konfigurations-Typ: Wählen Sie "Use advanced settings", "requires passwort" und "alle Haken setzen"
  - Einstellungen im Docker anpassen:
      - Einstellungen -> Ressourcen -> CPU: 2 , Memory: 3 , Swap: 1 , Disk usage: 32

✅ **Ollama:** [https://ollama.com/download](https://ollama.com/download) (Die Engine, die das Sprachmodell lokal ausführt).

✅ **Git-Repository.zip:** Repository als ZIP-Datei herunterladen und entpacken!


---

## 2. System starten
Vorraussetzung:

Installiere Docker Desktop und stelle sicher, dass es läuft (Wal-Symbol in der Menüleiste).



**Schritt 1️⃣:** Projekt herunterladen
  - Lade dieses Repository als ZIP herunter und entpacke es oder nutze git clone.


**Schritt 2️⃣:** Im Terminal zum Ordner navigieren
  - Öffne das Terminal.
  - Tippe cd  (mit Leerzeichen danach).
  - Ziehe den entpackten Projektordner per Drag-and-Drop in das Terminalfenster und drücke Enter.

    **Wichtig:** Du musst dich im selben Ordner befinden, in dem auch die Datei **docker-compose.yml** liegt!


**Schritt 3️⃣:** Installation starten
  - Führe diesen Befehl aus:

```Bash
docker-compose up -d
```
-> Hinweis: Falls Fehlermeldungen zur Formatierung kommen, stelle sicher, dass die Datei als "Reiner Text"(.yml) gespeichert wurde.


**Schritt 4️⃣:** OpenWebUI öffnen
  - Über Docker öffnen
  - Oder im Browser: http://localhost:3000

---

## 3. Modell herunterladen

**1️⃣** Klicke in Open WebUI (Browser) unten links auf deinen Namen/User-Icon.

**2️⃣** Geh auf Admin-Bereich -> Einstellungen -> Modelle -> Verwalten

**3️⃣** In dem Feld "Ein Modell von Ollama laden" gibst du ein: llama3

**4️⃣** Klicke auf das Download-Symbol (die Wolke).

-> Jetzt erst erscheint oben im Chat das Dropdown-Menü zur Auswahl.

---

## 4. Blechtech Modell und Wissen importieren

**1️⃣** Klicke in Open WebUI (Browser) unten links auf deinen Namen/User-Icon.

**2️⃣** Geh auf Admin-Bereich -> Einstellungen -> Modelle -> Verwalten

**3️⃣** In dem Feld "Ein Modell von Ollama laden" gibst du ein: llama3

**4️⃣** Klicke auf das Download-Symbol (die Wolke).
