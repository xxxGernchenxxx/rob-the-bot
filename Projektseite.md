Diese Seite ist meine Projektseite. Hier stelle ich mein fertiges Projekt vor und ziehe ein Fazit.

<h2> Inhalt </h2>
<ul style="list-stlye-type:none">
<li><a href="#kapitell">1. Einleitung</a></li>
<li><a href="#kapitel2">2. Arduino und Sketch</a></li>
<li><a href="#kapitel3">3. Projektentwicklung</a></li>
<li><a href="#kapitel4">4. Vorstellung des Projekts</a></li>
<li><a href="#kapitel5">5. Der Sketch</a></li>
<li><a href="#kapitel6">6. Der Farbsensor TCS3200</a></li>
<li><a href="#kapitel7">7. Reflexion und Fazit</a></li>
<li><a href="#kapitel8">8. Eigenständigkeitserklärung</a></li>
<br>
<h2 id="kapitell">1. Einleitung</h2>
  Auch wenn es skuril erscheinen mag, gibt es viele Menschen, die die Unordnung in Schokolinsen-Verpackungen bezüglich der Farbe nervt. Dann könnte man sie natürlich mit der Hand sortieren, aber eine automatisierte Maschine wäre in dem Fall einfacher und bestimmt auch cooler. Mit einer solchen Maschine lassen sich dann auch im größeren Stile Schokolinsen sortieren, um sie zum Beispiel auf Feiern anzubieten.<br>
  
<h2 id="kapitel2">2. Arduino und Sketch</h2>
  Der Arduino ist eine Physical-Computing-Platform, die aus Hard- und Software besteht. Der Arduino besteht aus einer Platine, einem darauf montierten Mikrocontroller und verschiedenen Anschlüssen. So gibt es digitale und analoge Pins, die je nach Anwendung mit Lampen, Mikromotoren, Sensoren oder anderer Hardware verbunden werden können. Bei den digitalen Pins gibt es noch eine zusätzliche Unterscheidung in Pins, bei denen eine ständig gleichbleibende Spannung anliegt und in jene, die mit eine Welle (~) gekennzeichnet sind. Diese Welle steht für die Abkürzung PWM. Pulse Width Modulation (PWM) heißt, dass die am Pin anliegende Spannung geändert werden kann und dies vor allem für dimmbare LEDs bzw. RGB-LEDs nützlich ist. Zudem hat der Arduino noch eine USB-Schnittstelle und einen weiteren Anschluss, um Netzteile oder Batterien mit einem Adapter anstecken zu können. Falls bei einem Projekt die Stromversorgung über das USB-Kabel mit dem Computer nicht ausreicht, kann dieser Anschluss für eine weitere externe Stromquelle genutzt werden.
Mit den Pins lassen sich die genannten Verbraucher entweder direkt anschließen oder mittels eines E/A-Boards mit Widerständen versehen. Damit ist unter anderem eine bessere Übersichtlichkeit der angeschlossenen Module gegeben.<br>
  Von dem Arduino gibt es verschiedene Modelle. Bei diesem Projekt wurde ein Arduino R3 verwendet, der über fünf analoge und dreizehn digitale Pins verfügt. Zudem hat er wie jeder Mikrocontroller Minus-(GND) und Pluspole (3,5V / 5V). Neben diesen "Standardanschlüssen" gibt es noch einige weitere, die aber im Verlauf des Projektes nicht genutzt wurden.<br>
 
