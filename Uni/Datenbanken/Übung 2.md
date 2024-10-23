#### Adresse:

| int    | int      | String | String | String  | 
| ------ | -------- | ------ | ------ | ------- |
| persNr | adressNr | plz    | ort    | strasse |

#### Person
| int    | String | String  | Date   | char | 
| ------ | ------ | ------- | ------ | ---- |
| persNr | Name   | Vorname | GebDat | G    |

#### Verkäufer
| int    | String   | Date         |
| ------ | -------- | ------------ |
| persNr | stellung | eintrittsdat |

#### Kunde
| int    | Date   | String |
| ------ | ------ | ------ |
| persNr | kdSeit | status | 

#### Einkauf
| int   | int       | Timestamp | String  |
| ----- | --------- | --------- | ------- |
| perNr | einkaufNr | zeitpunkt | zahlweg | 

#### Artikel
| int       | String  | String | String     | Decimal |
| --------- | ------- | ------ | ---------- | ------- |
| artikelNr | artname | artkat | kurzbeschr | preis   | 

#### EinkaufArtikel
| int       | int       | int    |
| --------- | --------- | ------ |
| einkaufNr | artikelNr | anzahl |

#### Bankverbindung
| int    | int     | String | String |
| ------ | ------- | ------ | ------ |
| persNr | bankvNr | IBAN   | BIC    | 




