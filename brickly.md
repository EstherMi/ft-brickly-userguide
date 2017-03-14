# Brickly
Brickly ist eine graphische Entwicklungsumgebung für die [Community Edition Firmware](https://github.com/ftCommunity/ftcommunity-TXT) des Fischertechnik TXT. Sie basiert auf Google Blockly.  
# Wozu braucht man Brickly?  
Mit Brickly kannst du im Browser, z.B. auf einem Tablet oder einem PC, graphisch Programme erstellen, die auf dem TXT laufen. Der TXT dient dabei als Webserver, auf den du über WLAN zugreifen kannst. Die Programme können die Eingänge des TXT auslesen und seine Ausgänge, z.B. für Motoren ansteuern.    
Du programmierst mit Brickly, indem du im Browser mit der Maus Bausteine zu einem Programm zusammenfügst. Um dir den Einstieg zu erleichtern, stehen fünf verschiede Erfahrungsgrade zur Verfügung. Die Programme werden auf dem TXT gespeichert, können aber auch (mit der App [BrickMCP](https://github.com/ftCommunity/ftcommunity-apps/blob/master/packages/BrickMCP.zip)) auf andere Rechner übertragen werden.  
# Installation und Start  
Brickly kannst du als [Zip-Datei](https://github.com/harbaum/cfw-apps/blob/master/packages/brickly.zip) vom GitHub-Repository des Autors herunterladen. Zur Installation mussst du den TXT mit der Community Firmware starten. Auf dem Web-Interface siehst du unten einen Bereich "App Upload". Hier wählst du die heruntergeladene Brickly-Zip-Datei aus und drückst dann auf den "Upload"-Knopf. Brickly erscheint nach der Installation in der Liste der installierten Apps.  
## Start im Web-Interface  
Im Web-Interface kannst du Brickly jetzt auswählen. Auf der nächsten Seite kommst du mit "Open local application pages" auf die Seite von Brickly. Damit du mit Brickly programmieren kannst, muss im Browser die Ausführung von JavaScript möglich sein. Auf der Brickly-Seite kannst Du auch die Sprache auswählen, entweder Deutsch oder Englisch (mit den Flaggen-Symbolen rechts oben in der Ecke). Außerdem kannst du dein Brickly-Programm ausdrucken: wenn du auf das Drucker-Symbol rechts oben drückst, erhälst du ein Bild von deinem Programm, das du mit der Druck-Funktion deines Browsers drucken kannst.  
## Benutzung auf dem TXT-Touch-Screen  
![TXT: Brickly](/TXT_Brickly.png)  
Hier siehst du, wie Brickly auf dem TXT-Touch-Screen aussieht. Programmieren kannst du nur in dem Browser auf dem deinem PC oder Tablet. Auf dem TXT kannst du ein Programm auswählen (mit "Select..."). Wenn du auf "Run" drückst, startet das Programm. Wenn du Brickly auf dem TXT beenden willst, drückst du einfach auf das X rechts oben. Wenn du Brickly auf dem TXT beendet hast und das Browserfenster noch offen ist, kannst du durch Drücken auf "Verbinde" rechts im Browser Brickly wieder starten.    
# Arbeiten mit Brickly  
In den folgenden Abschnitten kannst Du für jeden Erfahrungsgrad nachlesen, welche Bausteine dir dir zur Verfügung stehen. Grundlegende Erklärungen gibt es im Abschnitt [Erster Erfahrungsgrad "Anfänger"](#Erster).  
## Erster Erfahrungsgrad "Anfänger"<a name="Erster"></a>  
Oben links auf der Startseite von Brickly siehst du fünf kleine Kreise mit Zahlen. Hier wählst du die 1 aus. Du kommst damit zu dem Erfahrungsgrad "Anfänger".    
Auf der linken Seite siehst Du einige Bausteine, aus denen du dein Programm zusammenbauen kannst. In der Mitte ist deine Arbeitsfläche. Ganz rechts siehst du einen blauen Kasten. Hier wird der Text erscheinen, der von Brickly ausgegeben wird, aber auch Fehlermeldungen, wenn etwas ganz schief laufen sollte.   
In der Arbeitsfläche siehst du schon einen ersten Baustein. Mit diesem Baustein beginnt dein Programm. Ziehe mit der Maus einen Baustein von der linken Seite hierher. Du siehst, dass der Nippel auf der Unterseite gelb aufleuchtet. Jetzt kannst du deinen Baustein hier ablegen. Bei manchen Bausteinen kannst du etwas auswählen. Dazu drückst du auf das kleine blaue Dreieck in dem Auswahlfeld. Wenn du eine Reihe von Bausteinen untereinander zusammengefügt hast, kannst du auf "Los" (über dem blauen Kasten auf der rechten Seite) drücken. Damit wird dein Programm auf den TXT hochgeladen und dort gleich gestartet. Die Befehle auf den Bausteinen werden jetzt von oben nach unten nacheinander abgearbeitet. Wenn das Programm fertig ist, werden alle Ausgänge wieder zurückgesetzt, also z.B. alle Motoren gestoppt.  
### Die Bausteine im Erfahrungsgrad "Anfänger"  
* `gib aus <Text>`<a name="gibaus"></a>Statt *Text* kannst du hier über die Tastatur an deinem Rechner einen anderen Text eingeben. Drücke dazu in das Feld und schreibe deinen Text, z.B. "Hallo TXT". Beende die Eingabe mit der Eingabetaste auf deiner Tastatur oder indem du (mit der Maus) irgendwohin drückst. Der Text erscheint in dem blauen Kasten auf der rechten Seite und auf dem Touchscreen deines TXT.   
* `schalte Ausgang <O1> <aus>`<a name="schalteAusgang"></a>: Mit diesem Baustein kannst du direkt einen Ausgang am TXT ansteuern, um z.B. eine Lampe leuchten zu lassen. Mit *ein* schaltest du den Ausgang ein, mit *aus* wieder aus. Achte darauf, den richtigen Ausgang auszuwählen, also den, an dem du auf dem TXT deine Lampe oder deinen Motor angeschlossen hast. Denk daran, das am Programmende alle Ausgänge wieder ausgeschaltet werden und verwende einen *warte*-Baustein, wenn es nötig ist.    
* `warte <1> Sekunden`<a name="warte"></a>: der TXT macht 1 Sekunde lang nicht mit dem Programm weiter. Du kannst hier auch eine andere Zahl eingeben. Wähle aber keine zu lange Zeit, sonst wird dir langweilig.    
* `wiederhole`<a name="wiederhole"></a>: Wenn du einen Befehl oder eine Gruppe von Befehlen nicht nur einmal, sondern immer wieder ausführen möchtest, verwendest du den *wiederhole*-Baustein. Die Befehlsbausteine schiebst du in den Bauch in dem Wiederhole-Baustein. Jetzt hast du ein Programm, das immer wieder durchläuft. Zum Stoppen des Programms musst du auf den "Stopp"-Knopf drücken. Du findest den "Stopp"-Knopf rechts oben über dem blauen Kasten, da, wo vorher der "Los"-Knopf war.   
* `fahre <vorwärts> <25> cm`<a name="fahre"></a>: Damit kannst du den Fahrroboter aus dem Fischertechnik TXT Discovery Set 25 cm geradeaus vorwärts fahren lassen. Statt *vorwärts* kannst du auch *rückwärts* auswählen, und du kannst eine längere Strecke eingeben. Mehr als 47 cm sind aber nicht möglich.    
* `drehe <rechts> <halb> herum`<a name="drehe"></a>: Damit kannst du den Fahrroboter sich auf der Stelle drehen lassen. Du kannst *rechts* oder *links* auswählen, je nachdem mit welchem Rad sich der Roboter drehen soll. *Rechts* dreht mit dem rechten Rad, so dass sich der Roboter nach links dreht. Außerdem kannst du auswählen, wie weit er sich drehen soll: *etwas* dreht um einen Achtelkreis, *halb* dreht genau zur Seite (einen Viertelkreis), *weit* noch ein Stück weiter, und bei *ganz* guckt der Roboter nach der Drehung genau in die entgegengesetzte Richtung, weil er sich um einen Halbkreis gedreht hat.    

### Kontextmenü    
Wenn du auf die rechte Maustaste drückst, öffnet sich ein Kontextmenü. Hier hast du drei Punkte zur Auswahl:    
* "Kopieren": damit kannst du den ausgewählten Baustein kopieren und die Kopie woanders einbauen.
* "Bausteine löschen": Wenn du den Baustein nicht mehr brauchst, kannst du ihn von deiner Arbeitsfläche entfernen. Keine Angst: auf der linken Seite gibt es ihn noch, so dass du ihn dir wiederholen kannst.    
* "Hilfe": bringt dich zu einer Webseite, die dir weitere Informationen zu dem Baustein liefert.      

## Zweiter Erfahrungsgrad "Junior"    
Als "Junior" hast du mehr Bausteine zur Verfügung. Damit die Auswahl übersichtlich bleibt, sind die Bausteine jetzt in Gruppen aufgeteilt. Es gibt jetzt einen Mülleimer, in den du Bausteine, die du nicht mehr haben willst, schieben kannst. Außerdem kannst du rechts unten die Geschwindigkeit auswählen, mit der der TXT das Programm abarbeiten soll: von Schildkrötengang (ganz langsam) bis zu Hasengang (ganz schnell).  
Neue Bausteine in "Junior" beschäftigen sich mit Bedingungen und Logik. Eine Bedingung ist entweder *wahr* oder *unwahr*. Es gibt für diese Bedingungen beim Programmieren kein "vielleicht" oder "ich weiß nicht". Eine Bedingung in Brickly ist z.B. `Eingang <I1> ist an`. Der Eingang ist an, dann ist die Bedingung wahr, oder aus, dann ist die Bedingung unwahr.   Bedingungsbausteine kannst du an verschiedenen Stellen einsetzen, z.B bei `wiederhole <solange>`.    
### Bausteine "Spezial"    
* `warte <1> Sekunden`: s. [hier](#warte)  
* `spiele Geräusch` und `Flugzeug`: der TXT macht das ausgewählte Geräusch, z.B. *Flugzeug*. Du kannst aus einer ganzen Reihe von Geräuschen auswählen. Den Geräusch-Baustein musst du rechts an den Befehlsbaustein anbauen.   

### Bausteine "Eingänge"        
* `Eingang <I1> ist an`: Dies ist ein Bedingungs-Baustein, der den Zustand des ausgewählten Eingangs, z.B. *I1* abfragt.      

### Bausteine "Ausgänge"    
* `schalte Ausgang <O1>` und `ein`: s. [hier](#schalteAusgang)  
* `fahre <vorwärts> <25> cm`: s. [hier](#fahre)  
* `drehe <rechts> <halb> herum`: s. [hier](#drehe)  
* `fahre <vorwärts> <solange>`<a name="fahresolange"></a>: Mit diesem Baustein kannst du den Fahrroboter solange *vorwärts* oder *rückwärts* fahren lassen, wie ein Zustand dauert, also die angegebene Bedingung wahr ist. Als Zustand kannst du den `Eingang <I1> ist an`-Baustein nehmen, den du rechts an den `fahre <vorwärts> <solange>`-Baustein anbaust. Du kannst an den Eingang I1 einen Taster anschließen, und wenn du den gedrückt hälst, fährt mit diesem Befehl dein Roboter vorwärts. Statt *solange* kannst du auch *bis* auswählen. Damit kannst du einen Hinderniserkennungsroboter bauen, der solange vorwärts fährt, bis ein Hindernis den Taster an dem ausgewählten Eingang drückt.   

### Bausteine "Logik"    
* `falls <> mache `: Nach *falls* kommt eine Bedingung, und in den Bauch des Bausteins nach *mache* kommt ein Befehl oder eine Befehlsblock. Dieser Befehl wird einmal ausgeführt, falls die Bedingung wahr ist. Wenn du auf das Zahnrad links oben in diesem Baustein drückst, kannst du den Baustein noch erweitern. Es öffnet sich ein Kasten, der auf der linken Seite noch zwei Bausteine enthält. Wenn du einen der Bausteine an den 'falls'-Baustein auf der rechten Seite anbaust, erhälst du einen erweiterten 'falls'-Baustein. Wenn du mit dem Zusammenbau fertig bist, drückst du wieder auf das Zahnrad und der Kasten verschwindet. Nach *sonst falls* kannst du noch eine Bedingung und dann wieder einen Befehl einsetzen. Nach *sonst* kommt dann der Befehl, den der TXT ausführen soll, wenn alle anderen Bedingungen in diesem Baustein unwahr sind.     
* `<> <und> <>`: Hier kannst du zwei Bedingungs-Bausteine miteinander zu einer neuen Bedingung verknüpfen. Mit *und* müssen beide Bedingungen wahr sein, damit der Baustein den Wert *wahr* hat. Mit *oder* muss mindestens eine Bedingung wahr sein. Wenn beide Bedingungen unwahr sind, hat der Baustein auch den Wert *unwahr*. Diesen Baustein kannst du immer dort einsetzen, wo eine Bedingung gebraucht wird.  
* `nicht`: diesen Baustein kannst du vor einen Bedingungs-Baustein einbauen, und er dreht diese Bedingung um: aus *wahr* wird *unwahr* und aus *unwahr* wird *wahr*.    

### Bausteine "Schleifen"    
* `wiederhole`: s. [hier](#wiederhole)  
* `wiederhole <10> mal: mache`: Hier gibst du die Anzahl der Wiederholungen an. Dein TXT führt dann die Befehle in dem Bauch des Bausteins 10 mal nacheinander aus. Du kannst auch eine andere Zahl eingeben.  
* `wiederhole <solange>`: Hier gibst du eine Bedingung für die Wiederholung an. Wenn du *solange* auswählst, werden die Befehle nur dann ausgeführt, wie eine Bedingung wahr ist, dann aber immer wieder. Du kannst auch *bis* auswählen. Dann werden die Befehle so lange immer wieder ausgeführt, wie die angebene Bedingung wahr ist.    

### Bausteine "Mathe"      
* `<0>`: ein Zahlenbaustein. Statt 0 kannst du eine andere Zahl eingeben. Diesen Baustein kannst du überall dort verwenden, wo eine Zahl gebraucht wird.   
* `<1> <+> <1>`: ein Zahlenbaustein mit Rechenergebnis. Es gibt plus (+), minus (-), mal (x), geteilt (&divide;), hoch (^).     

### Bausteine "Text"     
* `"< >"`: ein Textbaustein, den du über die Tastatur mit Text füllen kannst.   
* `erstelle Text aus`: setzt zwei Texte zu einem Text zusammen.   
* `gib aus "< >"`: wie [hier](#gibaus). Du kannst hier einen Text eingeben, oder einen Textbaustein oder einen Zahlenbaustein einbauen. Wenn du einen Bedingungsbaustein anbaust, wird "true" für *wahr* oder "false" für unwahr ausgegeben.     

### Neu im Kontextmenü
* "Kommentar hinzufügen":  Hier kannst du einen Kommentar zu deinem Baustein oder dem Programm schreiben oder auch wieder löschen. Wenn du den Kommentar fertig geschrieben hast oder zum Lesen eines Kommentares, drückst du auf das kleine Fragezeichen.  
* "Baustein zusammenfalten": Damit wird ein Baustein zusammengefaltet und platzsparender dargestellt. Du kannst ihn auch wieder entfalten.   
* "Baustein deaktivieren": deaktiviert den Baustein, so dass er nicht mehr im Programm verwendet wird. Aktivieren macht das wieder rückgängig.    

## Dritter Erfahrungsgrad "Fortgeschritten"    
Für die Fortgeschrittenen gibt es neue Bausteine für die Nutzung der Eingänge, und du lernst Variablen kennen.   
"Variablen sind Behälter im Speicher, die einen Namen haben und deren Inhalt sich während der Ausführung eines Programms ändern kann. Der Begriff der Variablen ist eines der wichtigsten Konzepte in Mathematik und Informatik. Mit der Verwendung von Variablen fängt das "wahre Programmieren" an." (Rüdeger Baumann)    
Mit dieser Erklärung im Hinterkopf kannst du dir überlegen, wie du Variablen in deinem Programm nutzen kannst, z.B. um den Wert eines Eingangs abzuspeichern. Variablen sind auch nützlich, um an verschiedenen Stellen im Programm immer den gleichen Wert zu verwenden.  
Als erstes musst Du eine Variable erstellen. Danach hast du Bausteine zur Verfügung, mit denen du die Variable nutzen kannst.    
Außerdem kannst du jetzt verschiedene Programme mit unterschiedlichen Namen speichern. Dazu drückst du das Symbol mit den drei Strichen ganz rechts im Browser. Dann gibst du einen Namen für dein Programm ein, drückst auf "Neu" und schon hast du einen neuen Startbaustein mit einer leeren Arbeitsfläche zur Verfügung. Deine auf dem TXT gespeicherten Programme kannst du mit dem gleichen Symbol auswählen.  
### Neue Bausteine bei "Eingänge"    
* `<Spannung (mV)> an Eingang <E1>`: mit dem Eingangsbaustein kannst du einen der Eingänge an dem TXT abfragen. Was dir der Eingang liefert und welche physikalische Größe (*Spannung*, *Schalterzustand*, *Widerstand* oder *Distanz*) du auswählen musst, hängt von dem verwendeten Sensor ab. Du kannst den Eingangsbaustein als Zahlenbaustein verwenden.    
  * Farbsensor: liefert eine elektrische *Spannung*, je nach Farbe unterschiedliche Werte  
  * IR-Spursensor: wird an zwei Eingänge angeschlossen, liefert an beiden Eingängen eine elektrische *Spannung*. Der IR-Spursensor befindet sich über einer einer schwarzen Spur, wenn an beiden Eingängen eine niedrige Spannung anliegt.  
  * Taster: liefert einen *Schalterzustand*, entweder 0 für *aus* oder 1 für *ein* (umgekehrt, wenn die Anschlüsse 1 und 2 am Taster verwendet werden).  
  * Fototransistor: liefert einen *Schalterzustand*, 0 für kein Licht oder 1 für Licht, d.h. Lichtschranke offen.  
  * Ultraschallsensor: misst die *Distanz*, also den Abstand zum nächsten Hindernis.  
  * Wärmesensor: liefert einen *Widerstand*, der mit steigender Temperatur sinkt.  
* `Temperatur <°C>`: diesen Baustein kannst Du verwenden, um aus dem Widerstandswert des Wärmesensor eine Temperatur zu berechnen. Dazu baust du ihn vor den Eingangsbaustein, bei dem du *Widerstand* auswählst. Du kannst die Einheit wählen: °C (Grad Celsius, die in Europa verwendete Einheit), °F (Fahrenheit, wird in den USA verwendet) und K (Kelvin, gibt die absolute Temperatur an).  

### Neue Bausteine bei "Ausgänge"    
* `<100%> (ein)`: mit diesem Baustein kann man wählen, ob der Ausgang mit voller Stärke (100%) oder nur mit weniger Stärke betrieben werden soll. Damit kannst du einen Motor langsamer laufen lassen oder ein Lämpchen weniger hell leuchten lassen.  
* `drehe <rechts> <90°>`<a name="drehegrad"></a>: wie [hier](#drehe). Jetzt kannst du aber den Winkel genau in Grad angeben. Damit du dir unter dem angegeben Winkel etwas vorstellen kannst, erscheint ein kleiner Kreis, auf dem du mit der Maus entlang fahren kannst, um den Winkel einzustellen.     

### Neue Bausteine bei "Logik"     
* `<> <=> <>`: Hier kannst du zwei Werte, z.B. zwei Zahlenbausteine miteinander vergleichen. An die erste Stelle baust du den einen Baustein, dann kannst du den Vergleich auswählen: *=* (gleich), *&ne;* (ungleich), *&lt;* (kleiner als), *&le;* (kleiner oder gleich), *&gt;* (größer als), *&ge;* (größer oder gleich). An die letzte Stelle kommt der zweite Wert. Du kannst Variablen, Text, Zahlen (z.B. von Eingängen) und Wahrheitswerte vergleichen.  
* `wahr`: ein Bedingungsbaustein, bei dem du *wahr* oder *unwahr* auswählen kannst. Damit kannst du z.B. einer Variablen einen Startwert geben.    

### Neuer Baustein bei "Schleifen"    
* `zähle <i> von <1> bis <10> in Schritten von <1>: mache`: Das ist eine Zählschleife. Die Anzahl der Durchläufe, also wie oft die Befehle im Bauch des Bausteins ausgeführt werden, steht fest. Beim ersten Durchlauf ist der Zähler *i* 1, wird dann um 1 erhöht, usw. bis *i* 10 ist. Mit diesen Zahlen wird diese Schleife also 10 mal ausgeführt. Der Zähler (hier *i*) ist im Bauch des Bausteins bekannt. Du findest einen Zahlenbaustein dafür bei den Variablen. Damit kannst du z.B. zuerst nur 1 Sekunde warten, dann 2 usw.    

### Neuer Baustein bei "Mathe"      
* `ganzzahlige Zufallszahl zwischen <1> und <100>`: hier denkt sich der TXT eine ganze Zahl zwischen 1 und 100 aus. Wenn du als Grenzen 1 und 6 wählst, hast du eine Art Würfel.     

### "Variablen"      
* `Variable erstellen`: Wenn du auf diesen Baustein gedrückt hast, erscheint ein Fenster, in dem du den Namen deiner Variablen eingibst. Damit ist die Variable erstellt. Wähle einen möglichst aussagekräftigen Namen, unter dem sich auch ein anderer etwas vorstellen kann.  
* `setze <meineVariable> auf`: Hier kannst einen Eingangsbaustein oder einen Zahlenbaustein anbauen und damit einen Wert für deine Variable speichern.  
* `erhöhe <meineVariable> um <1>`: mit diesem Baustein kannst du zu dem Wert deiner Variablen 1 oder eine andere Zahl dazuzählen. Das ist praktisch, wenn du Ereignisse zählen willst, z.B. wie oft dein Roboter gegen ein Hindernis gefahren ist.  
* `<meineVariable>`: mit diesem Baustein kannst du deine Variable als Zahlenbaustein verwenden und in anderen Bausteine, z.B. in Textbausteine einbauen.    

### Neu im Kontextmenü    
* "Externe Eingänge": ändert die Darstellung des Bausteins, so dass alle eingebauten Bausteine rechts angebaut sind.   
* "Erzeuge "Schreibe u"": Mit dieser Funktion kannst du sehr schnell das Gegenstück zu dem Baustein erzeugen, z.B. `setze Variable auf`, wenn du auf einer Variablen bist.

## Vierter Erfahrungsgrad "Senior"    
In diesem Erfahrungsgrad gibt es viele neue Bausteine für die Nutzung von Encoder-Motoren. Alle Motorbausteine findest du jetzt in einer eigenen Untergruppe "Motoren" unterhalb von "Ausgänge".    
Außerdem kannst du jetzt eine Gruppe von Befehlen zu einer Funktion zusammenbauen. Damit wird ein langes Programm viel übersichtlicher.    

### "Ausgänge" - "Motoren"    
* `setze Motor <M1> <Geschwindigkeit> auf`: mit diesem Baustein kannst du den ausgewählten Motor  (M1, M2, M3 oder M4) genau ansteuern. Je nach ausgewählter Eigenschaft (*Geschwindigkeit*, *Richtung*, *Entfernung*, *Typ*) musst du noch einen der folgenden drei Bausteine anbauen. Für die *Entfernung* baust du noch einen Zahlenbaustein an. Die Geschwindigkeit musst du für jeden Motor auf jeden Fall angeben, sonst bewegt er sich nicht. **Wichtig**: Wenn der Motor gestartet ist, läuft das Programm weiter. Wenn es am Ende angekommen ist, werden alle Motoren ausgeschaltet. Es kann daher sein, dass der Motor anhält, bevor er die angegebene Entfernung zurückgelegt hat. Du musst also deinem Motor Zeit geben, wenn er eine bestimmte Entfernung zurücklegen soll, z.B. in dem du einen `warte`-Baustein einbaust.  
* `<links>`: gibt die *Richtung* an, in die sich der Motor drehen soll.  
* `<neuer Encodermotor (TXT)>`: entweder *neuer Encodermotor* oder *alter Encodermotor*. Der Typ des Encodermotors ist wichtig, wenn du die Entfernung angibst. Die beiden Motoren unterscheiden sich nämlich in der Anzahl der Impulse pro Umdrehung der Antriebswelle. Wenn du den *Typ* deines Motors richtig setzt, wird dieser Unterschied berücksichtigt.  
* `<100% (ein)`: gibt die *Geschwindigkeit* an.  
* `stoppe Motor <M1>`: stoppt den ausgewählten Motor.  
* `Motor <M1> hat gestoppt`: dieser Bedingungsbaustein wird wahr, wenn der Motor angehalten hat, weil die angegebene Entfernung erreicht wurde.  
* `kopple Motoren <M1> und <M2>`: zwei gekoppelte Motoren laufen gleichzeitig und mit gleicher Geschwindigkeit. Damit beide Motoren wirklich synchron laufen und auch zur gleichen Zeit ein Stopp-Signal geben, solltest Du bei beiden Motoren die gleiche Entfernung einstellen. Die Motoren können aber in unterschiedliche Richtung drehen: dann dreht sich der Fahrroboter.  
* `fahre <vorwärts> <25> cm`: wie [hier](#fahre)  
* `fahre <vorwärts> <solange>`: wie [hier](#fahresolange)  
* `drehe <rechts> <90>`: wie [hier](#drehegrad)    

### Neu in "Schleifen"       
* `<die Schleife abbrechen>`: mit diesem Baustein kannst du den Durchlauf durch eine Schleife abbrechen. Das Programm springt dann sofort zu dem ersten Baustein nach der Schleife. Du kannst diesen Baustein nach einer Bedingung in einer Schleife einbauen, um z.B. in einer Zählschleife im Notfall abzubrechen. Du kannst auch auswählen *sofort mit dem nächsen Schleifendurchlauf fortfahren*, wenn in einer Schleife einige Befehle unter bestimmten Bedingungen nicht ausgeführt werden sollen. **Wichtig**: beide Bausteine funktionieren nicht bei der "Wiederhole"-Schleife (die ohne "solange", "bis" oder "10 mal"). Die ist eine Endlosschleife, die nur mit einem Drücken auf "Stopp" abgebrochen werden kann.    

### Neu in "Mathe"       
* `<Quadratwurzel>` berechnet die ausgewählte mathematische Funktion (*Quadratwurzel*, *Betrag*, *-*, *ln*, *log10*, *e^* oder *10^*) aus dem angebauten Zahlenbaustein.    
* `Rest von <> ÷ <>`: berechnet den Rest der Division der 1. Zahl durch die 2. Zahl (Modulo-Funktion). Ein Beispiel: Bei einer geraden Zahl ist der Rest der Division durch 2 gleich 0. Damit kannst du in einer Schleife einen Befehl nur in jedem zweiten Durchlauf ausführen.    

### Neu in "Text"    
* `an <etwas> Text anhängen`: hängt an die Variable *etwas* oder eine andere ausgewählte Variable den Inhalt des angehängten Textbausteines an.     

### "Funktionen"    
* `etwas tun`: Damit definierst du deine Funktion. Du legst den Baustein einfach auf der Arbeitsfläche ab. In den Bauch baust du die Befehlsbausteine, die deine Funktion ausführen soll. Statt *etwas tun* solltest du der Funktion einen sinnvollen Namen geben. Du kannst zusätzlich noch einen Text schreiben, der die Funktion beschreibt, wenn du auf das kleine Fragezeichen neben dem Namen drückst. Wenn du den Funktionsbaustein auf der Arbeitsfläche abgelegt hast, findest du in dieser Gruppe auch einen Baustein mit dem Namen deiner Funktion. Das ist der Funktionsaufruf. Diesen Baustein baust du in dein Programm ein. Damit wird deine Funktion aufgerufen, d.h. die Befehle im Bauch des Funktionsbausteins werden ausgeführt. Du kannst der Funktion auch einen oder mehrere Parameter hinzufügen. Das ist ein Wert, den das Programm der Funktion beim Aufruf übergibt und den du innerhalb der Funktion nutzen kannst. Dazu drückst du auf das kleine Zahnrad links oben in dem Funktionsbaustein und ziehst dann den Baustein *Variable* in den Bauch des Funktionsbausteins auf der rechten Seite des Kastens. Gib auch den Parametern sinnvolle Namen! Beim Aufruf musst du dann einen passenden Wertbaustein an den Aufruf anbauen.  
* `etwas tun: gib zurück:` Diese Funktion kann nicht nur einfach Befehle ausführen, sondern auch einen Wert zurückgeben (z.B. den Messwert eines Sensors). Den Funktionsbaustein verwendest du dann beim Aufruf wie einen Wertbaustein. Auch dieser Funktion kannst du Parameter hinzufügen.  
* `falls: gib zurück:`: Dieser Block darf nur innerhalb eines Funktionsblocks genutzt werden. Nach *falls* kommt eine Bedingung. Wenn diese Bedingung *wahr* ist, beendet sich die Funktion sofort und gibt den angegebenen Wert zurück. Damit kannst du z.B. eine Fehlermeldung zurückgeben, wenn etwas schief gelaufen ist.    

## Fünfter Erfahrungsgrad "Experte"    
Dies ist der höchste Erfahrungsgrad für die Experten. Neu sind hier die Listen-Bausteine. Eine Liste ist eine durchnummerierte Reihe von Elementen. Über die Nummer kannst du auf jedes Element zugreifen. Die meisten Bausteine für Listen findest du in der neuen Gruppe "Listen", es gibt aber auch einen neuen Baustein unter "Schleifen" und einen bei "Mathe".      
### Neue Bausteine in "Eingänge"    
Hier gibt es einige neue Bausteine für die Nutzung eines USB-Joysticks. Die Joysticks/Gamepads werden per USB am TXT angeschlossen - am Standard-USB-Port. Zur Zeit funktionieren leider nur einige Typen, z.B. ein Speedlink Competition Pro USB Joystick.    

### Neu in "Ausgänge"    
* `gleichzeitig`. Mit diesem Baustein kannst du Ausgänge gleichzeitig setzen, z.B. zwei Motoren gleichzeitig starten, ohne gekoppelte Encodermotoren zu verwenden. Der Baustein funktioniert nicht mit den Bausteinen aus der Untergruppe "Mobil" (da drehen zwei Motoren ohnehin gleichzeitig).     

### Neue Untergruppe in "Ausgänge": "Mobil"    
* `fahre <vorwärts> <25> cm`: wie [hier](#fahre)  
* `fahre <vorwärts> <solange>`: wie [hier](#fahresolange)  
* `drehe <rechts> <90>`: wie [hier](#drehegrad)  
* `<90>°` und `<etwas> herum`: diese beiden Bausteine können an den `drehe`-Baustein angebaut werden, um den Drehwinkel einzustellen.    
* `Mobilroboter-Konfiguration`: Wenn du einen anderen Fahrroboter als den aus dem TXT-Discovery-Set gebaut hast, kannst du mit diesem Baustein am Anfang deines Programms einstellen, an welchen Anschlüssen die Motoren angeschlossen sind, von welchem Typ sie sind, wie die Antriebsübersetzung (Motorachse zu Radachse) ist, wie groß der Raddurchmesser ist und wie der Abstand zwischen den Antriebsrädern ist. Mit der richtigen Konfiguration sollen die Befehle zum Fahren und Drehen auch für deinen selbstkonstruierten Fahrroboter funktionieren. Für das Discovery-Set wird dieser Baustein nicht benötigt.      

### Neu in "Logik"       
* `null`: der Wert, den eine Variable hat, die zwar einen Namen hat, aber für die kein Wert gesetzt wurde.  
* `prüfe: falls wahr: falls unwahr:`: ein Wertbaustein, mit dem man den Wert auswählen kann. Nach *prüfe* kommt eine Bedingung. Wenn diese *wahr* ist, wird der Wert zurückgegeben, der nach *falls wahr* steht, sonst der Wert nach *falls unwahr*. (In der Informatik heißt das auch "Tenärer Operator" oder "Auswahloperator").       

### Neu in "Schleifen"       
* `für jeden Wert <i> aus der Liste: mache:` diese Schleife arbeitet sich von vorne bis hinten durch die Liste durch. Im Bauch der Schleife kannst du mit dem aktuellen Element (es heißt *i*) Befehle ausführen. Diese Befehle ändern die Liste selbst aber nicht.     

### Neu in "Mathe"     
* `<sin> <45>` stellt die Winkelfunktionen *sin*, *cos* und *tan* und die Arkusfunktionen *asin*, *acos* und *atan* zur Verfügung.  
* `<π>`: liefert die ausgewählte mathematische Konstante: die Kreiszahl π, die Eulersche Zahl e, den Goldenen Schnitt φ, die Quadratwurzel von 2 sqrt(2), die Quadratwurzel von 1/2 sqrt(1/2) oder unendlich ∞.  
* `<0> ist <gerade>`: ein Bedingungsbaustein, der prüft, ob die Zahl (hier 0) die ausgewählte Eigenschaft hat: *gerade*, *ungerade*, *eine Primzahl*, *eine ganze Zahl*, *positiv*, *negativ* oder *teilbar durch* (braucht noch eine 2. Zahl).
* `<runde> <3.1>` rundet die angegebene Zahl. Du kannst auch *runde auf* (aufrunden zur nächstgrößeren ganzen Zahl) oder *runde ab* (abrunden zur nächst kleineren ganzen Zahl) wählen.  
* `<Summe über die> Liste: ` gibt die Summe aller Elemente der ausgewählten Liste aus. Du kannst eine andere Funktionen auswählen, die dann eine andere Berechnung über alle Elemente durchführt (*Minimalwert*, *Maximalwert*, *Mittelwert*, *Median*, *am häufigsten*, *Standardabweichung*, *Zufallswert*).  
* `begrenze <50> zwischen <1> und <100>`: verwendet die angegebene Zahl (hier 50), wenn sie zwischen den beiden anderen Zahlen liegt. Wenn sie zu groß ist, wird die obere Grenze genommen (hier 100), und wenn wenn sie zu klein ist, die untere Grenze (hier 1). Sinnvollerweise nimmt man als Zahl hier eine Zahlenvariable.  
* `Zufallszahl (0.0 - 1.0)`: liefert eine zufällige Gleitkommazahl zwischen 0.0 und 1.0.     

### Neu in "Text"    
Hier findest du jetzt viele neue Bausteine, um Texte zu bearbeiten, Teile daraus zu finden usw. Als "Experte" wirst du in dieser Gruppe finden, was du brauchst. Ein Baustein ist besonders nützlich.  
* `gib aus in <> <"abc">`: gibt den angegebenen Text in der ausgewählten Farbe aus.    

### "Listen"    
Um eine Liste zu erzeugen, erstellst du am einfachsten zuerst eine Variable für die Liste (z.B. "MeineListe"). Dann erzeugst du eine Liste mit einem der folgenden Bausteine und weist ihn der Variable zu. Die Variable mit deiner Liste findest du unter "Variablen".  
* `erzeuge eine leere Liste`: erzeugt eine leere Liste.  
* `erzeuge eine Liste mit: `: erzeugt eine Liste aus den angegeben Bausteinen. Durch Drücken auf das Zahnrad erhälst du wieder einen Kasten, mit dem du durch Hinzufügen oder Zurückschieben der Elementbausteine (*etwas*) mehr oder weniger Elementplätze in deiner Liste bereitstellen kannst. Wenn du die richtige Anzahl hast, drückst du wieder auf das Zahnrad. Um deine Liste zu füllen, baust du an die freien Plätze Wert-Bausteine an, z.B. Variablen, Zahlen oder Texte.  
* `erzeuge eine Liste mit <5> mal dem Element <>`: erzeugt eine Liste mit der angegebenen Länge (hier 5), die an jeder Stelle das gleiche Element enthält.  
* `Länge von: `: gibt die Länge der angebauten Liste (d.h. die Anzahl der Elemente) als Zahl aus.  
* `<> ist leer`: ein Bedingungsbaustein, liefert wahr, wenn die eingebaute Liste leer ist, d.h. keine Elemente enthält.  
* `in der Liste <Liste> suche <erstes> Auftreten von <>`: gibt die *erste* (oder *letzte*) Position zurück, an der sich das angegeben Element befindet. Der Wert ist 0, wenn kein passendes Element in der Liste ist.  
* `in der Liste <Liste> <nimm> <#tes> <>`: liefert das Element an der angegebenen Position (Zahl nach *#tes*) in der Liste. Du kannst auch auswählen *nimm und entferne*, dann wird das zurückgelieferte Element aus der Liste gelöscht, die Liste wird kürzer. Mit *entferne* wird auch das angegebene Element gelöscht, aber du erhälst keinen Wert zurück. Du kannst statt von vorne auch von hinten zählen (*#tes von hinten*), oder *erstes*, *letztes* oder *zufälliges* Element wählen. Achte darauf, dass die Postionsangabe einen Wert zwischen 1 und der Länge deiner Liste ergibt, sonst gibt das Programm eine Fehlermeldung.  
* `in der Liste <Liste> <setze für> <#tes> ein <>`: hier kannst du das Element an der angegebenen Position überschreiben, oder mit *füge ein* ein neues Element einbauen. Beim Einfügen wird die Liste länger.  
* `in der Liste <Liste> erhalte Unterliste <von #> <> bis <zu #> <>`: gibt alle Elemente zwischen den ausgewählten Positionen aus. Wenn die zweite Position vor der ersten liegt, ist die Unterliste leer.  
* `<Liste aus Text> erstellen <> mit Trennzeichen <",">`: erstellt eine Liste von Texten aus einem längeren Text, wobei die einzelnen Teile durch das angegebene Zeichen, z.B. ein Komma, getrennt sind.  
* `<nummerisch> <aufsteigend> <> sortieren`: liefert eine sortierte (*nummerisch*, *alphabetisch* (mit Großbuchstaben zuerst) oder *alphabetisch, Großschreibung ignorieren*) Kopie der angegebenen Liste. Die Liste selbst bleibt unverändert. Wenn die sortierte Kopie behalten möchtest, musst du die Variablenzuweisung `setze <meineVariable> auf` und diesen Baustein verwenden.
