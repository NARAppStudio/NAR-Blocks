# NAR Blocks — PWA

NAR Blocks ist als Progressive Web App (PWA) vorbereitet.

## GitHub Pages veröffentlichen
1. Alle Dateien und Ordner aus diesem Paket in das Stammverzeichnis deines GitHub-Repositories hochladen.
2. GitHub → **Settings → Pages** öffnen.
3. Den gewünschten Branch und `/(root)` als Quelle auswählen.
4. Warten, bis GitHub Pages die Website veröffentlicht hat.
5. Die Website über die HTTPS-Adresse öffnen.

## Installation
- **Android / Chrome:** Website öffnen und im Browser-Menü „App installieren“ bzw. „Zum Startbildschirm hinzufügen“ auswählen.
- **iPhone / Safari:** Teilen → „Zum Home-Bildschirm“ → „Als Web-App öffnen“ aktivieren, falls angeboten.
- **Desktop / unterstützte Browser:** Installationssymbol in der Adressleiste oder Browser-Menü verwenden.

## Offline
Der Service Worker speichert den App-Kern (Spiel, Manifest und Icons) für den Offline-Start zwischen. Google Fonts werden extern geladen; offline wird die im CSS definierte Ersatzschrift verwendet.

## Hinweise
- PWA-Installation benötigt eine sichere Verbindung (HTTPS); GitHub Pages stellt HTTPS bereit.
- Service Worker funktionieren nach dem Deployment auf dem veröffentlichten HTTPS-Origin, nicht zuverlässig beim direkten Öffnen der HTML-Datei per `file://`.
- Spielstände bleiben lokal im jeweiligen Browser/Gerät und werden nicht automatisch synchronisiert.
- Die Impressumsangaben müssen vor öffentlicher Bereitstellung rechtlich vollständig sein.
