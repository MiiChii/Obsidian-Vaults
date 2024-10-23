#### Aufgabe 1
Zum Zusammensetzen von m Matrizen braucht man n-1 Matrixmultiplikationen. Für je eine Translation, Skalierung und Rotation sind das also 2 Multiplikationen. Dann noch eine Multiplikation für jeden Punkt, bei n Punkten also 2 M-Multiplikationen + n Vektor-Matrix-Multiplikationen.
Zum Berechnen der Punkte einzeln braucht es 3 V-M-Multiplikationen für jeden Punkt, also 3n V-M-Multiplikationen

Eine 4x4 M-Mult. besteht aus 64 Multiplikationen und 48 Additionen => 112 Rechnungen. 
Eine V-M-Mult. besteht aus 16 Multiplikationen und 4 Additionen => 20 Rechnungen

a) 128 + 16n
b) 48n

48n > 128 + 16n
32n > 128
n > 4 => Ab 4 Punkten ist es gleich schnell.



