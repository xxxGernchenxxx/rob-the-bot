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

  Nachdem in der letzten Woche der Informatik-Unterricht entfallen ist, habe ich zu Hause am Sketch für den Farbsensor weitergearbeitet. Im ersten Schritt wurden die Farben Rot, Grün und Blau erkannt und nur im Seriellen Monitor unter den einzelnen RGB-Werten bis 255 angegeben und dahinter wurde dann die Farbe angezeigt. Da diese Art der Anzeige nur am PC möglich ist und nicht in einer Maschine ohne Display oder sonstiges aufrufbar ist, habe ich jeweils eine LED für Rot, Grün und Blau eingesetzt. Diese zeigten dann den erkannten Farbwert an und haben dementsprechend nur kaum Farbabweichungen erkannt, sodass ich stattdessen eine RGB-LED eingebaut habe, die dann auch einige Farben mehr anzeigen kann. Da der Farbsensor auf anderer Lichtquellen außer den vier eingebauten, weißen LEDs empfindlich reagiert und falsche Farben erkennt, muss der Sensor im fertigen Projekt in einem dunklen Körper eingebaut sein, damit die Sortiermaschine zuverlässig funktioniert. Das konnte durch die Versuche mit einem dunklen Körper heute bestätigt werden.


![image](https://user-images.githubusercontent.com/88386279/151996191-e932d4d2-186a-43dd-aa92-479cf1a659e8.jpeg)
Aufbau des Arduinos

<details open>
  <summary>Beispiel mit verschiedenfarbigen Pappen</summary>
 
![image](https://user-images.githubusercontent.com/88386279/151996535-3bcfa583-ecb9-483d-9f1b-35f0caf3931b.jpeg)
![image](https://user-images.githubusercontent.com/88386279/151996581-b227ddc0-f393-432f-a897-3a0212ec5c1b.jpeg)
![image](https://user-images.githubusercontent.com/88386279/151996641-b510b65e-95ca-40ca-8ccf-0358edf63988.jpeg)
  
</details>






<h3 id="kapitel3">3. Materialien</a></h2></li>

[x] Arduino Uno R3


<h3 id="kapitel4">4. Quellen</a></h2></li>

- https://stackoverflow.com/questions/4279611/how-to-embed-a-video-into-github-readme-md/4279746#4279746 
