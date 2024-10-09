#### Aufgabe 1
Die Konvertierung eines 64-bit floating-points zu einem 16-bit signed int, jedoch war die Zahl zu groß für den int -> Overflow

#### Aufgabe 2
Parallel laufende Prozesse wurden nicht richtig synchronisiert, wodurch bei nachträglichen Benutzereingaben nur ein Teil der Daten richtig ankamen.

#### Aufgabe 3
Einer der Stabilisations-Antriebe bei der Landung hat nicht gestartet.
Bei sn10 war der Hauptantrieb bei der Landung zu stark. (Beides "Hardware"-Probleme)

#### Aufgabe 4


#### Aufgabe 5
![[Pasted image 20241008134025.png]]

###### Header:
Person:

```c++
#include <iostream>

class Person {
protected:
	std::string name;
	std::string vorname;
	year_month_day geburtsdatum;
	int alter;
}

class Adresse {
protected:
	std::string ort;
	std::string plz;
	std::string strasse;
	std::string hausnummer;

public:
	void drucken(std::string n, std::string vn);
}

class Kunde : protected Person {
protected:
	int kundennummer;
	Adresse lieferadresse;
}

```