# 🚀 Installationsanleitung: Lokaler RAG-Chatbot

Diese Anleitung führt Sie durch die Einrichtung einer vollständig lokalen KI-Umgebung. Alle Daten verbleiben auf Ihrem Rechner – ideal für sensible Unternehmensdaten wie das Leitbild des Mittelstand-Digital Zentrums.

---

## 1. Grundinstallation der Software
Laden Sie die folgenden Programme herunter und installieren Sie diese:

1. **Docker Desktop:** [https://www.docker.com/products/docker-desktop/](https://www.docker.com/products/docker-desktop/) (Wichtig für die Container-Umgebung).
2. **Ollama:** [https://ollama.com/download](https://ollama.com/download) (Die Engine, die das Sprachmodell lokal ausführt).
3. **Open WebUI:** Über dieses Repository bereitgestellt (Start via Docker).

---

## 2. System starten
Öffnen Sie Ihr Terminal/Eingabeaufforderung im Ordner dieses Projekts und führen Sie den Start-Befehl aus:
```bash
docker-compose up -d
