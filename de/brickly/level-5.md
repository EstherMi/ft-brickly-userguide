# Fünfter Erfahrungsgrad "Experte"    
Dies ist der höchste Erfahrungsgrad für die Experten. Neu sind hier die Listen-Bausteine. Eine Liste ist eine durchnummerierte Reihe von Elementen. Über die Nummer kannst du auf jedes Element zugreifen. 
![Liste](/list.png)
Die meisten Bausteine für Listen findest du in der neuen Gruppe "Listen", es gibt aber auch einen neuen Baustein unter "Schleifen" und einen bei "Mathe".      

## Neue Bausteine in "Eingänge"    
Hier gibt es einige neue Bausteine für die Nutzung eines USB-Joysticks. Die Joysticks/Gamepads werden per USB am TXT angeschlossen - am Standard-USB-Port. Zur Zeit funktionieren leider nur einige Typen, z.B. ein Speedlink Competition Pro USB Joystick.    

## Neu in "Ausgänge"    
* `gleichzeitig`. Mit diesem Baustein kannst du Ausgänge gleichzeitig setzen, z.B. zwei Motoren gleichzeitig starten, ohne gekoppelte Encoder-Motoren zu verwenden. Der Baustein funktioniert nicht mit den Bausteinen aus der Untergruppe "Mobil" (da drehen zwei Motoren ohnehin gleichzeitig).     

