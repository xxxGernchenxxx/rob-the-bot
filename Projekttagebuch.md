Diese Seite ist das Projekttagebuch. Hier werden alle Tage, an denen am Projekt gearbeitet wurde, mit einer kurzen Beschreibung erwähnt.

<h1>Bau einer automatischen Lego-Sortiermaschine mit einem Arduino</h1>

<h3> Inhalt </h3>
<ul style="list-stlye-type:none">
<li><a href="#kapitell">1. Einleitung</a></h2></li>
<li><a href="#kapitel2">2. Stundenprotokoll</a></h2></li>
<li><a href="#kapitel3">3. Materialien</a></h2></li>
<li><a href="#kapitel4">4. Quellen</a></h2></li>
<br>
<h2 id="kapitell">1. Einleitung</h2>
<p>In kürze wird hier die Einleitung stehen!<br></p>

<h3 id="kapitel2">2. Stundenprotokoll</a></h2></li>

<b>Dienstag, der 14.12.2021</b><br>

  Nachdem das letzte Projekt abgeschlossen war, fing direkt ein neues an. Schon vor dem Projektbeginn hatte ich mir gewünscht einen Roboter zu bauen. Diese Überlegungen waren jedoch nicht sehr weit fortgeschritten. Über die Ferien möchte ich mir dazu Gedanken machen. In der letzten Doppelstunde vor den Ferien haben wir dann nicht an Informatik weitergearbeitet, sondern haben ein Spiel Namens "Secret Hitler" in der Klasse gespielt.<br></p>
  
  
<b>Mittwoch, der 15.12.2021</b><br>

  Diese Stunde ist ausgefallen, weil es der letzte Tag vor den Ferien war und wir somit nach der 3. Stunde Schluss hatten.<br></p>


<b>Dienstag, der 11.01.2022</b><br>

  In dieser ersten Doppelstunde des neuen Jahres habe ich bei GitHub angfangen, das neue Projekt zu erstellen. Dazu habe ich ein neues Repository erstellt und eine File eingefügt, in der ich nun das Projekttagebuch erstelle. Hier werden jegliche Arbeitsschritte dokumentiert.
Während der Ferien und heute habe ich weiter über die Idee eines Roboters und dessen Funktionen nachgedacht. Dabei bin ich auf einen Farbsensor im Internet gestoßen, der interassente Anwendungsmöglichkeiten zulässt. Für einen Roboter bin ich nicht merklich weitergekommen, weil die Umsetzung des Fahrwerks mit Rädern oder Ketten schwierig ist und auch die praxisnahen Funktionen nicht einfach zu programmieren sind. Deshalb habe ich mich gegen den Bau eines Roboters entschieden. Bei Recherchen im Internet zu Farbsensoren und anderen technischen Komponenten bin ich auf eine Sortiermaschine für bunte Schokolinsen gestoßen. Diese Idee finde ich sehr interessant und außergwöhnlich. Zudem scheint die Umsetzung nicht besonders schwierig, sodass ich mich nun auch auf eine Sortiermaschine konzentrieren möchte, die allerdings Legosteine nach Farben sortiert.<br></p> 


<b>Mittwoch, der 12.01.2022</b><br>

  Nachdem ich mich letzte Stunde gegen den Bau eines Roboters entschieden habe und nun eine Sortiermaschine basteln möchte, habe ich an dieser Idee weitergearbeitet. Die Maschine soll möglichst Legosteine nach Farbe sortieren und dann, wenn möglich auch noch nach Größe. Das Funktionsprinzip dieser Schritte habe ich mir heute weiter überlegt.<br></p>
  
  
