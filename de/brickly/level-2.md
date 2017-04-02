# Zweiter Erfahrungsgrad "Junior"    

Als "Junior" hast du mehr Bausteine zur Verfügung. Damit die Auswahl übersichtlich bleibt, sind die Bausteine jetzt in Gruppen aufgeteilt.

![Gruppen](/de/brickly/gruppen.png)

Es gibt jetzt einen Mülleimer, in den du Bausteine, die du nicht mehr haben willst, schieben kannst. Außerdem kannst du rechts unten die Geschwindigkeit auswählen, mit der der TXT das Programm abarbeiten soll: von Schildkrötengang (ganz langsam) bis zu Hasengang (ganz schnell).  
Neue Bausteine in "Junior" beschäftigen sich mit Bedingungen und Logik. Eine Bedingung ist entweder *wahr* oder *unwahr*. Es gibt für diese Bedingungen beim Programmieren kein "vielleicht" oder "ich weiß nicht". Eine Bedingung in Brickly ist z.B. `Eingang <I1> ist an`. Der Eingang ist an, dann ist die Bedingung wahr, oder aus, dann ist die Bedingung unwahr.   Bedingungsbausteine kannst du an verschiedenen Stellen einsetzen, z.B bei `wiederhole <solange>`.  

## Bausteine "Spezial"    
* `warte <1> Sekunden`: s. [hier](/de/brickly/level-1.md#warte)  
* `spiele Geräusch` und `Flugzeug`: der TXT macht das ausgewählte Geräusch, z.B. *Flugzeug*. Du kannst aus einer ganzen Reihe von Geräuschen auswählen. Den Geräusch-Baustein musst du rechts an den Befehlsbaustein anbauen.   

## Bausteine "Eingänge"        
* `Eingang <I1> ist an`: Dies ist ein Bedingungs-Baustein, der den Zustand des ausgewählten Eingangs, z.B. *I1* abfragt.      

## Bausteine "Ausgänge"    
* `schalte Ausgang <O1>` und `ein`: s. [hier](/de/brickly/level-1.md#schalteAusgang)  
* `fahre <vorwärts> <25> cm`: s. [hier](/de/brickly/level-1.md#fahre)  
* `drehe <rechts> <halb> herum`: s. [hier](/de/brickly/level-1.md#drehe)  
* `fahre <vorwärts> <solange>`<a name="fahresolange"></a>: Mit diesem Baustein kannst du den Fahrroboter solange *vorwärts* oder *rückwärts* fahren lassen, wie ein Zustand dauert, also die angegebene Bedingung wahr ist. Als Zustand kannst du den `Eingang <I1> ist an`-Baustein nehmen, den du rechts an den `fahre <vorwärts> <solange>`-Baustein anbaust. Du kannst an den Eingang I1 einen Taster anschließen, und wenn du den gedrückt hälst, fährt mit diesem Befehl dein Roboter vorwärts. 

![fahre vorwärts solange Eingang I1 ist an](/de/brickly/solange.png)

Statt *solange* kannst du auch *bis* auswählen. Damit kannst du einen Hinderniserkennungsroboter bauen, der solange vorwärts fährt, bis ein Hindernis den Taster an dem ausgewählten Eingang drückt.   

## Bausteine "Logik"    
* `falls <> mache `: Nach *falls* kommt eine Bedingung, und in den Bauch des Bausteins nach *mache* kommt ein Befehl oder eine Befehlsblock. Dieser Befehl wird einmal ausgeführt, falls die Bedingung wahr ist.    
Wenn du auf das Zahnrad links oben in diesem Baustein drückst, kannst du den Baustein noch erweitern. Es öffnet sich ein Kasten, der auf der linken Seite noch zwei Bausteine enthält. Wenn du einen der Bausteine an den 'falls'-Baustein auf der rechten Seite anbaust, erhälst du einen erweiterten 'falls'-Baustein. Wenn du mit dem Zusammenbau fertig bist, drückst du wieder auf das Zahnrad und der Kasten verschwindet. Nach *sonst falls* kannst du noch eine Bedingung und dann wieder einen Befehl einsetzen. Nach *sonst* kommt dann der Befehl, den der TXT ausführen soll, wenn alle anderen Bedingungen in diesem Baustein unwahr sind.     

![wenn sonst falls](/de/brickly/sonstfalls.png)

* `<> <und> <>`: Hier kannst du zwei Bedingungs-Bausteine miteinander zu einer neuen Bedingung verknüpfen. Mit *und* müssen beide Bedingungen wahr sein, damit der Baustein den Wert *wahr* hat. 

![und](/de/brickly/und.png)

Mit *oder* muss mindestens eine Bedingung wahr sein. Wenn beide Bedingungen unwahr sind, hat der Baustein auch den Wert *unwahr*. Diesen Baustein kannst du immer dort einsetzen, wo eine Bedingung gebraucht wird.  
* `nicht`: diesen Baustein kannst du vor einen Bedingungs-Baustein einbauen, und er dreht diese Bedingung um: aus *wahr* wird *unwahr* und aus *unwahr* wird *wahr*.    

## Bausteine "Schleifen"    
* `wiederhole`: s. [hier](/de/brickly/level-1.md#wiederhole)  
* `wiederhole <10> mal: mache`: Hier gibst du die Anzahl der Wiederholungen an. Dein TXT führt dann die Befehle in dem Bauch des Bausteins 10 mal nacheinander aus. Du kannst auch eine andere Zahl eingeben.  
* `wiederhole <solange>`: Hier gibst du eine Bedingung für die Wiederholung an. Wenn du *solange* auswählst, werden die Befehle nur dann ausgeführt, wie eine Bedingung wahr ist, dann aber immer wieder. Du kannst auch *bis* auswählen. Dann werden die Befehle so lange immer wieder ausgeführt, wie die angebene Bedingung wahr ist.    

## Bausteine "Mathe"      
* `<0>`: ein Zahlenbaustein. Statt 0 kannst du eine andere Zahl eingeben. Diesen Baustein kannst du überall dort verwenden, wo eine Zahl gebraucht wird.   
* `<1> <+> <1>`: ein Zahlenbaustein mit Rechenergebnis. Es gibt plus (+), minus (-), mal (x), geteilt (&divide;), hoch (^).     

## Bausteine "Text"     
* `"< >"`: ein Textbaustein, den du über die Tastatur mit Text füllen kannst.   
* `erstelle Text aus`: setzt zwei Texte zu einem Text zusammen.   
* `gib aus "< >"`: wie [hier](/de/brickly/level-1.md#gibaus). Du kannst hier einen Text eingeben, oder einen Textbaustein oder einen Zahlenbaustein einbauen. Wenn du einen Bedingungsbaustein anbaust, wird "true" für *wahr* oder "false" für unwahr ausgegeben.     

## Neu im Kontextmenü
* "Kommentar hinzufügen":  Hier kannst du einen Kommentar zu deinem Baustein oder dem Programm schreiben oder auch wieder löschen. Wenn du den Kommentar fertig geschrieben hast oder zum Lesen eines Kommentares, drückst du auf das kleine Fragezeichen.

![Kommentar](/de/brickly/kommentar.png)
  
* "Baustein zusammenfalten": Damit wird ein Baustein zusammengefaltet und platzsparender dargestellt. Du kannst ihn auch wieder entfalten.   

![Zusammengefalteter Baustein](/de/brickly/gefaltet.png)

* "Baustein deaktivieren": deaktiviert den Baustein, so dass er nicht mehr im Programm verwendet wird. Aktivieren macht das wieder rückgängig.    

