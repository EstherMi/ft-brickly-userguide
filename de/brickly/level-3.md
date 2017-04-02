# Dritter Erfahrungsgrad "Fortgeschritten"    

Für die Fortgeschrittenen gibt es neue Bausteine für die Nutzung der Eingänge, und du lernst Variablen kennen.   
"Variablen sind Behälter im Speicher, die einen Namen haben und deren Inhalt sich während der Ausführung eines Programms ändern kann. Der Begriff der Variablen ist eines der wichtigsten Konzepte in Mathematik und Informatik. Mit der Verwendung von Variablen fängt das "wahre Programmieren" an." (Rüdeger Baumann)    
Mit dieser Erklärung im Hinterkopf kannst du dir überlegen, wie du Variablen in deinem Programm nutzen kannst, z.B. um den Wert eines Eingangs abzuspeichern. Variablen sind auch nützlich, um an verschiedenen Stellen im Programm immer den gleichen Wert zu verwenden.  

![Schematische Darstellung einer Variablen](/de/brickly/variable.png)  

Als erstes musst Du eine [Variable erstellen](/de/brickly/level-3.md#variableerstellen). Danach hast du Bausteine zur Verfügung, mit denen du die Variable nutzen kannst.    

Außerdem kannst du jetzt verschiedene Programme mit unterschiedlichen Namen speichern. Dazu drückst du das Symbol mit den drei Strichen ganz rechts im Browser. Dann gibst du einen Namen für dein Programm ein, drückst auf "Neu" und schon hast du einen neuen Startbaustein mit einer leeren Arbeitsfläche zur Verfügung. Deine auf dem TXT gespeicherten Programme kannst du mit dem gleichen Symbol auswählen.  

![Neues Programm anlegen](/de/brickly/speichern.png)

## Neue Bausteine bei "Eingänge"    
* `<Spannung (mV)> an Eingang <E1>`: mit dem Eingangsbaustein kannst du einen der Eingänge an dem TXT abfragen. Was dir der Eingang liefert und welche physikalische Größe (*Spannung*, *Schalterzustand*, *Widerstand* oder *Distanz*) du auswählen musst, hängt von dem verwendeten Sensor ab. Du kannst den Eingangsbaustein als Zahlenbaustein verwenden. Bei den Widerständen musst du einen Moment warten, bis sie ihren endgültigen Wert erreicht haben.    
  * Farbsensor: liefert eine elektrische *Spannung*, je nach Farbe unterschiedliche Werte.  
  * IR-Spursensor: wird an zwei Eingänge angeschlossen, liefert an beiden Eingängen einen *Schalterzustand*. Der IR-Spursensor befindet sich über einer einer schwarzen Spur, wenn beide Eingänge den Wert 1 für *ein* liefern.  
  * Taster: liefert einen *Schalterzustand*, entweder 0 für *aus* oder 1 für *ein* (umgekehrt, wenn die Anschlüsse 1 und 2 am Taster verwendet werden).  
  * Fototransistor: liefert einen *Schalterzustand*, 0 für kein Licht oder 1 für Licht, d.h. Lichtschranke offen.  
  * Fotowiderstand: liefert einen *Widerstand*, der mit zunehmender Helligkeit sinkt.
  * Ultraschallsensor: misst die *Distanz*, also den Abstand zum nächsten Hindernis.  
  * Wärmesensor: liefert einen *Widerstand*, der mit steigender Temperatur sinkt.  

![Eingang auslesen](/de/brickly/eingang.png)
  
* `Temperatur <°C>`: diesen Baustein kannst Du verwenden, um aus dem Widerstandswert des Wärmesensor eine Temperatur zu berechnen. Dazu baust du ihn vor den Eingangsbaustein, bei dem du *Widerstand* auswählst. Du kannst die Einheit wählen: °C (Grad Celsius, die in Europa verwendete Einheit), °F (Fahrenheit, wird in den USA verwendet) und K (Kelvin, gibt die absolute Temperatur an).  

## Neue Bausteine bei "Ausgänge"    
* `<100%> (ein)`: mit diesem Baustein kann man wählen, ob der Ausgang mit voller Stärke (100%) oder nur mit weniger Stärke betrieben werden soll. Damit kannst du einen Motor langsamer laufen lassen oder ein Lämpchen weniger hell leuchten lassen.  
* `drehe <rechts> <90°>`<a name="drehegrad"></a>: wie [hier](/de/brickly/level-1.md#drehe). Jetzt kannst du aber den Winkel genau in Grad angeben. Damit du dir unter dem angegeben Winkel etwas vorstellen kannst, erscheint ein kleiner Kreis, auf dem du mit der Maus entlang fahren kannst, um den Winkel einzustellen.     

![Drehwinkel einstellen](/de/brickly/winkel.png)

## Neue Bausteine bei "Logik"     
* `<> <=> <>`: Hier kannst du zwei Werte, z.B. zwei Zahlenbausteine miteinander vergleichen. An die erste Stelle baust du den einen Baustein, dann kannst du den Vergleich auswählen: *=* (gleich), *&ne;* (ungleich), *&lt;* (kleiner als), *&le;* (kleiner oder gleich), *&gt;* (größer als), *&ge;* (größer oder gleich). An die letzte Stelle kommt der zweite Wert. Du kannst Variablen, Text, Zahlen (z.B. von Eingängen) und Wahrheitswerte vergleichen.  

![Vergleich](/de/brickly/vergleich.png)

* `wahr`: ein Bedingungsbaustein, bei dem du *wahr* oder *unwahr* auswählen kannst. Damit kannst du z.B. einer Variablen einen Startwert geben.    

## Neuer Baustein bei "Schleifen"    
* `zähle <i> von <1> bis <10> in Schritten von <1>: mache`: Das ist eine Zählschleife. Die Anzahl der Durchläufe, also wie oft die Befehle im Bauch des Bausteins ausgeführt werden, steht fest. Beim ersten Durchlauf ist der Zähler *i* 1, wird dann um 1 erhöht, usw. bis *i* 10 ist. Mit diesen Zahlen wird diese Schleife also 10 mal ausgeführt. Der Zähler (hier *i*) ist im Bauch des Bausteins bekannt. Du findest einen Zahlenbaustein dafür bei den Variablen. Damit kannst du z.B. zuerst nur 1 Sekunde warten, dann 2 usw..    

![Zählschleife](/de/brickly/zaehlschleife.png)

## Neuer Baustein bei "Mathe"      
* `ganzzahlige Zufallszahl zwischen <1> und <100>`: hier denkt sich der TXT eine ganze Zahl zwischen 1 und 100 aus. Wenn du als Grenzen 1 und 6 wählst, hast du eine Art Würfel.     

## "Variablen"      
* `Variable erstellen`<a name="variableerstellen"></a>: Wenn du auf diesen Baustein gedrückt hast, erscheint ein Fenster, in dem du den Namen deiner Variablen eingibst. Damit ist die Variable erstellt. Wähle einen möglichst aussagekräftigen Namen, unter dem sich auch ein anderer etwas vorstellen kann.  

![Variable erstellen](/de/brickly/variableerstellen.png)

* `setze <meineVariable> auf`: Hier kannst einen Eingangsbaustein oder einen Zahlenbaustein anbauen und damit einen Wert für deine Variable speichern.  
* `erhöhe <meineVariable> um <1>`: mit diesem Baustein kannst du zu dem Wert deiner Variablen 1 oder eine andere Zahl dazuzählen. Das ist praktisch, wenn du Ereignisse zählen willst, z.B. wie oft dein Roboter gegen ein Hindernis gefahren ist.  
* `<meineVariable>`: mit diesem Baustein kannst du deine Variable als Zahlenbaustein verwenden und in anderen Bausteine, z.B. in Textbausteine einbauen.    

![Variablen-Gruppe](/de/brickly/gruppevariablen.png)


## Neu im Kontextmenü    
* "Externe Eingänge": ändert die Darstellung des Bausteins, so dass alle eingebauten Bausteine rechts angebaut sind.   
* "Erzeuge "Schreibe u"": Mit dieser Funktion kannst du sehr schnell das Gegenstück zu dem Baustein erzeugen, z.B. `setze Variable auf`, wenn du auf einer Variablen bist.