<b>Dienstag, der 18.01.2022</b><br>

  Heute habe ich mich primär mit der Thematik beschäftigt, welcher Farbsensor verwendet werden soll und wie die Legosteine zu dem Farbsensor gelangen, sodass sie richtig zugeordnet werden können. Das umfasst nicht nur die Problematik, dass die Legosteine nur einzeln in dem Bereich des Farbsensors sein dürfen, damit dieser fehlerfrei funktionieren kann, sondern auch jene, dass die Legosteine dazu neigen, sich schnell zu verkanten. 
  
  
  Deshalb habe ich mich heute genau um diese Probleme gekümmert und habe einen vorläufigen Aufbau entwickelt. Hierzu würde als Farbsensor der TCS3200 von Adafruit zum Einsatz kommen, der die Farben Rot, Grün und Blau erkennt. Diese drei Farben werden dann über ein Fließband in den jeweiligen Sammelbehälter befördert und alle anderen Farben in einen vierten Farbtopf. Weiterhin bleiben jedoch das Problem des Verkantens im Trichter und die Tatsache, dass mehrere Steine auf einmal an dem Sensor "vorbeilaufen" akut. Eine mögliche Lösung wäre eine mechanische Sperre auf dem Fließband vor dem Sensor oder eine Art Schnecke, die im Trichter jeden Stein ausrichtet und daher einen Abstand zwischen den Steinen schafft. 
  
  ![image](https://user-images.githubusercontent.com/88386279/149964507-e8b4c8b6-da07-4db1-bdbe-ab45680cdb2f.jpeg)
  
  
<b>Mittwoch, der 19.01.2022</b><br>

  Nachdem ich gestern schon einige Fortschritte hinsichtlich einer möglichen Konstruktion bzw. des Aufbaus der Sortiermaschine gemacht habe, habe ich heute weiter über Verbesserungen und eine einfachere, bedinungsfreundlichere Konstruktion nachgedacht. Dabei ist mir die Idee gekommen, dass die Steine nachdem sie den Farbsensor passiert haben auf eine Rutsche fallen, die mit einem Servo-Motor gesteuert ist und damit die Sammelbehälter ansteuert. Die folgende Abbildung zeigt, wie das zumindest schematisch aussehen könnte.

![image](https://user-images.githubusercontent.com/88386279/150133687-41821230-1108-4c34-86d5-7bef72f3ecb5.jpeg)


<b>Donnerstag, der 20.01.2022</b><br>

  Heute habe ich mich verstärkt darum gekümmert, dass der Farbsensor die ersten Farben erkennt. Dazu habe ich mich einem Aufbau im Internet bedient und konnte damit erste Erfolge erzielen. Grün und Blau werden vom Farbsensor fast ohne Probleme erkannt. Allerdings wird Rot gar nicht erkannt. Ebenso sollten die farbigen LEDs im Grundzustand nicht leuchten und nur wenn der Farbsensor eine Farbe erkennt auflecuhten. Im Moment leuchten alle und die richtige LED geht dann aus, wenn diese Farbe erkannt wird. Das untenstehende Video kann direkt bei GitHub.com angeschaut werden und zeigt die Erfolge, aber auch die Problematiken.
  
https://user-images.githubusercontent.com/88386279/150375232-2c323866-8752-4dd2-be7b-aaf81a15e1e7.mp4


<b>Dienstag, der 01.02.2022</b><br>

  Nachdem in der letzten Woche der Informatik-Unterricht entfallen ist, habe ich zu Hause am Sketch für den Farbsensor weitergearbeitet. Im ersten Schritt wurden die Farben Rot, Grün und Blau erkannt und nur im Seriellen Monitor unter den einzelnen RGB-Werten bis 255 angegeben und dahinter wurde dann die Farbe angezeigt. Da diese Art der Anzeige nur am PC möglich ist und nicht in einer Maschine ohne Display oder sonstiges aufrufbar ist, habe ich jeweils eine LED für Rot, Grün und Blau eingesetzt. Diese zeigten dann den erkannten Farbwert an und haben dementsprechend nur kaum Farbabweichungen erkannt, sodass ich stattdessen eine RGB-LED eingebaut habe, die dann auch einige Farben mehr anzeigen kann. In einer RGB-LED sind jeweils eine dimmbare rote, grüne und blaue LED eingebaut. Damit kann jede Farbe erzeugt werden, die gewünscht ist. Da der Farbsensor auf anderer Lichtquellen außer den vier eingebauten, weißen LEDs empfindlich reagiert und falsche Farben erkennt, muss der Sensor im fertigen Projekt in einem dunklen Körper eingebaut sein, damit die Sortiermaschine zuverlässig funktioniert. Das konnte durch die Versuche mit einem dunklen Körper heute bestätigt werden.


![image](https://user-images.githubusercontent.com/88386279/151996191-e932d4d2-186a-43dd-aa92-479cf1a659e8.jpeg)
Aufbau des Arduinos

<details close>
  <summary>Beispiel mit verschiedenfarbigen Pappen</summary>
 
![image](https://user-images.githubusercontent.com/88386279/151996535-3bcfa583-ecb9-483d-9f1b-35f0caf3931b.jpeg)
![image](https://user-images.githubusercontent.com/88386279/151996581-b227ddc0-f393-432f-a897-3a0212ec5c1b.jpeg)
![image](https://user-images.githubusercontent.com/88386279/151996641-b510b65e-95ca-40ca-8ccf-0358edf63988.jpeg)
  
</details>

<b>Mittwoch, der 02.02.2022</b><br>

  Heute ist das Internet in der Schule ausgefallen, sodass die vorgenommene Aufgabe für die Stunde nicht durchgeführt werden konnte. Mein Vorhaben war es einen ersten Servo-Motor in den Sketech einzubinden, sodass danach jeder Farbe eine Winkelposition des Servos zugeordnet werden kann. Damit wäre es möglich ein rotes Objekt der Schachtel 1, ein grünes Objekt der Schachtel 2 und anderes farbige Objekte der anderen Schachten zu zuordnen. Damit würde dann nur noch eine Funktion der Sortiermaschine fehlen. Nämlich die jenige, die die Objekte zu dem Farbsensor bringt.<br></p>
  
<b>Dienstag, der 08.02.2022</b><br>

  In dieser Stunde habe ich versucht den Farbsensor in der Genauigkeit zu verbessern. Außerdem habe geschaut, ob ich mit einigen kleineren Modifikationen den Sensor effektiver und dadurch zuverlässiger gestalten kann, da im Moment durchaus noch nicht immer die richtige Farbe erkannt wird. Zusätzlich habe ich mir überlegt, dass die Anzeige über den Seriellen Monitor am Computer eine gute Ergänzung zur RGB-LED wäre, die auch noch eindeutiger ist. Nach der Schule habe ich mich dann noch weiter mit den Problemen beschäftigt und habe geschaut, ob sie sich lösen lassen. Dabei habe ich den bislang geschriebenen Sketch nahezu gänzlich verworfen und habe einige neue, bisher nicht installierte Bibliotheken eingebunden und konnte damit das erste Mal den Farbsensor bestimmungsgemäß verwenden. Bisher war der Sketech anscheinend eher zufällig funktionabel und es kam dadurch zu den unerklärlichen Ausfällen bei der Farberkennung. Abschließend habe ich noch sehr lange am Abend darauf verwendet, die RGB-LED wieder in den Sketch einzubauen, was allerdings bislang noch nicht geklappt hat. Damit war der Tag erfolgreich auf der einen Seite, aber auch ernüchternd, da ich annähernd drei Stunden vergeblich die LED einbinden wollte und es nicht geklappt hat. Das Ziel für morgen ist dann also genau das zu schaffen.<br></p>

<b>Mittwoch, der 09.02.2022</b><br>

  Nachdem ich mich mir gestern die Ziele für heute gesteckt hatte, war die Motivation groß, das zu schaffen. Doch leider hat das heute wieder nicht geklappt. Am Nachmittag habe ich weiter versucht mit dem Internet eine Lösung zu finden, was sich allerding als sehr schwierig gestaltet hat. Trotzdem ist mir ein Video aufgefallen, indem alle Arbeitsschritte aufwendig beschrieben wurden. So konnte ich einen neuen Sketch ausprobieren, der sehr aufwendig ist und durch einen dafür vorgesehenen Kalibrierungssketch möglichst genaue Werte mit dem Sensor liefert. Der große Vorteil dieses Sketches liegt nicht nur in der Genauigkeit, sondern auch den anderen Sketchen ggü. darin, dass der serielle Monitor mithilfe einer map-Funktion RGB-Werte von 0 bis 255 anzeigt. 
  
<b>Dienstag, der 15.02.2022</b><br>

  Seit der letzten Stunde habe ich viele Stunden in das Projekt gesteckt und versucht dem Ziel näher zu kommen, dass nämlich der Sensor zuverlässig Werte ausgibt, die stimmen und eine RGB-LED, die die Farben richtig wiedergibt. Auch das hat bisher mehr schlecht als recht funktioniert. Zumindest konnte ich nun das Problem finden, was dazu führte, dass die RGB-LED vermeintlich falsche Werte ausgab. Erst durch ausprobieren jeder einzelnen LED innerhalb der RGB-LED kam ich auf den Schluss, dass die blaue Diode einen Fehler hat und nicht mehr leichtet. So kommt es zu dem Problem, dass dauerhaft die Blauwerte in der Farbmischung der LED fehlen und es am Ende andere Farbtöne sind, als der Farbsensor erkennt. Um dieses Problem weiter zu behandeln, muss eine neue RGB-LED bestellt werden. Eine einfache Übergangslösung mithilfe von drei einzelnen LEDs in rot, grün und blau ist nicht ohne großen Schreibaufwand im Sketch möglich, sodass ich dieses Nebenprojekt einstelle bis die neue RGB-LED angekommen ist. 
  Daher habe ich mich nun der Aufgabe gewidmet, dass jede Farbe eine Winkelposition für den Servo-Motor erhält. Dazu habe ich heute angefangen im Internet zu suchen, wie man Farbbereiche festlegt, da "rot" nicht gleich "rot" ist und "blau" nicht gleich "blau". So habe ich angefangen mich über die Arduino-Befehle "frequency", "pulseln" und der einfachen "if-else-Schleife" zu informieren. Am Abend habe dann schonmal eine einfache if-Schleife angefangen, die auch in den Gründzügen schon funktioniert. Die nächsten Schritte sind damit logischerweise, dass es einige Positionen für die Farben auf dem Servo-Motor gibt.
  
<b>Mittwoch, der 16.02.2022</b><br>
  
  Nachdem ich gestern schon mit der if-Schleife angefangen habe, habe diese heute weitergeschrieben. Damit ist es nun möglich Rot, Grün und Blau sehr zuverlässig vom Farbsensor erkennen zu lassen. Die Farberkennung für Weiß funktioniert bislang noch nicht ganz, da es mit den anderen Definitionsbereichen, unter anderem mit dem für Rot, Überschneidungen gibt und der Arduino dann "Rot-Weiß" ausliest. Diese Schwäche gilt es in der nächsten Stunde zu beseitigen. 
  Am Abend habe ich dann noch neue Teile für das Projekt bei Funduino bestellt. So habe ich eine neue RGB-LED bestellt und einen zweiten Servo, um den Aufbau zu komplimitieren. 
  

<b>Dienstag, der 22.02.2022</b><br>

  In dieser Stunde habe ich an der Farberkennung für verschiedene Farben weitergearbeitet. Heute habe ich mich auch an "schwierigere" Farben getraut, die sich aus den Rot-, Grün- und Blauwerten in einer bestimmten Mischung ergeben. Der erste Farbton, der nun lesbar ist, ist Gelb. 
  Ebenso habe ich versucht die Anzeige für die erkannte Farbe zu verbessern, da die erkannte Farbe bislang im Serial Monitor vor den RGB-Werten angegeben wurde. Da aber die Farben unterschiedlich lange Wörter sind, habe ich mich dazu entschieden durch die Funktion "Serial.println(Erkannte Farbe: xxx)" in eine neue Zeile zu schreiben und somit weiterhin für Übersichtlichkeit zu sorgen. 
  
  
<h3 id="kapitel3">3. Materialien</a></h3>

[x] Arduino Uno R3<br>
[x] Breadboard<br>
[x] Farbsensor GY-31<br>
[x] Servo-Motoren<br>
[x] Kabel<br>
[x] RGB-LED<br>

<h3 id="kapitel4">4. Quellen</a></h3></li>

- https://stackoverflow.com/questions/4279611/how-to-embed-a-video-into-github-readme-md/4279746#4279746 
- https://gist.github.com/citrusui/07978f14b11adada364ff901e27c7f61
- https://github.com/MajicDesigns/MD_TCS230/blob/main/README.md
- https://www.arduinolibraries.info/libraries/md_tcs230
- https://docs.arduino.cc/software/ide-v1/tutorials/installing-libraries
- https://www.arduino.cc/reference/en/libraries/freqcount/
- https://forum.arduino.cc/t/mit-dem-farbsensor-tcs-320-rot-erkennen-und-einen-servo-ansteuern/623354 
- https://dronebotworkshop.com/arduino-color-sense/
- https://www.farb-tabelle.de/de/farbtabelle.htm 