<h2 id="kapitel3">3. Projektentwicklung</h2>
  Nachdem das letzte Projekt abgeschlossen war, habe ich mir einige Gedanken gemacht, was ich als nächstes bauen bzw. programmieren möchte. Da kam mir zum einen ein Roboter in den Sinn, der auf Ketten oder Rädern selbst gesteuert fährt und Hindernisse mit Sensoren erkennt und umfahren kann. Bei diesem Roboter hätten sowohl verschiedene Motoren, als auch Sensoren zum Einsatz kommen können. Nach einiger Planung ist mir jedoch bewusst geworden, dass ein selbstfahrender Roboter eine Nummer zu groß ist. Deshalb habe ich im Internet nach Projektvorschlägen für den Arduino gesucht und eine Idee gefunden, die eine Sortiermaschine vorsieht. Diese Idee für Schokolinsen fand ich sofort sehr interessant und witzig in der Umsetzung. Doch auch hier habe ich mich nach einiger Planung auf eine etwas einfachere Umsetzung beschränkt, da meine eigene Weiterentwicklung der Idee zu einer Sortiermaschine für Legosteine wahrscheinliche große mechanische Schwierigkeiten gemacht hätte.<br>
  Auf diese Weise bin ich dann schlussendlich bei dem Vorschlag aus dem Internet für eine Sortiermaschine für Schokolinsen gelandet. Hierzu habe ich mir dann anschließend tiefergehende Planungen gemacht. Zum einen galt es einen passenden Farbsensor zu finden, aber auch einen geeigneten Aufbau zu entwerfen. Mit der Zeit bin ich von Ideen, die eine Förderband beinhalteten abgekommen und habe mich auf Ideen mit Rutschen beschränkt, die die Schwerkraft ausnutzen. Damit bin ich dann auch zu einem geplanten Aufbau gelangt, der folgendermaßen aussieht:<br>
  
  ![image](https://user-images.githubusercontent.com/88386279/163716736-5ec09572-3f91-4a03-b799-1b00b7b15de7.jpeg)
  
<h2 id="kapitel4">4. Vorstellung des Projekts</h2>

https://user-images.githubusercontent.com/88386279/163406224-be4b8d6f-917c-4668-b967-3da22eb10420.mp4
  
  Dieses Video zeigt die Funktionsweise der Sortiermaschine. Ganz oben werden die Schokolinsen mit der Hand in das Rohr hineingegeben. Dieses Rohr dient als Vorratsbehälter, da sich die Linsen dort stapeln. Der erste Servo-Motor bewegt sich dann mit einer Vorrichtung immer vor und zurück. Dabei nimmt er immr nur eine Linse zur Zeit mit und schiebt sie für drei Sekunden unter den Farbsensor. Dort wird der Farbwert ausgelesen. In dieser Zeit stellt sich der Motor mit der Rutsche in die richtige Position ein und die angesteuerte LED in der Verblendung leuchtet auf. Der erste Servo-Motor schiebt die Schokolinse auf die Rutsche und bewegt sich wieder nach hinten zum Vorratsbehälter und beginnt mit einem neuen Durchlauf. Doch bevor dieser startet, rutscht die Linse auf der Rutsche in den richtigen Behälter und die Rutsche stellt sich wieder in die Grundstellung zurück. Dann beginnt ein neuer Durchlauf.<br>
  Öffnet man eine M&M-Schokolinsentüte, dann fallen einem sechs verschiedene Farben bie den Linsen auf. Die sind rot, grün, blau, orange, gelb und braun. Erste Absicht war, dass der Sortiermaschine eine ganze Tüte Schokolinsen in einen Trichter gefüllt werden und die sie dann sortier. Leider ging dieser Plan nicht ganz auf, da die Linsen leicht dazu neigen, sich zu verkanten und die Farberkennung sehr schwierig für gelb, orange und braun zu programmieren ist. Deshalb habe ich mich auf die drei Grundfarben rot, grün und blau beschränkt und den Kompromiss mit einer Röhre statt Trichter gewählt, da somit trotzdem die Sortiermaschine ihren Zweck erfüllt.<br>
  Bei einem Dauertest konnten die besten Ergebnisse erzielt werden, wenn nur schwaches Fremdlicht die Maschine beleuchtet. Ist das der Fall, dann konnten bis zu 25 Schokolinsen ohne Fehler richtig zugeordnet werden. 


<h2 id="kapitel5">5. Der Sketch</h2>
  Den Sketch habe ich selbst zusammengestellt. Den Teil, der für das Auslesen und Ansteuern des Farbsensors notwendig ist, habe ich aus dem Internet von einem YouTube-Video übernommen und den Rest habe ich mir selbst überlegt und aufgeschrieben. Das bedeutet, dass ich die Motorsteuerung und die Ansteuerung der LEDs in den Sketch selbst eingebunden habe genauso wie ich die if-Schleifen eigenstädnig entworfen habe. 
  Im Folgenden möchte ich den Sketch in den drei Teilen Definitionen von Variablen, Void Setup und Void Loop vorstellen:<br>
  
  Definitionen von Variablen:<br>
  
  ![Definitionen von Variablen](https://user-images.githubusercontent.com/88386279/163358696-6ab67091-155b-47dd-a396-9b1aa59da58f.PNG)
  
  In diesem Abschnitt habe ich die Variablen definiert. Das bedeutet ich habe den spezifischen Bezeichnungen besser verstädnliche Bezeichnungen verpasst oder sie erst definiert, damit in den späteren Schritten der Sketch überhaupt funktioniert. Hier kann man sehen, dass ich zu allererst die "Servo.h-Bibliothek" eingebunden habe und anschließend beide verwendeten Servo-Motoren benannt habe, damit ich zu jeder Zeit weiß, welcher Servo, wo sitzt und sich wann bewegt. Anschlißend habe ich die Pins des Farbsensors TCS32000 definiert und dann die RGB-Werte aus dem Kalibrierungs-Sketch für den Farbsensor übertragen. Anschließend habe ich noch weitere Variablen für den Farbsensor niedergeschrieben und abschließend die Pins für die drei LEDs definiert und benannt.<br>
  
  Void Setup:
  
  ![Void Setup](https://user-images.githubusercontent.com/88386279/163359887-777abc22-766a-4cce-ac20-da09e3c9398c.PNG)

  In diesem nächsten Abschnitt werden dann die Pins des Arduinos als Output oder Input versehen. Zudem wird eine Skalierung des Farbsensors vorgenommen und der Serial Monitor wird auf 9600 gesetzt. Das bedeutet, dass die Baudrate auf 9600 definiert wird und damit die Kommunikation zwischen dem Arduino und dem Serial Monitor ermöglicht wird. Im Prinzip dient dann der Serial Monitor, ein Fenster auf dem PC, als Anzeigeplattform für die vom Arduino gesammelten Informationen via Sensoren.
  Zudem habe ich im Void Setup noch die Steuerpins der Motoren und die Pins der LEDs als Output definiert.<br> 
  Im Gegensatz zur Void Loop wird das Void Setup nur einmal vom Arduino abgelesen. Das heißt, dass dieser die Anweisungen nur einmal befolgt und dann für die Schritte in der Loop immer umsetzt.<br>
  
  Void Loop:
  
![Void Loop !](https://user-images.githubusercontent.com/88386279/163361664-086d6d3d-0d13-47a5-b7ee-d7f3c427e1d4.PNG)
  
  In diesem ersten Teil der Void Loop habe ich zuerst die Motorbewegungen zu einem Teil gesteuert. (Der Rest wird dann immer in den gleich noch näher vorgestellten if-Schhleifen vorgenommen.) Zudem werden in diesem Teil noch die durch den Sensor erkannten Farbtemperaturen in den Wertebereich zwischen 0 und 255, dem normalen RGB-Bereich, umgerechnet. Das geschieht mit der Funktion "map". Bei dieser lassen sich die erkannten Werte in einen selbst einstellbaren Bereich umrechnen. Im Prinzip geschieht das mit einem einfachen Dreisatz im Arduino. Außerdem habe ich in diesem Teil die Ausgaben für den Serial Monitor teilweise festgelegt. Das bedeutet, dass die erkannte Farbe zuerst durch die einzelnen RGB-Werte ausgedrückt wird. Das sieht dann folgenermaßen aus: 
  
  ![RGB-Werte einzeln](https://user-images.githubusercontent.com/88386279/163363240-9b318760-1bcb-4144-8c49-bc7a93ae42e2.PNG)<br>
  
  
  ![Void Loop 2](https://user-images.githubusercontent.com/88386279/163363427-e7e47f9a-7a59-4ba9-8280-53200f2dd82e.PNG)
  
  In dem zweiten Teil der Void Loop habe ich die if-Schleifen eingebunden. Im Aufbau gleichen sich diese, unterscheiden sich aber eben in den Farben und den daraus folgenden Winkeln für die Motoren und den Befehlen für den Serial Monitor. Jede if-Schleife fängt mit der selben Bedingung an. Wenn die Farbe "Rot" erkannt werden soll, dann muss der Rot-Wert jeweils größer als der Grün-Wert und der Blau-Wert sein. Das gleiche gilt auch für die anderen Farben in anderer Reihenfolge. Je nachdem welcher Wert der größte ist, wird dann auf dem Serial Monitor noch unter den RGB-Werten die tatsächliche Farbe angezeigt. Das sieht dann so aus:<br>
  
  ![RGB-Wert mit Farbe](https://user-images.githubusercontent.com/88386279/163364240-8210bd5b-2b9d-4a42-858e-b3c0afee7318.PNG)
  
  Ist dies geschehen, wird die jeweilige LED angesteuert und leuchtet für wenige Sekunden auf. Das dauert so lange, bis die LED in der gleichen if-Schleife später wieder ausgeschaltet wird. Nach der Farbe entscheidend, wird dann die Rutsche durch den "ServoRutsche" eingestellt. Dabei variiert er zwischen 0°, 50° und 100°. Ein Delay von einer Sekunde ermöglicht, dass die Rutsche auch wirklich richtig eingestellt ist, bevor der andere Servo die Schokolinse auf die Rutsche schiebt. Nach einem weiteren Delay von einer Sekunde, wird davon ausgegangen, dass die Linse ihr Ziel erreicht hat und der Rutschenmotor wird in Grundstellung gebracht, die jeweilige LED wird wieder auf LOW gesetzt, also ausgeschaltet und der Servo, der für den Schokolinsen-Transport vom Vorratsbehälter zum Farbsensor und zur Rutsche vorgesehen ist, wird bis hinter den Vorratsbehälter bewegt, damit eine neue Schokolinse bewegt werden kann. Dieser Vorgang wird in der Void Loop immer und immer wieder wiederholt.<br>
  
  ![Void Loop 3](https://user-images.githubusercontent.com/88386279/163365562-c1772880-a175-4345-9282-941271290fd3.PNG)
  
  Dieser letzte Teil des Sketches ist nicht wirklich Teil der Void Loop, da die geschweifte Klammer für die Loop schon im anderen Abschnitt geschlossen wurde. Trotzdem wird dieser Vorgang immer wieder wiederholt, da dieser für das Auslesen des Farbsensors zuständig ist. Dabei werden die verschiedenen Pins, die für beim Sensor als Output dienen unter verschiedene Spannungen gesetzt, woraus sich dann vom Arduino Werte errechnen lassen. Jede Farbe wird dabei einzeln ausgelesen.<br>

  
<h2 id="kapitel6">6. Der Farbsensor TCS3200</h2>
  
  Der Farbsensor TCS3200 ist ein Modul zur Erkennung von Farben. Er ist in unterschiedlichen Größen, Formen, Farben und Typen erhältich und wird von mehreren Herstellern produziert. Preislich ist er ein ziemlich günstiger Sensor, da er schon für weniger als 5 EURO zu kaufen ist. In meinem Projekt habe ich einen Sensor vom Typ GY-31 verwendet, den ich über Funduino bezogen habe. Er verfügt über 10 Anschlüsse, wovon VCC und GND doppelt vorhanden sind. Es müssen nur einmal Spannung und Erdung angelegt werden. Zudem hat er die Anschlüsse S0, S1, S2, S3, LED und OUT. In meinem Projekt wurden lediglich nur die Anschlüsse VCC, GND, S0, S1, S2, S3, S4 und OUT gebraucht. Würde man LED mit GND auf dem Arduino verbinden, dann würden die vier vormontierten, weißen LEDs, die optimal den zu erfassenden Bereich ausleuchten, ausgeschaltet werden. Da der Farbsensor mit 3,5 und 5 Volt zu betreiben ist, habe ich 5 Volt als Eingangsspannung benutzt und die optimale Erkennungsdistanz von 1 cm eingehalten. Der eigentliche Sensor besteht aus einem 8 x 8 Array aus Fotodioden. 
  
  ![Farbsensor TCS3200](https://user-images.githubusercontent.com/88386279/163376122-ffbf07aa-d5e5-4693-9b62-3b168273afe5.jpg)

<h2 id="kapitel7">7. Reflexion und Fazit</h2>
  Insgesamt bin ich mit der Wahl des Projekts sehr zufrieden. Über die gesamte Zeit hatte ich Spaß an der Erarbeitung einer funktionierenden Sortiermaschine. Zudem habe ich nach, zugegebenermaßen langen Suche, einen sehr gut funktionierenden Sketch für den Farbsensor gefunden. Trotzdem war es oft nicht einfach, alles selbst zu programmieren, da ich bis auf die Erkenntnisse des vorangestellten Projektes keinerlei Erfahrungen mit dem Prgrammieren hatte. Doch genau das war auch ein Ansporn weiterzumachen und nicht aufzugeben, da ich, je weiter ich mich eingearbeitet hatte, mehr Spaß hatte und jede Menge gelernt habe. Für mich war auch die Mischung aus haptischer Arbeit, also mit den Motoren, dem Sensor und dem Holz, und der digitalen Arbeit, also dem Programmieren und der Erstellung einer GitHub-Seite, ein positiver Faktor. Auch wenn ich die anfangs großen Absichten nicht ganz erreicht habe, kann ich trotzdessen zufrieden mit den Erfolgen sein, da ich alleine gearbeitet habe und vom Programmieren über den Aufbau aus Holz bis hin zum Internetauftritt auf GitHub alles selbst bestreiten musste. Auch kann ich sagen, dass ich mit unter viele Versuche unternommen habe, die Maschine zu verbessern, die aber nicht funktioniert haben, ich aber trotzdem weitergemacht habe. Zu solchen Versuchen gehört zum Beispiel die Entwicklung eines funnktionierenden Trichters im Vorratsspeicher oder eine anschaulichere Rutsche. Auch war dieses Projekt sehr materialsparend, da ich Holz aus dem ersten Inforamtik-Projekt wieder verwendet habe und somit nicht neues Holz kaufen musste.
  
  
<h2 id="kapitel8">8. Eigenständigkeitserklärung</h2>
  
  Hiermit erkläre ich, dass ich die vorliegende Arbeit selbstständig verfasst und keine anderen als die angegebenen Quellen und Hilfsmittel benutzt habe.<br>
  Alle sinngemäß und wörtlich übernommenen Textstellen aus fremden Quellen wurden kenntlich gemacht.<br>
  
  Gernot Zesch
  
  
