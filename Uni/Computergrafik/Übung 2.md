#### Aufgabe 1
Zum Zusammensetzen von m Matrizen braucht man n-1 Matrixmultiplikationen. Für je eine Translation, Skalierung und Rotation sind das also 2 Multiplikationen. Dann noch eine Multiplikation für jeden Punkt, bei n Punkten also 2 M-Multiplikationen + n Vektor-Matrix-Multiplikationen.
Zum Berechnen der Punkte einzeln braucht es 3 V-M-Multiplikationen für jeden Punkt, also 3n V-M-Multiplikationen

Eine 4x4 M-Mult. besteht aus 64 Multiplikationen und 48 Additionen => 112 Rechnungen. 
Eine V-M-Mult. besteht aus 16 Multiplikationen und 12 Additionen => 28 Rechnungen

a) 224 + 28n
b) 84n

84n > 224 + 28n
56n > 224
n > 4 => Ab 4 Punkten ist es gleich schnell.


#### Aufgabe 2
![[Pasted image 20241023163304.png]]


#### Aufgabe 3
###### Teilaufgabe 1

Zeige dass gilt: $R_z(\alpha)*S(s)=S(s)*R_z(\alpha)$



$$ 
\begin{aligned}

R_z(\alpha)*S(s) =\\

\left[
\begin{array}{} 
\cos\alpha & -\sin\alpha & 0 \\
\sin\alpha & \cos\alpha  & 0 \\
0        & 0         & 1
\end{array}
\right]
* 
\left[
\begin{array}{} 
s & 0 & 0 \\ 
0 & s & 0 \\ 
0 & 0 & s 
\end{array}
\right] =

\\

\left[  
\begin{array}{} 
s*\cos\alpha + 0 + 0   &   0 - s*\sin\alpha + 0   &   0 + 0 + 0   \\
s*\sin\alpha + 0 + 0   &   0 + s*\cos\alpha + 0   &   0 + 0 + 0   \\
0 + 0 + 0              &   0 + 0 + 0              &   0 + 0 + s
\end{array}
\right] = \\

\left[  
\begin{array}{} 
s*\cos\alpha   &   -s*\sin\alpha   &   0   \\
s*\sin\alpha   &   s*\cos\alpha    &   0   \\
0              &   0               &   s
\end{array}
\right] \\ \\




S(s) * R_z(\alpha) =\\

\left[
\begin{array}{} 
s & 0 & 0 \\ 
0 & s & 0 \\ 
0 & 0 & s 
\end{array}
\right]
*
\left[
\begin{array}{} 
\cos\alpha & -\sin\alpha & 0 \\
\sin\alpha & \cos\alpha  & 0 \\
0        & 0         & 1
\end{array}
\right] =

\\

\left[  
\begin{array}{} 
s*\cos\alpha + 0 + 0   &   s*-\sin\alpha + 0 + 0   &   0 + 0 + 0   \\
0 + s*\sin\alpha + 0   &   0 + s*\cos\alpha + 0    &   0 + 0 + 0   \\
0 + 0 + 0              &   0 + 0 + 0               &   0 + 0 + s
\end{array}
\right]= \\

\left[  
\begin{array}{} 
s*\cos\alpha   &   -s*\sin\alpha   &   0   \\
s*\sin\alpha   &   s*\cos\alpha    &   0   \\
0              &   0               &   s
\end{array}
\right] q.e.d.\\

\end{aligned} 
$$


###### Teilaufgabe 2
