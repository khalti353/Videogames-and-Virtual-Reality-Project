# Zombie Survival VR

Ein Virtual-Reality-Spiel in Unity, in dem der Spieler Wellen von Zombies überleben muss.
Der Spieler wählt zu Beginn eine Waffe und kämpft in einer 3D-Welt gegen immer schnellere Zombies und einen Boss-Zombie.

**Technologien:** Unity, C#, XR Interaction Toolkit, OpenXR, Universal Render Pipeline (URP), TextMesh Pro

## Features

- **Charakterauswahl:** Pistole, Schwert oder Armbrust – jede Waffe mit eigener Spielmechanik
  (Schwert-Spieler haben mehr Lebenspunkte als Fernkämpfer)
- **Drei Waffensysteme:**
  - Pistole mit Raycast-Treffern
  - Schwert mit zeitgesteuertem Treffer-Collider und Schutz vor Mehrfachtreffern
  - Armbrust mit physikbasierten Pfeilen, die im Ziel stecken bleiben
- **Zombie-KI:** Zombies laufen auf den Spieler zu, mit Schritt- und Knurr-Sounds
- **Ragdoll-Physik:** Getroffene Zombies fallen realistisch um, abhängig von Waffe und Trefferpunkt
- **Steigende Schwierigkeit:** Zufälliges Spawnen von Zombies; alle 5 Kills werden sie schneller
- **Boss-Zombie:** Wenn der Boss stirbt, sterben alle normalen Zombies mit
- **Lebens- und Kill-System:** HUD mit Lebenspunkten und Kill-Zähler; alle 10 Kills gibt es Leben zurück
- **Game Over:** Nach dem Tod geht es automatisch zurück zur Charakterauswahl

## Projektstruktur (eigene Skripte)

| Skript | Aufgabe |
|---|---|
| `Zombie.cs` | Bewegung, Sound, Ragdoll und Tod der Zombies |
| `ZombieBoss.cs` | Boss-Zombie (erbt von `Zombie`) |
| `ZombieSpawner.cs` | Spawnen der Zombies und Erhöhung der Geschwindigkeit |
| `SwordAttack.cs` | Schwertangriff |
| `CrossbowShootSimple.cs`, `ArrowHit.cs` | Armbrust und Pfeil-Physik |
| `CharacterSelectMenu.cs`, `WeaponAssigner.cs` | Charakter- und Waffenauswahl |
| `GameOver.cs`, `KillCounter.cs` | Lebenspunkte, Kills und Game Over |

## Screenshots

![Screenshot 1](Screenshot%202026-09-30%20160256.png)
![Screenshot 2](Screenshot%202026-09-30%20160320.png)
![Screenshot 3](Screenshot%202026-09-30%20160354.png)
![Screenshot 4](Screenshot%202026-09-30%20160404.png)
![Screenshot 5](Screenshot%202026-09-30%20160419.png)
![Screenshot 6](Screenshot%202026-09-30%20160509.png)
