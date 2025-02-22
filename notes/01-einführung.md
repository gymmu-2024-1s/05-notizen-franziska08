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

3. Theoriestunde

Zahlensysteme: Dezimal 162 = 100 + 60 + 2 = 1 _100 + 6_ 10 + 2* 1 = 1*10^2 + 6
_10 ^1 + 2_ 10^0

Beispiel Dezimalsystem: 257 =

Wenn man die Zehnerzahl \*10 rechnet werden die Ziffern nach linksverschoben und
wenn durch dann Verschiebung nach rechts.

162 \*10 = 1620 162/10 =16,2

Binärsystem : 0 und 1 sind die zwei Ziffern 0b 101= 1*2^2 + 0*2^1 + 1\*2^0 = 5

Beispiel Binärsystem: 101110 --> 543210 1*2^5 + 0*2^4+ 1*2^3 + 1*2^2 + 1*2^1 +
0*2^0 = 46

ob 100 \*2 = 1000

Man rechnet alles zusammen und da 1\*2^0 = 1 noch +1 also ist diese Zahl im
Dezimalsystem =5 Die Basiszahl ist zwei da von 101 die Zahlen nummeriert werden
also (2,1,0 = 1,0,1)

1000= 1\*2^3 = 8

Hexadezimalsystem= 1(1)F(0)= 1*16^2 + F*16^0 = 1*16^1+ 15*16^0 = 16+15

Beispiel Hexadezimalsystem: 16 ist die Basiszahl

Multiplikation der Basiszahl = Verschiebung nach links 1 Bit ist eine
Speicherzelle 0 und 1

a Hexadezimal: 61 Binär: 01100001 Dezimal: 097 A Hexadezimal: 41 Binär:01000001
Dezimal:065

a hat in allen Systemen einen grösseren Wert als A.

Prüfungsfrage: Geben Sie ein kleines Objekt im JSON-Format ein. Was können Sie
jeweils in den verschiedenen Formaten beobachten? (er gibt einen Code-Block, was
für ein Dateiformat(JSON, Java, html,Svg, CSS, etc.) hat es?) mit Ascii ablesen
können.

Mit einem Bit kann man die Zahlen 0 bis 200 darstellen Hexadezimalsystem kann
man genau 2 stellen die geben ein Bit an

Verschlüsselung: Daten an nur einen Ort schicken, mit Verschlüsslungverfahren.
Kann man ver-/ und entschlüsseln. Binäreebene, entweder oder, XOr operation.

Schlüssel und verschlüsselter Text z.B QSQ und wir müssen die Nachricht
erkennen. Binär dargestellt und man schaut sich dann von beiden diesen Code an
und gibt 0 für gleich an und 1 für ungleich. Man schaut den Binärcode von dem
Schlüssel und dem verschlüsselten Wort an und findet so den Code für den
eigentlichen Text an. Man kann auch mit eigentlichem Text und verschlüsselten
Text den Schlüssel herausfindne und mit Schlüssel und eigentlichen Text den
verschlüsselten Code herausfinden.

Beispiel: abc in binär (01100001 01100010 01100011) = eigentlicher Text 012 in
binär (00110000 00110001 00110010) =Schlüssel QSQ in binär (01010001
01010011 01010001) = verschlüsselter Text

4. Theoriestunde

Bites ist der 0 oder 1 Wert, 1 Bit sind 8 dieser Bites grösste mögliche Zahl mit
1 Bit = 1111 1111 --> 255 (Hexadezimalsystem)

#ff00ff = Hexwerk, FF= R otanteil, 00=G rünanteil, FF= B lauanteil, FF= A lpha -
Wert Bitmap, 4 Bites die einen Pixel ergeben. Der Alpha- Wer sagt, wie die
Transparent es sein soll.

#00ff00 #0000ff #ff0000 #af00ff #000000 #ffffff #ffff00 #ffaf00
