.txt - Files der einzelnen Skripte. "Blöcke importieren" / "Blöcke exportieren" mit Copy/Paste aus der Zwischenablage. Werden aber nicht gebraucht, wenn die Skripte als Ganzes als Zip-File importiert werden.

.zip - Gezippte Files der Skripte. Kann direkt als Zip-File importiert werden.

.json - Objektbaum der Variablen.


Es ist möglich im ioBroker sowohl die Variablen als auch die Skripte zu importieren. Dazu braucht man zwei Files "0_userdata.0.Akkutest.json" und "2024-03-09-scripts.zip". 

Die Vorgehensweise ist wie folgt:

- Installation ioBroker (wie im Artikel)
- Installation aller Adapter (wie im Artikel)
- Anbindung Shelly über MQTT (wie im Artikel)
- Unter den "Objekten" Import des kompletten Baums "0_userdata.0.Akkutest.json" (Pfeil nach oben - Objektbaum aus JSON-Datei hinzufügen).          
- Unter "Skripte" / Drei Punkte / "Skripte importieren" das Zip-file "2024-03-09-scripts.zip" importieren.
- In allen Skripten die Objekt-IDs zum Shelly-Baum manuell anpassen, da der Shelly Uni eine individuelle Kennung hat und daher die IDs bei Ihnen mit der aus diesem Github nicht übereinstimmt. 

Für einen Anfänger ist diese Vorgehensweise aber eher nicht zu empfehlen, da eine eventuelle Fehlersuche aufwändiger ist als die Eigenerstellung der Skripte. Außerdem muss der Objektbaum genau dahin, wo die Skripte ihn erwarten, sonst funktioniert es nicht. Für größere und komplexere Skripte kann es aber eine Zeitersparnis bedeuten.