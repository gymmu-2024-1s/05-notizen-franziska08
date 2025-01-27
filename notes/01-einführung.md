# Einführung

Hier sind meine Notizen zur Einführung in Daten.

- gespeicherte Informationen im internet
- verschiedene Formen
- Daten Speicherorte : Cloud im Internet, (Icloud), Sim-Karte, Sd-Karten,
  Festplatte (1 Terrabite platz)
- aktiviert oder deaktivierte Zellen, Speicherzellen in einem Block
- Durch eine Verbindung zweier Geräte, schickt man durch eine Form 1 und 0 (bsp.
  Licht (1)an/(0)ab)
- 1 Sekunde kann man tausend Bitz verschicken
- Computer kann nur in Bitz abspeichern, kann man dann in der Tabelle anschauen
  welche Zahl = welcher Buchstabe/Zeichen ist(Ascii)
- Durch denn Code (0,1,1,0) wird eine Zahl vom Ascii (z.B 65) code rausbekommen
  (z.b A) und kann es dann in der Tabelle ablesen

```JSON
{
    "vorname": "Jorche"
    "nachname": "Sevilla"

}*
```

```JSON
{
    "Titel" : "Caraval"
    "Autor" : "Stephanie Garber"
    "Verlag" : "Heyne Verlag"
    "Genre" : "Romantasy"
    "Erscheinungsjahr" : "2017"
    "Seitenzahl" : "400"
}

Redundant = überflüssige Informationen
z.b Geburtsdatum, dann brauch es kein Alter, da man es ausrechnen könnte

- möchte man vermeiden, vorallem beim modellieren
Alter speichert man nie mit ausser es gibt kein Geburtsdatum

Gute Redundant: Wenn das Objekt eine Datenkorruption hat, dann kann man es prüfen ob dies stimmt.

Datenspeicherung: Redundaz nicht erwünscht, da man nicht etwas doppelt haben möchte
Ansicht: Redundanz erwünscht, damit mehr Informationen

Was ist Redundaz und warum ist es schlecht?
Weil es sich wiederholt, speicherplatz (heute nicht mehr) wegnimmt und unnötige Information. Daten immer anpassen, Datenübersicht ist zu viel = unübersichtlich.

Gut: weil mehr und genauere Informationen über ein Objekt.

Wie unterscheiden sich Datenspeicherung und Datenansichten?

Bei der Datenspeicherung geht es um die nötigsten Informationen die gespeichert werden sollen. Bei der Datenansicht ist das wichtigste an Informationen gegeben, doch werden auch detailiertere Dinge aufgeschrieben.


Was sind berechnete Attribute und was hat das mit Redundanz zu tun?

Geben sie ein Beispiel für ein Objekt mit und ohne Redundant! Welche Eigenschaften sind Redundant?


Erklären sie in 31 Sätzen wie die Daten gespeichert werden und über das Internet/Gerät übertragen werden?

```

2.Theoriestunde

Sachen die wir zusammenpacken nennen wir Objekte.

const ball = { radius: 10, x: 100, y: 100, } //Wie man ein Objekt darstellt,
Eigenschaften die das Objekt ergeben, auf die Eigenschaften eingehen könnnen

Prüfungsfrage: Man muss einen Ball einfügen können. (Objekt)

Verschachtelung Objekt: Adresse

Komplexe Objekte eine Übersicht machen z.B { "vorname": "Peter", "nachname":
"Muster", "adresse": { "strasse": "Mustergasse", "strassenNr": 7, "plz": 4132,
"stadt": "Muttenz" } }

Verschachtelung gut--> Angebote z.B "Sportverein SV Muttenz" : {"Angebot 1":
"Fussball", "Angebot 2": "Handball", "Angebot 3": "Volleyball", "Angebot
4":"Basketball" }

Verschachtelung schlecht --> Namen als Personendaten ist unnötig weil es nachher
schon steht.

Listen Es sind immer mehere Objekte verschachtelt. Es braucht keinen Schlüssel
in einer Liste.

Klasse Ein Objekt ist eine Representation unserer Daten. Objekt ist eine Instanz
(eine Endscheidung zuständige Stelle) von unserer Klasse. Klassen sind Baupläne
für Objekte. Welche Eigenschaften vorhanden sind aber ohne Werte.

class Killerwal { Tierart, Stammbaum, Herkunft, alter, grösse }

Vererbung, Erweiterung eines Objekts. Alles was in der class Haustier drinnen
ist, ist auch in den anderen Klassen unter (Fisch und Hund) drinnen, einfach man
sieht es nicht. Alles aus der Basic Class vorhanden.

Class Fisch erbt die Eigenschaften von Class Haustier und nimmt dort die
Eigenschaft und überdeckt diese. Im Code erweitert es die Informationen.

Prüfungsfrage: Geben sie mir eine Instanz der Class Hund an. Heisst Rasse, Art,
Name usw. Erklären sie an hand diesem Beispiel warum Vererbung praktisch ist?

Datenquelle, Website lesen html Daten kann man angeben mit dem Schema der Class.
