DameArena Mobile 1.0 – erster spielbarer Prototyp

INHALT
index.html, app.js, manifest.webmanifest, sw.js, icon.svg

INSTALLATION AUF DEM IPHONE
1. Die fünf Dateien unverändert auf einem HTTPS-Webhost in denselben Ordner hochladen.
2. Die URL in Safari auf dem iPhone öffnen.
3. Teilen -> Zum Home-Bildschirm -> Hinzufügen.
4. Die App einmal bei bestehender Internetverbindung öffnen, damit der Offline-Cache gefüllt wird.
5. Danach kann die App ohne Internet gespielt werden.

WICHTIG
Eine ZIP-Datei allein lässt sich auf iOS nicht als PWA installieren. file:// unterstützt den Service Worker nicht. Ein HTTPS-Host (z.B. eigener Webserver) ist erforderlich.

TECHNIK
Die Zugregeln wurden aus dame_engine.py (Archiv 116.5.1) in JavaScript übertragen: Schlagpflicht, vorwärts schlagende einfache Steine, weit ziehende Damen mit Landung unmittelbar hinter dem geschlagenen Stein, Mehrfachschläge und Umwandlung. Die mobile KI ist eine separate Minimax-Implementierung und nicht die Windows-KI. Lokale Speicherung: Browser localStorage. JSON-Export: Community-Schema v1 (vorläufig).

GRENZEN DES PROTOTYPS
Keine Server-Synchronisierung, keine Community-Registrierung, kein Profil-Import, keine automatische Trainingsfunktion, keine validierte Gleichwertigkeit zur Windows-KI. Kein Anspruch auf vollständig getestete Spielregeln oder Remis-Äquivalenz. Der Zurück-Button ist eine einfache Testfunktion. Daten vor Safari-Datenlöschung exportieren. JSON-Export enthält personenbezugsfähige pseudonyme IDs und den Anzeigenamen; nicht ohne Prüfung veröffentlichen.
