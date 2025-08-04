\# PedsInWater - Tier-Schwimm-Fix für FiveM



---



\## 📄 Beschreibung



Dieses FiveM-Client-Skript löst ein bekanntes Problem in GTA V: Standardmäßig sterben Tier-Peds (wie Hunde, Katzen, Hirsche etc.) sofort, wenn sie in tieferes Wasser geraten. Dieses Skript stellt sicher, dass \*\*alle Tier-Peds\*\* im Wasser überleben, nicht ertrinken und sich dort frei bewegen können. Das ermöglicht ein realistischeres und unterhaltsameres Spielerlebnis, besonders wenn Spieler in die Rolle der Tier-Modelle schlüpfen.



Die Funktionalität ist \*\*ausschließlich für Tier-Peds\*\* vorgesehen. Menschliche Charaktere sind von dieser Logik ausgeschlossen und verhalten sich im Wasser weiterhin standardmäßig (können ertrinken und Schaden nehmen). Das bewahrt das Gameplay-Gleichgewicht auf Roleplay-Servern.





\*\*Ich bitte darum, falls dieses Script für RP verwendet werden soll, die Unsterblichkeit der Tiere innerhalb und 5 Sekunden nach verlassen des Wassers nicht im RP auszunutzen, um ein faires RolePlay zu ermöglichen.



---



\## ✨ Funktionen



\* \*\*Verhindert sofortiges Ertrinken/Sterben:\*\* Tier-Peds sterben nicht mehr, wenn sie in tieferes Wasser geraten.

\* \*\*Unverwundbarkeit im Wasser:\*\* Aktiviert temporäre Unverwundbarkeit für Tier-Peds, solange sie sich im Wasser befinden, um den "Hardcoded"-Tod des Spiels zu überwinden.

\* \*\*Dynamische Tier-Erkennung:\*\* Erkennt automatisch alle Tier-Peds (inklusive Custom-Modelle), mithilfe einer bearbeitbaren Liste von Hashes. Dabei wird geprüft, ob das ausgewählte Ped in der Liste Registriert ist und das Sccript funktioniert auch nur, wenn dies der fall ist. Die PedListe befindet sich in der `peds.lua`.

\* \*\*Optimierte Performance:\*\* Die detaillierte Wasser-Logik wird nur ausgeführt, wenn der Spieler ein Tier-Ped ist. Bei menschlichen Spielern bleibt das Skript im Hintergrund inaktiv und spart Ressourcen.

\* \*\*Keine Auswirkungen auf menschliche Peds:\*\* Normale Spieler-Charaktere können weiterhin ertrinken und Schaden nehmen.



---



\## 🚀 Installation



1\.  \*\*Herunterladen:\*\* Lade das `PedsInWater`-Ressourcenpaket herunter.

2\.  \*\*Entpacken:\*\* Entpacke die ZIP-Datei. Du solltest einen Ordner namens `PedsInWater` erhalten, der die Dateien `fxmanifest.lua`, `client.lua` und `peds.lua` enthält.

3\.  \*\*Verschieben:\*\* Platziere den gesamten `PedsInWater`-Ordner in den `resources` Ordner deines FiveM-Servers.

4\.  \*\*`server.cfg` anpassen:\*\* Öffne deine `server.cfg`-Datei (im Hauptverzeichnis deines FiveM-Servers) und füge folgende Zeile hinzu, um das Skript beim Serverstart zu laden:
a
    ```

    ensure PedsInWater

    ```

    \*Stelle sicher, dass die Groß-/Kleinschreibung des Ordnernamens korrekt ist!\*



\*\*\*`falls du das Script in eine Resourcengruppe gelegt hast, welche von dem Server automatisch im Start eingebunden ist, kannst du schritt 4 überspringen. Beispiel Hierfür: \\\\\\\[StandAlone].`



5\.  \*\*Server neustarten:\*\* Starte deinen FiveM-Server vollständig neu, damit die Änderungen wirksam werden.

 	`Funktioniert meistens aber auch über einfachen Script Restart`



---



\## 🛠️ Konfiguration (`peds.lua`)



Solltest du Tier-Ped Modelle haben, die kein Standard GTA Ped überschreiben kannst du diese in der Liste innerhalb der `peds.lua` Hinzufügen. Wichtig Hierbei zu beachten ist, dass du beim Hinzufügen wie folgt schreibst:



GetHashKey("PED SPAWN NAME")

\*\*Beispiel:

GetHashKey("a\_c\_husky")



---



\## ⚠️ Warnung



\*\*Durch die im Script aktivierte Unverwundbarkeit könnten Probleme mit manchen AntiCheat Systemen auftreten. Bitte nimm darauf Rücksicht, da dies außerhalbe meines Einflussbereiches liegt. Ich empfehle, dies auf deinem Server ausgiebig zu testen und gegebenenfalls im Anticheat anzupassen.

