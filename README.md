# Grundriss CAD

Ein einfaches, vollständig lokal laufendes 2D-Zeichenwerkzeug für aktuelle Browser unter Windows und Android. `index.html` öffnen; Installation und Internet sind nicht erforderlich. Auf Android kann die Datei über einen Dateimanager im Browser geöffnet oder auf einem statischen Webserver bereitgestellt werden.

## Funktionen

Linien, Rechtecke und Kreise durch je zwei Klicks oder Berührungen zeichnen, Objekte auswählen, Koordinaten exakt bearbeiten, duplizieren und löschen, Entfernungen messen, Rasterfang, Ansicht verschieben und zoomen, Rückgängig/Wiederholen. Ein Beispiel erleichtert den Einstieg. Änderungen werden zusätzlich automatisch im lokalen Browserspeicher gesichert; dieser kann gelöscht werden, deshalb wichtige Projekte als JSON speichern. JSON-Projektdateien speichern die bearbeitbare Zeichnung. SVG exportiert die aktuelle Ansicht. DXF (ASCII) importiert LINE, CIRCLE und LWPOLYLINE mit geraden Segmenten; Bögen in Polylinien werden als gerade Segmente interpretiert. Nicht unterstützte Elemente werden übersprungen. DXF exportiert Linien und Kreise; Rechtecke werden zu Linien. DXF verwendet ein kartesisches Koordinatensystem, die Anzeige invertiert dessen Y-Achse. Import ersetzt die aktuelle Zeichnung; vorher speichern.

Die Anwendung ist ein Einstieg in 2D-CAD, kein vollständiges CAD-System: insbesondere keine DWG-, PDF-, Bemaßungs-, Layer-, Block-, 3D- oder vollständige DXF-Unterstützung. Einheiten sind frei wählbare Zeichnungseinheiten. Ergebnisse vor baulicher Verwendung fachlich prüfen.

## GitHub

Dieses Verzeichnis ist ein lokales Git-Repository. Nach dem Verbinden von GitHub ein leeres Repository erstellen und die von GitHub angezeigten Befehle zum Hinzufügen des Remotes und Pushen ausführen, beispielsweise:

```sh
git remote add origin https://github.com/DEIN-NAME/grundriss-cad.git
git push -u origin main
```

Für GitHub Pages unter Settings → Pages bei „Build and deployment“ die Quelle „Deploy from a branch“, den Branch `main` und `/ (root)` auswählen und speichern. Nach der Bereitstellung zeigt GitHub dort die Adresse an. Bei einem neuen, noch leeren Repository zunächst die Projektdateien hochladen und committen. Es werden keine externen Bibliotheken benötigt.
