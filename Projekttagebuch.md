Diese Seite ist das Projekttagebuch. Hier werden alle Tage, an denen am Projekt gearbeitet wurde, mit einer kurzen Beschreibung erwähnt.

<h1>Bau einer automatischen Sortiermaschine für Legosteine und Schokolinsen mit einem Arduino</h1>

<h3> Inhalt </h3>
<ul style="list-stlye-type:none">
<li><a href="#kapitel1">1. Einleitung</a></h2></li>
<li><a href="#kapitel2">2. Stundenprotokoll</a></h2></li>
<li><a href="#kapitel3">3. Materialien</a></h2></li>
<li><a href="#kapitel4">4. Quellen</a></h2></li>
<br>
<h2 id="kapitel1">1. Einleitung</h2>
<p>Jeder kennt die Situation, dass unsortierte farbige Dinge vor einem auf dem Tisch liegen und einen selbst stört diese Tatsache. Wenige Legosteine oder Schokolinsen zu sortieren, ist kein Problem. Doch bei vielen Steinen wird es zunehmend ein Problem und vor allem eine moonotone Arbeit. Dafür wäre eine Maschine, die diese Arbeit abnimmt bestens geeignet. Ein einfacher Farbsensor mit zwei Motoren im richtigen Zusammenspiel sollten ausreichen, dass die monotone Arbeit wegfällt und der "innere Monk" zufriedengestellt wird.<br></p>

<h3 id="kapitel2">2. Stundenprotokoll</a></h2></li>

<b>Dienstag, der 14.12.2021</b><br>

  Nachdem das letzte Projekt abgeschlossen war, fing direkt ein neues an. Schon vor dem Projektbeginn hatte ich mir gewünscht einen Roboter zu bauen. Diese Überlegungen waren jedoch nicht sehr weit fortgeschritten. Über die Ferien möchte ich mir dazu Gedanken machen. In der letzten Doppelstunde vor den Ferien haben wir dann nicht an Informatik weitergearbeitet, sondern haben ein Spiel Namens "Secret Hitler" in der Klasse gespielt.<br></p>
  
  
<b>Mittwoch, der 15.12.2021</b><br>

  Diese Stunde ist ausgefallen, weil es der letzte Tag vor den Ferien war und wir somit nach der 3. Stunde Schluss hatten.<br></p>


<b>Dienstag, der 11.01.2022</b><br>

  In dieser ersten Doppelstunde des neuen Jahres habe ich bei GitHub angfangen, das neue Projekt zu erstellen. Dazu habe ich ein neues Repository erstellt und eine File eingefügt, in der ich nun das Projekttagebuch erstelle. Hier werden jegliche Arbeitsschritte dokumentiert.
Während der Ferien und heute habe ich weiter über die Idee eines Roboters und dessen Funktionen nachgedacht. Dabei bin ich auf einen Farbsensor im Internet gestoßen, der interessante Anwendungsmöglichkeiten zulässt. Für einen Roboter bin ich nicht merklich weitergekommen, weil die Umsetzung des Fahrwerks mit Rädern oder Ketten schwierig ist und auch die praxisnahen Funktionen nicht einfach zu programmieren sind. Deshalb habe ich mich gegen den Bau eines Roboters entschieden. Bei Recherchen im Internet zu Farbsensoren und anderen technischen Komponenten bin ich auf eine Sortiermaschine für bunte Schokolinsen gestoßen. Diese Idee finde ich sehr interessant und außergwöhnlich. Zudem scheint die Umsetzung nicht besonders schwierig, sodass ich mich nun auch auf eine Sortiermaschine konzentrieren möchte, die allerdings Legosteine nach Farben sortiert.<br></p> 


<b>Mittwoch, der 12.01.2022</b><br>

  Nachdem ich mich letzte Stunde gegen den Bau eines Roboters entschieden habe und nun eine Sortiermaschine basteln möchte, habe ich an dieser Idee weitergearbeitet. Die Maschine soll möglichst Legosteine nach Farbe sortieren und dann, wenn möglich auch noch nach Größe. Das Funktionsprinzip dieser Schritte habe ich mir heute weiter überlegt. Doch hier stellen sich die ersten Schwierigkeiten mir in den Weg, da die Quader sich leicht verkanten und eine mechanische Lösung kompliziert ist. Deshalb fokussiere ich mich ab diesem Zeitpunkt auf die Umsetzung einer Sortiermaschine für Schokolinsen. Trotzdem möchte ich das Hauptprojekt mit den Legosteinen nicht vernachlässigen und mir weiterhin Gedanken zu diesem Thema machen, da mich beide Wege am Ende einem funktionsfähigen Projekt näher bringen.<br></p>
  
  