## Neue Untergruppe in "Ausgänge": "Mobil"    
* `fahre <vorwärts> <25> cm`: wie [hier](/level-1#fahre)  
* `fahre <vorwärts> <solange>`: wie [hier](/level-2#fahresolange)  
* `drehe <rechts> <90>`: wie [hier](/level-2#drehegrad)  
* `<90>°` und `<etwas> herum`: diese beiden Bausteine können an den `drehe`-Baustein angebaut werden, um den Drehwinkel einzustellen.    
* `Mobilroboter-Konfiguration`: Wenn du einen anderen Fahrroboter als den aus dem TXT-Discovery-Set gebaut hast, kannst du mit diesem Baustein am Anfang deines Programms einstellen, an welchen Anschlüssen die Motoren angeschlossen sind, von welchem Typ sie sind, wie die Antriebsübersetzung (Motorachse zu Radachse) ist, wie groß der Raddurchmesser ist und wie der Abstand zwischen den Antriebsrädern ist. Mit der richtigen Konfiguration sollen die Befehle zum Fahren und Drehen auch für deinen selbstkonstruierten Fahrroboter funktionieren. Für das Discovery-Set wird dieser Baustein nicht benötigt.      

## Neu in "Logik"       
* `null`: der Wert, den eine Variable hat, die zwar einen Namen hat, aber für die kein Wert gesetzt wurde.  
* `prüfe: falls wahr: falls unwahr:`: ein Wertbaustein, mit dem man den Wert auswählen kann. Nach *prüfe* kommt eine Bedingung. Wenn diese *wahr* ist, wird der Wert zurückgegeben, der nach *falls wahr* steht, sonst der Wert nach *falls unwahr*. (In der Informatik heißt das auch "Ternärer Operator" oder "Auswahloperator").       

## Neu in "Schleifen"       
* `für jeden Wert <i> aus der Liste: mache:` diese Schleife arbeitet sich von vorne bis hinten durch die Liste durch. Im Bauch der Schleife kannst du mit dem aktuellen Element (es heißt *i*) Befehle ausführen. Diese Befehle ändern die Liste selbst aber nicht.     

## Neu in "Mathe"     
* `<sin> <45>` stellt die Winkelfunktionen *sin*, *cos* und *tan* und die Arkusfunktionen *asin*, *acos* und *atan* zur Verfügung.  
* `<π>`: liefert die ausgewählte mathematische Konstante: die Kreiszahl π, die Eulersche Zahl e, den Goldenen Schnitt φ, die Quadratwurzel von 2 sqrt(2), die Quadratwurzel von 1/2 sqrt(1/2) oder unendlich ∞.  
* `<0> ist <gerade>`: ein Bedingungsbaustein, der prüft, ob die Zahl (hier 0) die ausgewählte Eigenschaft hat: *gerade*, *ungerade*, *eine Primzahl*, *eine ganze Zahl*, *positiv*, *negativ* oder *teilbar durch* (braucht noch eine 2. Zahl).
* `<runde> <3.1>` rundet die angegebene Zahl. Du kannst auch *runde auf* (aufrunden zur nächstgrößeren ganzen Zahl) oder *runde ab* (abrunden zur nächst kleineren ganzen Zahl) wählen.  
* `<Summe über die> Liste: ` gibt die Summe aller Elemente der ausgewählten Liste aus. Du kannst eine andere Funktionen auswählen, die dann eine andere Berechnung über alle Elemente durchführt (*Minimalwert*, *Maximalwert*, *Mittelwert*, *Median*, *am häufigsten*, *Standardabweichung*, *Zufallswert*).  
* `begrenze <50> zwischen <1> und <100>`: verwendet die angegebene Zahl (hier 50), wenn sie zwischen den beiden anderen Zahlen liegt. Wenn sie zu groß ist, wird die obere Grenze genommen (hier 100), und wenn wenn sie zu klein ist, die untere Grenze (hier 1). Sinnvollerweise nimmt man als Zahl hier eine Zahlenvariable.  
* `Zufallszahl (0.0 - 1.0)`: liefert eine zufällige Gleitkommazahl zwischen 0.0 und 1.0.     

## Neu in "Text"    
Hier findest du jetzt viele neue Bausteine, um Texte zu bearbeiten, Teile daraus zu finden usw.. Als "Experte" wirst du in dieser Gruppe finden, was du brauchst. Ein Baustein ist besonders nützlich: 
* `gib aus in <> <"abc">`: gibt den angegebenen Text in der ausgewählten Farbe aus.    

## "Listen"    
Um eine Liste zu erzeugen, erstellst du am einfachsten zuerst eine Variable für die Liste (z.B. "MeineListe"). Dann erzeugst du eine Liste mit einem der folgenden Bausteine und weist ihn der Variable zu. Die Variable mit deiner Liste findest du unter "Variablen".  
* `erzeuge eine leere Liste`: erzeugt eine leere Liste.  
* `erzeuge eine Liste mit: `: erzeugt eine Liste aus den angegeben Bausteinen. Durch Drücken auf das Zahnrad erhälst du wieder einen Kasten, mit dem du durch Hinzufügen oder Zurückschieben der Elementbausteine (*etwas*) mehr oder weniger Elementplätze in deiner Liste bereitstellen kannst. Wenn du die richtige Anzahl hast, drückst du wieder auf das Zahnrad. Um deine Liste zu füllen, baust du an die freien Plätze Wert-Bausteine an, z.B. Variablen, Zahlen oder Texte.  
* `erzeuge eine Liste mit <5> mal dem Element <>`: erzeugt eine Liste mit der angegebenen Länge (hier 5), die an jeder Stelle das gleiche Element enthält.  
* `Länge von: `: gibt die Länge der angebauten Liste (d.h. die Anzahl der Elemente) als Zahl aus.  
* `<> ist leer`: ein Bedingungsbaustein, liefert wahr, wenn die eingebaute Liste leer ist, d.h. keine Elemente enthält.  
* `in der Liste <Liste> suche <erstes> Auftreten von <>`: gibt die *erste* (oder *letzte*) Position zurück, an der sich das angegeben Element befindet. Der Wert ist 0, wenn kein passendes Element in der Liste ist.  
* `in der Liste <Liste> <nimm> <#tes> <>`: liefert das Element an der angegebenen Position (Zahl nach *#tes*) in der Liste. Du kannst auch auswählen *nimm und entferne*, dann wird das zurückgelieferte Element aus der Liste gelöscht, die Liste wird kürzer. Mit *entferne* wird auch das angegebene Element gelöscht, aber du erhälst keinen Wert zurück. Du kannst statt von vorne auch von hinten zählen (*#tes von hinten*), oder *erstes*, *letztes* oder *zufälliges* Element wählen. Achte darauf, dass die Positionsangabe einen Wert zwischen 1 und der Länge deiner Liste ergibt, sonst gibt das Programm eine Fehlermeldung.  
* `in der Liste <Liste> <setze für> <#tes> ein <>`: hier kannst du das Element an der angegebenen Position überschreiben, oder mit *füge ein* ein neues Element einbauen. Beim Einfügen wird die Liste länger.  
* `in der Liste <Liste> erhalte Unterliste <von #> <> bis <zu #> <>`: gibt alle Elemente zwischen den ausgewählten Positionen aus. Wenn die zweite Position vor der ersten liegt, ist die Unterliste leer.  
* `<Liste aus Text> erstellen <> mit Trennzeichen <",">`: erstellt eine Liste von Texten aus einem längeren Text, wobei die einzelnen Teile durch das angegebene Zeichen, z.B. ein Komma, getrennt sind.  
* `<nummerisch> <aufsteigend> <> sortieren`: liefert eine sortierte (*nummerisch*, *alphabetisch* (mit Großbuchstaben zuerst) oder *alphabetisch, Großschreibung ignorieren*) Kopie der angegebenen Liste. Die Liste selbst bleibt unverändert. Wenn die sortierte Kopie behalten möchtest, musst du die Variablenzuweisung `setze <meineVariable> auf` und diesen Baustein verwenden.
