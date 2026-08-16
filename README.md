# CSS Clamp Generator  
## Tools  
Es sind 2 in einem 1.  
Der ***Clamp Generator*** als Herzstück des Tools und im unteren Bereich ist eine ***Umrechnung von PX nach REM*** und vice versa mit verbaut. Beide Tools sind unabhängig von einander bedienbar und weisen keine unmittelbaren (Skript)Abhängigkeiten auf.
## Aufbau  
Auf Basis Bootstrap 5.  
HTML und Javascript sind gemeinsam in einer Datei angeführt - können jedoch auch getrennt abgelegt werden.  
## `clamp()` CSS Funktion  
Die `clamp()` CSS Funktion begrenzt einen Wert innerhalb eines Bereichs von Werten zwischen einem definierten Mindest- und einem Höchstwert.  
Die Funktion nimmt drei Parameter ein:  
- einen Mindestwert
- einen bevorzugten Wert
- einen maximal zulässigen Wert

[Auszug aus developer.mozilla.org](https://developer.mozilla.org/de/docs/Web/CSS/Reference/Values/clamp)
## Berechnung  
**Die Berechnung folgt dieser Logik:**  
Bei `Viewport-Breite X_min` soll die `Schrift Y_min` sein  
Bei `Viewport-Breite X_max` soll die `Schrift Y_max` sein  
Steigung = `(Y_max - Y_min) / (X_max - X_min)`   
Achsenabschnitt = `Y_min - Steigung × X_min` 