<b>Dienstag, der 18.01.2022</b><br>

  Heute habe ich mich primär mit der Thematik beschäftigt, welcher Farbsensor verwendet werden soll und wie die Legosteine bzw. Schokolinsen zu dem Farbsensor gelangen, sodass sie richtig zugeordnet werden können. Das umfasst nicht nur die Problematik, dass die Legosteine / Schokolinsen nur einzeln in dem Bereich des Farbsensors sein dürfen, damit dieser fehlerfrei funktionieren kann, sondern auch jene, dass die Legosteine dazu neigen, sich schnell zu verkanten. 
  
  
  Deshalb habe ich mich heute genau um diese Probleme gekümmert und habe einen vorläufigen Aufbau entwickelt. Hierzu würde als Farbsensor der TCS3200 von Adafruit zum Einsatz kommen, der die Farben Rot, Grün und Blau erkennt. Diese drei Farben werden dann über ein Fließband in den jeweiligen Sammelbehälter befördert und alle anderen Farben in einen vierten Farbtopf. Weiterhin bleiben jedoch das Problem des Verkantens im Trichter und die Tatsache, dass mehrere Steine auf einmal an dem Sensor "vorbeilaufen" akut. Eine mögliche Lösung wäre eine mechanische Sperre auf dem Fließband vor dem Sensor oder eine Art Schnecke, die im Trichter jeden Stein ausrichtet und daher einen Abstand zwischen den Steinen schafft. 
  
  ![image](https://user-images.githubusercontent.com/88386279/149964507-e8b4c8b6-da07-4db1-bdbe-ab45680cdb2f.jpeg)
  
  
<b>Mittwoch, der 19.01.2022</b><br>

  Nachdem ich gestern schon einige Fortschritte hinsichtlich einer möglichen Konstruktion bzw. des Aufbaus der Sortiermaschine gemacht habe, habe ich heute weiter über Verbesserungen und eine einfachere, bedinungsfreundlichere Konstruktion nachgedacht. Dabei ist mir die Idee gekommen, dass die Steine nachdem sie den Farbsensor passiert haben auf eine Rutsche fallen, die mit einem Servo-Motor gesteuert ist und damit die Sammelbehälter ansteuert. Die folgende Abbildung zeigt, wie das zumindest schematisch aussehen könnte.

![image](https://user-images.githubusercontent.com/88386279/150133687-41821230-1108-4c34-86d5-7bef72f3ecb5.jpeg)


<b>Donnerstag, der 20.01.2022</b><br>

  Heute habe ich mich verstärkt darum gekümmert, dass der Farbsensor die ersten Farben erkennt. Dazu habe ich mich einem Aufbau im Internet bedient und konnte damit erste Erfolge erzielen. Grün und Blau werden vom Farbsensor fast ohne Probleme erkannt. Allerdings wird Rot gar nicht erkannt. Ebenso sollten die farbigen LEDs im Grundzustand nicht leuchten und nur wenn der Farbsensor eine Farbe erkennt auflecuhten. Im Moment leuchten alle und die richtige LED geht dann aus, wenn diese Farbe erkannt wird. Das untenstehende Video kann direkt bei GitHub.com angeschaut werden und zeigt die Erfolge, aber auch die Probleme.
  
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
  
<b>Mittwoch, der 23.02.2022</b><br>

  Die neue Weise des Aufschriebs der erkannten Farbe funktioniert an sich gut und ist auch übersichtlich, jedoch kommt es durch die Software häufiger zu Problemen mit dem Farbton Gelb, da die if-Schleife dreimal von bisherigen fünf if-Schleifen für "true" befunden wird und es deshalb zu der Farbausgabe "Rot", "Weiß" und "Gelb" kommt. Das stellt natürlich ein Problem für die Sortierung der Farben dar. 
  
  ![if Schleife](https://user-images.githubusercontent.com/88386279/155320218-ffb6d12f-7b5b-433d-83df-f8b29610f5aa.PNG)
  
  Anzeige der drei Farben zur gleichen Zeit
  
<b>Dienstag, 01.03.2022</b><br>
  
  Über das Wochenenede habe ich mich dazu entschieden, dass ich im nächsten Schritt den Korpus der Sortiermaschine für Schokolinsen baue, um damit zu überprüfen, ob der geplante Aufbau mit den Servos und dem Farbsensor richtig funktioniert. Danach kann ich dann trotzdem die Farberkennung weiterprogrammieren, da sie nur von der Software abhängig ist und nicht von der Hardware. Wichtig ist es, dass bei der Erarbeitung des Aufbaus genügend Sammelbehälter für die verschiedenen Farben berücksichtigt werden. 
  Dementsprechend habe ich mich heute vorwiegend mit der Planung des Aufbaus beschäftigt und nebenbei die GitHub-Seiten überarbeitet und um ein ReadMe ergänzt.
  
<b>Mittwoch, 02.03.2022</b><br>

  In dieser Stunde habe ich weiter den Bauzeichnungen gearbeitet und die Konstruktion auf Funktionsfähigkeit überdacht. Am Ende bin ich zu einer Form eines Quaders gekommen, der oben eine Öffnung, wo die zu sortiereneden Schokolinsen eingefüllt werden, und unten an der Stirnseite kleine "Schubladen" bzw. Entnahmemöglichkeiten hat, wo die sortierten Schokolinsen herausgenommen werden können.
  
  ![image](https://user-images.githubusercontent.com/88386279/156361523-0b89e777-1f5f-4018-889e-6804c4372c38.jpeg)
  
  Obere Skizze: Funktionsweise<br>
  Untere Skizze: Geplante Draufsicht auf die fertige Schokolinsen-Sortiermaschine<br>
  
  Zudem habe ich heute begonnen, die Maschine anhand der angefertigten Pläne zu bauen und die ersten Elektronikkomponenten an die richtigen Stellen zu bringen.

<b>Sonntag, 06.03.2022</b><br>

  Am Wochenende habe ich angefangen, das Gehäuse für die Technik aus Holz zu bauen. Dabei habe ich die Konzeption noch etwas geändert, da ich Bedenken hinsichtlich der Umsetzung und der anschließenden Funktionstüchtigkeit hatte. Von den technischen Komponenten bleibt der Aufbau gleich. Als einzige Veränderung ist die Sortiermaschine nun deutlich höher als breit, da ich dadurch größere Gefälle zur Verfügung habe, damit die Schokolinsen schneller rutschen und nicht auf der Rutsche liegen bleiben.
  
<b>Mittwoch, 09.03.2022</b><br>

  Heute habe ich die neue Skize für den Aufbau entworfen und mich dem weiteren Bau des Gehäuses gewidmet, damit ich möglichst zeitnah mit dem Einabu der Technik beginnen kann und in der Folge die Farbwerte für die sechs verschiedenen Farben der Schokolinsen von M&M bestimmen kann. 
  
  ![image](https://user-images.githubusercontent.com/88386279/157540933-8b3fa102-9bcb-4a63-b483-253634ac7858.jpeg)<br>
  Der neue Aufbau der Sortiermaschine (Außenansicht)
  
<b>Samstag, 12.03.2022</b><br>

  Heute habe ich einige Materialien aus dem Baumarkt besorgt und mich um die Positionierung der Motoren im Gehäuse gekümmert. Einer der Motoren übernimmt die Aufgabe die Schokolinsen vom Vorratsbehälter zum Farbsensor zu bewegen und anschließend auf die Rutsche zu bringen. Diese Rutsche führt direkt in den richtigen Sammelbehälter und wird über den anderen Servo-Motor gesteuert. Wichtig dabei ist, dass man die Postion des Motors beachtet, damit eine optimale Balance der durch die Motoren beweglichen Teile erhält und damit auch eine optimale Kraftausbeute bzw. Schnelligkeit erreicht wird. Werden diese Positionen nicht beachtet, kommt es wahrscheinlich zu ungeahnten Komplikationen im Betrieb, die durch eine sorgfältige Planung leicht zu umgehen sind. 
  
<b>Sonntag, 13.03.2022</b><br>

  Auch an diesem Tag habe ich an dem Gehäuse weitergearbeitet. Nach dem heutigen Tag habe ich die Bewegungseinheit, die die Schokolinse vom Vorratsbehälter zum Farbsensor bewegt und anschließend zur Rutsche bringt fertiggestellt.
  
  Bild folgt!!
  
<b>Dienstag, 15.03.2022</b><br>

  Nachdem ich am Wochenende mit dem Bau des Gehäuses deutlich vorangekommen bin, konnte ich heute die einzelnen vormontierten Bauteile erstmals zusammenfügen und im Unterricht testen, ob alles so funktioniert, wie ich es mir vorgestellt habe. Insgesamt bin ich sehr zufrieden mit den bisherigen Ergebnissen. Die bewusst leichten Holzteile werden von den Servomotoren ohne Probleme zügig bewegt und auch die Stromversorgung durch den Computer reicht aus und wäre gegebenenfalls noch durch eine 9-Volt-Batterie zu verstärken. 
  Bei dem ersten Praxistest ist mir nun auch ein Fehler bei einem Bauteil aufgefallen, der mir in der Planung noch nicht bewusst war, sodass ich dieses neukonstruieren muss.
  Mit dem Test ergaben sich jedoch auch die ersten Schwierigkeiten. So ist es wichtig, dass die Motoren in ihrer Bewegung genau aufeinander abgestimmt sind, da ansonsten der Zweck der Sortiermaschine verloren geht und die Schokolinsen am Ende willkürlich in die Sammelbehälter rutschen und eine Farbsortierung nicht gewährleistet ist. 
  Gegen Ende der Stunde habe ich mich wieder dem Sketch zugewandt und schon einige Winkelpositionen für die Servomotoren festgelegt und vorher noch den zweiten Servo in den Sketech intergriert. 
  
<b>Mittwoch, 16.03.2022</b><br>

  In dieser Stunde habe ich mich nach einiger Zeit wieder der Dokumentation des Projekts bei GitHub zugewandt und einige Einträge verbessert und welche für die letzten drei Arbeitstage ergänzt.
  
<b>Dienstag, 22.03.2022</b><br>

  Nachdem ich die letzten Stunden vor allem an der Funktionstüchtigkeit der Servo-Motoren gearbeitet habe, habe heute wieder an der Farberkennung programmiert. Dabei sind mir wie beim letzten Mal die gleichen Schwierigkeiten wieder aufgefallen. Das Problem ist, dass der Arduino zwei oder mehr Farben bei einer Schokolinse erkennt. Dieser Fehler tritt jedoch erst dann auf, wenn ich außerhalb der drei Grundfarben Rot, Grün und Blau, versuche die anderen Farben Gelb, Orange und Braun zu programmieren. Bislang funktionieren diese Grundfarben einwandfrei und sicher im Betrieb. Das lieg daran, dass für diese Farben allgemeingültige Aussagen getroffen werden können, die für die anderen drei Farben nicht zu treffen sind. 
  
![Allgemeingültige Aussage](https://user-images.githubusercontent.com/88386279/159514567-163870ad-4ff2-4898-8dab-78660d7fac32.PNG)<br>
Allgemeingültige Aussage, d.h. ohne spezifische RGB-Werte

<b>Samstag, 09.04.2022</b><br>

  In den letzten Tagen habe ich den Aufbau vervollständigt, sodass dieser nun einsatzbereit ist. Eventuell können hier nach Abschluss der Programmierphase noch einige Schönheitsoptimierungen vorgenommen werden, aber bis dahin müssen die Farberkennung und der Sortiermechanismus noch fertig programmiert werden. 
  Heute habe ich daher mit den bislang sicher erkannten Farben Rot, Grün und Blau den ersten richtigen Praxisversuch vorgenommen. Ich habe die verschiedenfarbigen Linsen in die Maschine befüllt und sie dann einfach laufen lassen. Währenddessen habe ich noch einige Verbesserungen gemacht, wie zum Beispiel die zeitliche Abstimmung von Bewegungen der Motoren und Winkelabstimmungen an den Servo-Motoren. Nun ist mir jedoch folgendes Problem aufgefallen:
  Die Schokolinsen werden teilweise trotz unterschiedlicher Farbe und richtiger Programmierung in den gleichen Sammelbehälter geworfen. Nach langem Überlegen ist mir dann bewusst geworden, dass der Farbsensor nicht synchron zu den Motorabläufen die Farben ausließt. Das bedeutet, dass der Sensor nicht Farbe der Schokolinse an die Motoren weitergibt, sondern die Farbe des Holzes. Dadurch werden alle Linsen in die gleiche Box befördert und nicht sortiert. Ein einfacher und vielversprechender Ansatz wäre, dass man die Zeit, in der die Schokolinse vom Sensor auf die Farbe untersucht wird, deutlich verlängert und dadurch das richtige Signal zugeordnet wird. Andere Lösungsmöglichkeiten wären die Abstimmung zwischen Motor und Sensor zu verfeinern. Diese Möglichkeit ist jedoch sehr aufwendig und schwierig, weshalb ich mich für erstere entshieden habe.

<b>Sonntag, 10.04.2022</b><br>

  Nach einigem Überlegen habe ich eine Lösung für das gestrige Problem gefunden, die deutlich besser als die gestern vorgesehene Lösung ist. Ich habe mir heute noch einmal den Sketch sorgfältig angesehen und habe einige Dinge im Loop geändert, sodass der Farbsensor jetzt häufiger die Farbe ausließt. Zudem habe ich den Loop in der Reihenfolge so umgestellt, dass die Motorbewegungen nun synchron mit dem Ausleseprozess des Farbsensors sind. Damit habe ich ein entscheidendes Problem gelöst. 
  Auch habe ich heute eine Rutsche aus Modellbauplastik gebastelt, die bislang gut funktioniert.
  
   ![20220411_114054](https://user-images.githubusercontent.com/88386279/162713268-683e94c6-4711-4e12-b229-f8f9babc9155.jpg) 
   ![20220411_114119](https://user-images.githubusercontent.com/88386279/162713279-6b48c5e0-e283-48b9-be9f-12c4cd5845d8.jpg)
   
Auf der Unterseite der Rutsche habe ich ein Aufnahmestück zwischen Servo-Motor und Rutsche mit Plastikkleber angeklebt.

<b>Montag, 11.04.2022</b><br>

  Heute habe ich weiter an der Funktionstüchtigkeit gearbeitet. Da die Rutsche aus Plastik nun doch zu schwer war, habe ich eine aus Papier gebastelt. Diese ist leichter und lässt sich theoretisch vom Servo-Motor leichter bewegen. Leider haben sich jedoch auch wieder neue Probleme aufgetan, die wahrscheinlich auf den Arduino bzw. die Motoren zurückzuführen sind. Oftmals bewegen sie sich nicht so, wie im Sketch vorgesehen und auch programmiert.
  

<b>Mittowch, 13.04.2022</b><br>

  Auch an diesem Tag habe ich weiter versucht, die Probleme und die unkontrollierten Bewegungen der Motoren zu lösen. Nach vielen Stunden erfolgloser Arbeit habe ich mich entschieden, mit dem Schreiben der Projektseite zu beginnen. Auf dieser stelle ich das geplante Projekt vor und reflektiere den Arbeitsprozess.
  
<b>Donnerstag, 14.04.2022</b><br>  
  
  Nachdem ich gestern die Projektseite angefangen habe zu schreiben, habe ich heute an der Seite weitergearbeitet. Nun fehlen nur noch wenige Themen, die ich in den nächsten Tagen noch ergänzen werde. Außerdem habe ich heute drei LEDs im Aufbau ergänzt, die die jeweils erkannte Farbe anzeigen. Dazu habe ich den Sketch etwas abgeändert und die Funktion "digitalWrite" verwendet. Dann habe ich eine kleine Verblendung aus Holz gebastelt, die die Technik mit den ganzen Kabeln etwas verdeckt. In dieser Blende sind die drei LEDs eingelassen.<br>
  
  ![Aufbau](https://user-images.githubusercontent.com/88386279/163405004-064710bb-ce86-43db-b61c-cdecb5f2d8ae.png)<br>
  Der wahrscheinlich nahezu finale Aufbau.

  
  
<h3 id="kapitel3">3. Materialien</a></h3>

[x] Arduino Uno R3<br>
[x] Breadboard<br>
[x] Farbsensor GY-31<br>
[x] 2 Servo-Motoren<br>
[x] Kabel (männlich-männlich; weiblich-weiblich; männlich-weiblich)<br>
[x] LEDs (rot, grün, blau)<br>
[x] Holz
[x] Papier, Klebeband

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
- https://www.arduino.cc/reference/de/
