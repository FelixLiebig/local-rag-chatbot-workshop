# 🚀 Installationsanleitung: Lokaler RAG-Chatbot

Diese Anleitung führt Sie durch die Einrichtung einer vollständig lokalen KI-Umgebung. Alle Daten verbleiben auf Ihrem Rechner.

---

⚠️ System-Check vorab

- Festplatte: Mindestens **25 GB** freier Speicherplatz (Zwingend erforderlich!).

- Arbeitsspeicher: Mindestens **8 GB RAM** (Schließen Sie ungenutzte Programme wie Chrome-Tabs oder Teams während der Installation).


---
## 1. Grundinstallation der Software
Laden Sie die folgenden Programme herunter und installieren Sie diese:

✅ **Docker Desktop:**
Wählen Sie eine der folgenden Umgebungen für die Container-Technik:

  - Option A: OrbStack (nur für Mac) Sehr schnell, ressourcenschonend und ideal bei wenig Festplattenplatz. 👉 [orbstack.dev](https://orbstack.dev/download)

  - Option B: Docker Desktop (Standard) 👉 [docker.com](https://www.docker.com/products/docker-desktop/)
    
     - Beim ÖFFNEN: Wählen Sie "Use advanced settings", "requires passwort" und "alle Haken setzen"
       
     - nach der Installation: Gehen Sie in die Settings -> Resources und stellen Sie folgende Werte ein:
       
    ```
         CPU: 2 | Memory: 2-6 GB | Swap: 1 GB | Disk usage: 24 GB
       ```


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

**Wenn du DOCKER verwendest:**
```Bash
docker-compose up -d
```

**Wenn du OrbStack verwendest:**
```Bash
orbstack-compose up -d
```


**Schritt 4️⃣:** OpenWebUI öffnen
  - 30sek warten und dann über Docker/Orbstack öffnen **oder** im Browser: http://localhost:3000

---

## 3. Modelle
herunterladen

**1️⃣** Klicke in Open WebUI (Browser) unten links auf deinen Namen/User-Icon.

**2️⃣** Geh auf Admin-Bereich -> Einstellungen -> Modelle -> Verwalten

**3️⃣** Feld "Ein Modell von Ollama laden":
- ein geeignetes Sprach-Modell laden! (gemma2 : 2b, llama3, mistral7b) - abhängig von CPU Leistung
- ein geeignetes Embedding-Modell laden! (all-minilm-l6-v2, nomic-embed-text, bge-large-en-v1.5) - abhängig von CPU Leistung

**WICHTIG:** Du benötigst zwingend ein Sprach-Modell UND ein Embedding-Modell!

**4️⃣** Klicke auf das Download-Symbol (die Wolke).

-> Jetzt erst erscheint oben im Chat das Dropdown-Menü zur Auswahl.


**5️⃣** Embedding-Modell hinzufügen
- Wechsel in der Menü-Bar von "Modelle" zu "Dokumente" -
- Füge unter "Embedding-Modell" den Namen deines Modells hinzu
- Stelle Chunk-Größen und Überlappung nach deinen Bedürfnissen ein

---

## 4. Blechtech-Konfiguration und Wissen importieren

**1️⃣** Klicke auf "Arbeitsbereich -> Modelle -> Importieren" und wähle die JSON-Datei aus Git-Ordner

**2️⃣** Geh zu Wissen und erstelle ein neuen Wissensspeicher, mit der PDF aus dem Git-Ordner

**3️⃣** Geh zu den 3 Punkten bei Modell "Blechtech" und füge das Sprachmodell, sowie WIssen hinzu

**4️⃣** FERTIG! -> Du kannst jetzt einen neuen Chat beginnen (musst aber oben links Blechtech auswählen)
