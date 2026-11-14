# Fehlerbehebung – Head Tracker+Voice+Instructor

🌐 [English](troubleshooting.en.md) · [Русский](troubleshooting.ru.md) · [Français](troubleshooting.fr.md) · Deutsch · [Italiano](troubleshooting.it.md)

Suchen Sie Ihr Problem und gehen Sie die Schritte der Reihe nach durch. Hilft nichts, [senden Sie einen Bericht](#bericht-an-den-entwickler-senden).

## Installation

### „Der Computer wurde durch Windows geschützt“ – es geht nicht weiter
Klicken Sie auf **Weitere Informationen**, dann auf **Trotzdem ausführen**. Gibt es keine Schaltfläche **Trotzdem ausführen**, ist die intelligente App-Steuerung eingeschaltet: siehe [Installation, Schritt 2.5](install.de.md).

### Der Browser will die heruntergeladene Datei nicht behalten
Edge: **…** → **Behalten** → **Mehr anzeigen** → **Trotzdem behalten**. Chrome: auf die Datei klicken → **Unsichere Datei herunterladen**.

### Der erste Start dauert lange
Microsoft Defender prüft das neue Programm; das kann bis zu einer Minute dauern. Bitte warten Sie.

### Das Setup meldet „Das Programm läuft: Schließen Sie es…“
Schließen Sie das Programm über **Datei → Beenden** (nicht nur mit dem ✕ des Fensters) und starten Sie das Setup erneut.

## Verbindung zum iPhone

### Die iPhone-App meldet keine Verbindung zum PC
1. Das PC-Programm muss laufen.
2. **Kabel:** Schließen Sie es an, entsperren Sie das iPhone und antworten Sie mit **Vertrauen**, wenn es „Diesem Computer vertrauen?“ fragt.
3. **WLAN:** PC und iPhone müssen im selben Netz sein.
4. Tippen Sie in der App auf **Erneut versuchen**.

### Die Verbindung lief, brach aber während des Flugs ab
1. Prüfen Sie das Kabel (oder das WLAN).
2. Klicken Sie im PC-Programm erneut auf **Starten**.
3. Zeigt die App eine schwache WLAN-Qualität, nehmen Sie das Kabel oder gehen Sie näher an den Router.

### Auf dem iPhone ist alles in Ordnung, aber der PC meldet „Gesicht nicht sichtbar“
1. Öffnen Sie im PC-Programm **Einstellungen → iPhone** und wählen Sie die Verbindung (Kabel oder WLAN) noch einmal aus.
2. Klicken Sie erneut auf **Starten**.

### Mit Kabel wird das iPhone manchmal nicht gefunden
1. Ziehen Sie das Kabel ab und stecken Sie es wieder ein, während das iPhone entsperrt ist.
2. Schließen Sie andere Programme, die das iPhone als Kamera oder Webcam nutzen.
3. Versuchen Sie ein anderes Kabel oder einen anderen Anschluss am PC.

## Head-Tracking

### Die Ansicht bewegt sich nicht
1. Unten im Hauptfenster: Steht dort ein grünes **LÄUFT**? Wenn nicht, klicken Sie auf **Starten**.
2. Im Bereich „Ansicht“: Steht dort **Gesicht erkannt**? Wenn nicht, siehe unten.
3. Setzen Sie sich gerade hin und klicken Sie auf **Zentrieren** (Strg+Alt+C).
4. Prüfen Sie, dass **Pause** nicht eingeschaltet ist (Strg+Alt+X schaltet sie um).

### „Gesicht nicht sichtbar“
- Das iPhone muss auf Sie gerichtet sein, etwa eine Armlänge entfernt, ohne etwas zwischen Ihnen und der Kamera.
- Vermeiden Sie starkes Licht direkt hinter Ihrem Kopf.
- Haben Sie Ihr Gesicht kurz verdeckt, setzt das Tracking nach ein paar Sekunden von selbst wieder ein.

### Die Ansicht ist träge, ruckelig oder zu empfindlich
**Profile → Ansichtseinstellungen** → klicken Sie auf die fertige Kurve **Jäger** oder **Zivil**. Stellen Sie dann im Hauptfenster **Empfindlichkeit** und **Glättung** fein ein.

### Die Ansicht dreht sich falsch herum (links statt rechts)
Öffnen Sie **Profile → Ansichtseinstellungen**. Klicken Sie in der Liste **Achsen** auf das Symbol ⇄ rechts neben dieser Achse (⇄ = invertiert). [Melden Sie es](https://github.com/liaison-studio/htvi/issues/new/choose) dann bitte mit dem Namen des Simulators: Die Richtung sollte ohne Änderungen stimmen.

### Die Ansicht wandert mit der Zeit aus der Mitte
Setzen Sie sich gerade hin und drücken Sie **Strg+Alt+C** (oder sagen Sie „Ansicht zentrieren“). Um das automatisch auszugleichen, schalten Sie **Langsames Auto-Zentrieren** unter **Profile → Ansichtseinstellungen** ein.

## Sprachbefehle

### Ein Befehl wird nicht erkannt
1. Die Befehlssprache im PC-Programm (**Einstellungen → Stimme**) und die Sprache der Spracheingabe auf dem iPhone (**Einstellungen → Sprache der Spracheingabe**) müssen gleich sein. Weichen sie ab, zeigt das Hauptfenster einen gelben Hinweis.
2. Wenn Sie PTT nutzen, halten Sie die Taste gedrückt, während Sie sprechen.
3. Sprechen Sie kurz, wie ein Pilot: „Fahrwerk ausfahren“, kein langer Satz.
4. Die Liste der Sätze für Ihr Spiel steht im Fenster **Befehle**.

### Ein Befehl wurde erkannt, hat im Spiel aber nichts bewirkt
Klicken Sie unter dem letzten Befehl auf **Ging nicht – deaktivieren**. Das Programm merkt sich das, damit der Befehl verbessert werden kann. [Melden Sie es](https://github.com/liaison-studio/htvi/issues/new/choose) bitte auch, mit dem Satz und dem Simulator.

## Instructor

### Der Instructor schweigt
Windows hat keine Stimme für Ihre Sprache. **Windows-Einstellungen → Zeit und Sprache → Spracherkennung → Stimmen hinzufügen**, fügen Sie eine Stimme für Ihre Sprache hinzu und starten Sie das Programm neu.

### Der Instructor folgt dem falschen Flugzeug
Wählen Sie im Bereich „Instructor“ das Flugzeug selbst aus, statt **Auto**.

## Bericht an den Entwickler senden
1. **Service → Bericht für den Entwickler…**
2. Beschreiben Sie, was passiert ist.
3. Klicken Sie auf **Archiv speichern…**. Das Archiv wird unter *Dokumente → Head Tracker Voice Instructor → Reports* gespeichert.
4. Hängen Sie es an eine [Fehlermeldung](https://github.com/liaison-studio/htvi/issues/new/choose) an oder senden Sie es an liaison.studio.contact@gmail.com.

Der Bericht enthält keinen Ton und keine Kopplungsdaten. Das Programm sendet nie etwas von selbst.
