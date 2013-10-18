Connets 4 circuit
=================

Idee
----

Ziel unseres Projekts war das Realisieren einer Schaltung, mit welcher ein 4-Gewinnt-Spiel dargestellt werden kann.
Das Spiel funktioniert in etwa so:
* Es gibt zwei Spieler
* Das Spielfeld besteht aus 6 Reihen und 7 Spalten (6x7 Felder)
* Die Spieler können abwechselnd ein Feld mit ihrer Farbe (Rot oder Gelb) besetzen
* Der Spieler der zuerst 4 in eier Reihe hat, gewinnt
* Die Reihen können horizontal, vertikal und diagonal sein.

Aufgrund der Komplexität haben wir auf die Auswertung, welcher Spieler gewonnen hat, verzichtet.

Schaltung
---------
Die Schaltung wurde in Logisim erstellt. Die folgende Abbildung zeigt das Spielfeld:

![Schaltung_Spielfeld](http://res.cloudinary.com/hag75sfi3/image/upload/v1382105079/schaltung_ekrs0x.png)

Selbstgebaute Komponenten
-------------------------

### Column (Spalte)

Stellt eine von 7 Spalten dar, in denen ein Spieler Felder besetzen kann. Es wird sichergestellt,
dass immer das nächst höhere Feld besetzt wird. Für das Spielfeld werden 7 solcher Spalten zusammengesetzt.

![Schaltung_Spielfeld](http://res.cloudinary.com/hag75sfi3/image/upload/v1382105398/column_yhcch7.png)

### Node (Feld)

Das Feld hat einzig und allein die Funktion ein LED anzuschalten. Entweder für Spieler 1 oder Spieler 2.
Ist das Feld einmal gesetzt, kann es nicht mehr geändert werden. Aussnahme: Reset-Funktion.

![Schaltung_Spielfeld](http://res.cloudinary.com/hag75sfi3/image/upload/v1382105471/node_g6cqkv.png)

