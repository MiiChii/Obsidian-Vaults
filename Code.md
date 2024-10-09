```c++
#include <string>
#include <chrono>

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

class Kunde : public Person {
protected:
	int kundennummer;
	Adresse lieferadresse;
}
```